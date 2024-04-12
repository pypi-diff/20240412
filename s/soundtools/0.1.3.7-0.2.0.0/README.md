# Comparing `tmp/soundtools-0.1.3.7.tar.gz` & `tmp/soundtools-0.2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundtools-0.1.3.7.tar", last modified: Wed Apr 10 17:23:06 2024, max compression
+gzip compressed data, was "soundtools-0.2.0.0.tar", last modified: Fri Apr 12 20:02:15 2024, max compression
```

## Comparing `soundtools-0.1.3.7.tar` & `soundtools-0.2.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 17:23:06.475005 soundtools-0.1.3.7/
--rw-rw-rw-   0        0        0      345 2024-04-10 17:23:06.474431 soundtools-0.1.3.7/PKG-INFO
--rw-rw-rw-   0        0        0      224 2024-04-10 02:26:25.000000 soundtools-0.1.3.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-10 17:23:06.475005 soundtools-0.1.3.7/setup.cfg
--rw-rw-rw-   0        0        0      411 2024-04-10 17:22:51.000000 soundtools-0.1.3.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 17:23:06.447934 soundtools-0.1.3.7/soundtools/
--rw-rw-rw-   0        0        0      369 2024-04-07 11:11:28.000000 soundtools-0.1.3.7/soundtools/__init__.py
--rw-rw-rw-   0        0        0    35281 2024-04-10 17:22:08.000000 soundtools-0.1.3.7/soundtools/soundtools.py
-drwxrwxrwx   0        0        0        0 2024-04-10 17:23:06.474002 soundtools-0.1.3.7/soundtools.egg-info/
--rw-rw-rw-   0        0        0      345 2024-04-10 17:23:06.000000 soundtools-0.1.3.7/soundtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-10 17:23:06.000000 soundtools-0.1.3.7/soundtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 17:23:06.000000 soundtools-0.1.3.7/soundtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-10 17:23:06.000000 soundtools-0.1.3.7/soundtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 20:02:15.058745 soundtools-0.2.0.0/
+-rw-rw-rw-   0        0        0      701 2024-04-12 20:02:15.057748 soundtools-0.2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2024-04-10 02:26:25.000000 soundtools-0.2.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 20:02:15.058745 soundtools-0.2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      789 2024-04-12 20:01:40.000000 soundtools-0.2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 20:02:15.055690 soundtools-0.2.0.0/soundtools/
+-rw-rw-rw-   0        0        0      369 2024-04-07 11:11:28.000000 soundtools-0.2.0.0/soundtools/__init__.py
+-rw-rw-rw-   0        0        0    36057 2024-04-12 19:59:12.000000 soundtools-0.2.0.0/soundtools/soundtools.py
+drwxrwxrwx   0        0        0        0 2024-04-12 20:02:15.057748 soundtools-0.2.0.0/soundtools.egg-info/
+-rw-rw-rw-   0        0        0      701 2024-04-12 20:02:14.000000 soundtools-0.2.0.0/soundtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-12 20:02:14.000000 soundtools-0.2.0.0/soundtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 20:02:14.000000 soundtools-0.2.0.0/soundtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-12 20:02:14.000000 soundtools-0.2.0.0/soundtools.egg-info/top_level.txt
```

### Comparing `soundtools-0.1.3.7/soundtools/soundtools.py` & `soundtools-0.2.0.0/soundtools/soundtools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
+version: 0.2.0.0
+
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves"""
 
 
@@ -15,16 +17,17 @@
 import matplotlib.pyplot as plt
 import librosa.effects as effect
 from os.path import splitext
 from pydub.audio_segment import AudioSegment
 from soundfile import read as sfRead
 
 
-# types #
-SoundBuffer = np.ndarray[np.any, np.dtype[np.float32|np.int16|np.uint8]]
+# types
+Dtype = np.dtype[np.float32|np.int16|np.uint8]
+SoundBuffer = np.ndarray[np.any, Dtype]
 Wave = Callable[[float, float, float], SoundBuffer]
 
 
 # its just a dictionary
 class Notes(dict[str, float]):
     """a dictionary used to store note names and frequencies"""
     def __init__(self):
@@ -50,15 +53,15 @@
         self.two_oper_pi = 2/np.pi
         self.four_over_pi = 4/np.pi
         self.eight_over_pi_sqr = 8/np.pi**2
         
         self.change_dtype(dtype)
     
     
-    def change_dtype(self, dtype):
+    def change_dtype(self, dtype: Dtype):
         self.dtype = dtype
         if self.dtype == np.float32:
             self.min_amp = -1
             self.max_amp = 1
         else:
             i = np.iinfo(self.dtype)
             self.min_amp = i.min
@@ -93,15 +96,15 @@
                 result[result < -1] = self.min_amp
                 self.existed_notes[name] = self.array_to_tuple(temp)
                 
                 return result
             return wrapper
         return decorator
 
-    @cache_wave("sine")
+    # @cache_wave("sine")
     def sine_wave(self, freq:float, dur:float, vol: float) -> SoundBuffer:
         """creates a sine wave based on the given frequency, duration and amplituse or volume
         returns a numpy array"""
         
         wave = (vol * np.sin(self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate)).astype(self.dtype)
         return wave
     
@@ -139,15 +142,15 @@
             if f > 20000:
                 break
             buf += (-1)**h * harmonic**(-2) * np.sin(self.tau * np.arange(self.default_sample_rate * dur) * f / self.default_sample_rate)
         
         wave = ((self.eight_over_pi_sqr)*vol*buf).astype(self.dtype)
         return wave
     
-    @cache_wave("fast_tri")
+    # @cache_wave("fast_tri")
     def fast_triangle_wave(self, freq:float, dur:float, vol: float) -> SoundBuffer:
         return (self.two_oper_pi * vol * np.arcsin(np.sin(self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate))).astype(self.dtype)
     
     @cache_wave("saw")
     def sawtooth_wave(self, freq:float, dur:float, vol: float) -> SoundBuffer:
         """returns a numpy array,
         creates a sawtooth wave based on the given frequency, duration and amplitude or volume\n
@@ -271,24 +274,39 @@
                 break
             buf += (-1)**h * (np.sin(self.tau * np.arange(self.default_sample_rate * dur) * f / self.default_sample_rate)/h)
         
         wave = (vol * (0.5 - self.rev_pi*buf)).astype(self.dtype)
         return wave
     
     
-    def fade_in_out(self, buffer: SoundBuffer, fadein_len:int = 1500, fadeout_len:int = 1500) -> SoundBuffer:
-        fadein = ((1 - np.cos(np.linspace(0, np.pi, fadein_len))) * 0.5).astype(buffer.dtype)
-        fadeout = np.flip(fadein)
-        
+    def _generate_fade_buffer(self, fade_len:int = 1500, dtype: Dtype|None=None) -> SoundBuffer:
+        dtype = self.dtype if not dtype else dtype
+        return ((1 - np.cos(np.linspace(0, np.pi, fade_len))) * 0.5).astype(dtype)
+    
+    
+    def fade_in(self, buffer: SoundBuffer, fadein_len:int = 1500) -> SoundBuffer:
+        fadein = self._generate_fade_buffer(fadein_len, buffer.dtype)
         buffer[:fadein_len] *= fadein
+        return buffer
+    
+    
+    def fade_out(self, buffer: SoundBuffer, fadeout_len:int = 1500) -> SoundBuffer:
+        fadein = self._generate_fade_buffer(fadeout_len, buffer.dtype)
+        fadeout = np.flip(fadein)
         buffer[-fadeout_len:] *= fadeout
         
         return buffer
     
     
+    def fade_in_out(self, buffer: SoundBuffer, fadein_len:int = 1500, fadeout_len:int = 1500) -> SoundBuffer:
+        buffer = self.fade_in(buffer, fadein_len)
+        buffer = self.fade_out(buffer, fadeout_len)
+        return buffer
+    
+    
     def array_to_tuple(self, np_array: SoundBuffer) -> tuple:
         """Iterates recursivelly."""
         try:
             return tuple(self.array_to_tuple(_) for _ in np_array)
         except TypeError:
             return np_array
 
@@ -749,16 +767,19 @@
         self.stream = self.AUDIO_OBJECT.open(format=self.AUDIO_OBJECT.get_format_from_width(sampwidth),
                                              channels=data.ndim,
                                              rate=sample_rate,
                                              output=True)
         self.play_buffer(data)
     
     
-    def visualize_sound(self, wave: SoundBuffer, sample_rate: int) -> None:
+    def visualize_sound(self, wave: SoundBuffer, sample_rate: int|None=None) -> None:
         """uses matplotlib.pyplot to visualize sound waves"""
+        
+        sample_rate = self.sample_rate if not sample_rate else sample_rate
+        
         times = np.linspace(0, wave.size/sample_rate, wave.size)
         duration = wave.size / sample_rate
         
         plt.figure(figsize=(15, 5))
         plt.plot(times, wave)
         plt.title('wave:')
         plt.ylabel('Signal Value')
```

