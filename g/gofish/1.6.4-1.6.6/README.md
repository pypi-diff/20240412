# Comparing `tmp/gofish-1.6.4.tar.gz` & `tmp/gofish-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gofish-1.6.4.tar", last modified: Mon Apr 10 00:11:52 2023, max compression
+gzip compressed data, was "gofish-1.6.6.tar", last modified: Fri Apr 12 12:53:17 2024, max compression
```

## Comparing `gofish-1.6.4.tar` & `gofish-1.6.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-04-10 00:11:52.405613 gofish-1.6.4/
--rw-r--r--   0 richardteague   (501) staff       (20)    35149 2023-03-27 18:30:37.000000 gofish-1.6.4/LICENSE.md
--rw-r--r--   0 richardteague   (501) staff       (20)      392 2023-04-10 00:11:52.405493 gofish-1.6.4/PKG-INFO
--rw-r--r--   0 richardteague   (501) staff       (20)     2778 2023-03-27 18:30:37.000000 gofish-1.6.4/README.md
-drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-04-10 00:11:52.404680 gofish-1.6.4/gofish/
--rw-r--r--   0 richardteague   (501) staff       (20)      104 2023-03-27 18:30:38.000000 gofish-1.6.4/gofish/__init__.py
--rw-r--r--   0 richardteague   (501) staff       (20)    45466 2023-04-09 23:58:51.000000 gofish-1.6.4/gofish/annulus.py
--rw-r--r--   0 richardteague   (501) staff       (20)   190217 2023-04-10 00:09:47.000000 gofish-1.6.4/gofish/gofish.py
-drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-04-10 00:11:52.405338 gofish-1.6.4/gofish.egg-info/
--rw-r--r--   0 richardteague   (501) staff       (20)      392 2023-04-10 00:11:52.000000 gofish-1.6.4/gofish.egg-info/PKG-INFO
--rw-r--r--   0 richardteague   (501) staff       (20)      232 2023-04-10 00:11:52.000000 gofish-1.6.4/gofish.egg-info/SOURCES.txt
--rw-r--r--   0 richardteague   (501) staff       (20)        1 2023-04-10 00:11:52.000000 gofish-1.6.4/gofish.egg-info/dependency_links.txt
--rw-r--r--   0 richardteague   (501) staff       (20)       38 2023-04-10 00:11:52.000000 gofish-1.6.4/gofish.egg-info/requires.txt
--rw-r--r--   0 richardteague   (501) staff       (20)        7 2023-04-10 00:11:52.000000 gofish-1.6.4/gofish.egg-info/top_level.txt
--rw-r--r--   0 richardteague   (501) staff       (20)       38 2023-04-10 00:11:52.405652 gofish-1.6.4/setup.cfg
--rw-r--r--   0 richardteague   (501) staff       (20)      593 2023-04-09 23:58:37.000000 gofish-1.6.4/setup.py
+drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2024-04-12 12:53:17.141147 gofish-1.6.6/
+-rw-r--r--   0 richardteague   (501) staff       (20)    35149 2023-03-27 18:30:37.000000 gofish-1.6.6/LICENSE.md
+-rw-r--r--   0 richardteague   (501) staff       (20)      392 2024-04-12 12:53:17.141023 gofish-1.6.6/PKG-INFO
+-rw-r--r--   0 richardteague   (501) staff       (20)     2778 2023-03-27 18:30:37.000000 gofish-1.6.6/README.md
+drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2024-04-12 12:53:17.140312 gofish-1.6.6/gofish/
+-rw-r--r--   0 richardteague   (501) staff       (20)      104 2023-03-27 18:30:38.000000 gofish-1.6.6/gofish/__init__.py
+-rw-r--r--   0 richardteague   (501) staff       (20)    45466 2023-04-09 23:58:51.000000 gofish-1.6.6/gofish/annulus.py
+-rw-r--r--   0 richardteague   (501) staff       (20)   193338 2024-04-12 12:52:54.000000 gofish-1.6.6/gofish/gofish.py
+drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2024-04-12 12:53:17.140903 gofish-1.6.6/gofish.egg-info/
+-rw-r--r--   0 richardteague   (501) staff       (20)      392 2024-04-12 12:53:17.000000 gofish-1.6.6/gofish.egg-info/PKG-INFO
+-rw-r--r--   0 richardteague   (501) staff       (20)      232 2024-04-12 12:53:17.000000 gofish-1.6.6/gofish.egg-info/SOURCES.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)        1 2024-04-12 12:53:17.000000 gofish-1.6.6/gofish.egg-info/dependency_links.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)       38 2024-04-12 12:53:17.000000 gofish-1.6.6/gofish.egg-info/requires.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)        7 2024-04-12 12:53:17.000000 gofish-1.6.6/gofish.egg-info/top_level.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)       38 2024-04-12 12:53:17.141192 gofish-1.6.6/setup.cfg
+-rw-r--r--   0 richardteague   (501) staff       (20)      593 2024-04-12 12:53:06.000000 gofish-1.6.6/setup.py
```

### Comparing `gofish-1.6.4/LICENSE.md` & `gofish-1.6.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gofish-1.6.4/README.md` & `gofish-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `gofish-1.6.4/gofish/annulus.py` & `gofish-1.6.6/gofish/annulus.py`

 * *Files identical despite different names*

### Comparing `gofish-1.6.4/gofish/gofish.py` & `gofish-1.6.6/gofish/gofish.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,32 +28,35 @@
         primary_beam (Optional[str]): Path to the primary beam as a FITS file
             to apply the correction.
         bunit (Optional[str]): If no `bunit` header keyword is found, use this
             value, e.g., 'Jy/beam'.
         pixel_scale (Optional[float]): If no axis information is found in the
             header, use this value for the pixel scaling in [arcsec], assuming
             an image centered on 0.0".
+        restfreq (Optional[float]): A user-specified rest-frame frequency in
+            [Hz] that will override the one found in the header.
     """
 
     frequency_units = {'GHz': 1e9, 'MHz': 1e6, 'kHz': 1e3, 'Hz': 1e0}
     velocity_units = {'km/s': 1e3, 'm/s': 1e0}
 
     def __init__(self, path, FOV=None, velocity_range=None, verbose=True,
-                 primary_beam=None, bunit=None, pixel_scale=None):
+                 primary_beam=None, bunit=None, pixel_scale=None,
+                 restfreq=None):
 
         # Default parameters for user-defined values.
 
         self._user_bunit = bunit
         self._user_pixel_scale = pixel_scale
         if self._user_pixel_scale is not None:
             self._user_pixel_scale /= 3600.0
 
         # Read in the FITS data.
 
-        self._read_FITS(path)
+        self._read_FITS(path, restfreq=restfreq)
         self.verbose = verbose
 
         # Primary beam correction.
 
         self._pb_corrected = False
         if primary_beam is not None:
             self.correct_PB(primary_beam)
@@ -3095,43 +3098,58 @@
         factor = {'GHz': 1e9, 'MHz': 1e6, 'kHz': 1e3, 'Hz': 1e0}
         for key in ['GHz', 'MHz', 'kHz', 'Hz']:
             if key in string:
                 return float(string.replace(key, '')) * factor[key]
 
     # -- FITS I/O -- #
 
-    def _read_FITS(self, path):
-        """Reads the data from the FITS file."""
+    def _read_FITS(self, path, restfreq=None):
+        """
+        Reads the data from the FITS file.
+
+        Args:
+            path (str): Path to the FITS file to read the header.
+            restfreq (Optional[float]): A user-specified rest-frame frequency in
+                [Hz] that will override the one found in the header.
+        """
 
         # File names.
+
         self.path = os.path.expanduser(path)
         self.fname = self.path.split('/')[-1]
 
         # FITS data.
+
         self.header = fits.getheader(path)
         self.data = np.squeeze(fits.getdata(self.path))
         self.data = np.where(np.isfinite(self.data), self.data, 0.0)
         try:
             self.bunit = self.header['bunit']
         except KeyError:
             if self._user_bunit is not None:
                 self.bunit = self._user_bunit
             else:
                 print("WARNING: Not `bunit` header keyword found.")
                 self.bunit = input("\t Enter brightness unit: ")
 
         # Position axes.
+
         self.xaxis = self._readpositionaxis(a=1)
         self.yaxis = self._readpositionaxis(a=2)
         self.dpix = np.mean([abs(np.diff(self.xaxis))])
         self.nxpix = self.xaxis.size
         self.nypix = self.yaxis.size
 
         # Spectral axis.
-        self.nu0 = self._readrestfreq()
+
+        if restfreq is None:
+            self.nu0 = self._readrestfreq()
+        else:
+            self.nu0 = restfreq
+
         try:
             self.velax = self._readvelocityaxis()
             if self.velax.size > 1:
                 self.chan = np.mean(np.diff(self.velax))
             else:
                 self.chan = np.nan
             self.freqax = self._readfrequencyaxis()
@@ -3147,19 +3165,21 @@
         try:
             self.channels = np.arange(self.velax.size)
         except AttributeError:
             self.channels = [0]
 
         # Check that the data is saved such that increasing indices in x are
         # decreasing in offset counter to the yaxis.
+
         if np.diff(self.xaxis).mean() > 0.0:
             self.xaxis = self.xaxis[::-1]
             self.data = self.data[:, ::-1]
 
         # Beam.
+
         self._read_beam()
 
     def _read_beam(self):
         """Reads the beam properties from the header."""
         try:
             if self.header.get('CASAMBM', False):
                 beam = fits.open(self.path)[1].data
@@ -3271,15 +3291,18 @@
             else:
                 a_del = 1.0 * self._user_pixel_scale
             a_pix = a_len / 2.0 + 0.5
         axis = 3600.0 * a_del * (np.arange(a_len) - 0.5 * (a_len - 1.0))
         return axis
 
     def _readrestfreq(self):
-        """Read the rest frequency."""
+        """
+        Read the rest frequency. If no rest frequency header value is found, it
+        will adopt the frequency used for defining the spectral axis.
+        """
         try:
             nu = self.header['restfreq']
         except KeyError:
             try:
                 nu = self.header['restfrq']
             except KeyError:
                 try:
@@ -3504,14 +3527,69 @@
         return self.estimate_RMS(N=5)
 
     @property
     def extent(self):
         """Cube field of view for use with Matplotlib's ``imshow``."""
         return [self.xaxis[0], self.xaxis[-1], self.yaxis[0], self.yaxis[-1]]
 
+    def remove_hot_pixels(self, npix=2, nsigma=1.0, niter=1, replace=True):
+        """
+        Remove hot pixels from the data. Hot pixels are identified by deviating
+        from the mean of the region +\- `npix` by an amount of at least `nsigma` 
+        times the standard deviation of the region. These hot pixels are
+        replaced by interpolated (using a box kernel convolution) values.
+
+        Args:
+            npix (Optional[int]): The number of pixels from the pixel of
+                interest to consider part of the region.
+            nsigma (Optional[float]): The threshold for considering a pixel a
+                'hot' pixel. Smaller values identify more hot pixels.
+            niter (Optional[int]): How many times to repeat this smoothing. Note
+                that with `niter > 1` some features may be washed out.
+            replace (Optional[bool]): If `True`, replace the attached dataset,
+                otherwise, return as an array.
+
+        Returns:
+            corrected_data (array): The correced data if `replace=False`.
+        """
+        from astropy.convolution import convolve, Box2DKernel
+
+        if self.data.ndim != 2:
+            raise NotImplementedError("Can only smooth 2D images.")
+
+        data_tmp = self.data.copy()
+
+        for _ in range(niter):
+        
+            # Cycle through each pixel and identify the hot pixels.
+
+            coldpix = np.ones(data_tmp.shape) * np.nan
+            for xi in np.arange(npix, self.nxpix - npix):
+                for yi in np.arange(npix, self.nypix - npix):
+                    point = data_tmp[yi, xi]
+                    region = data_tmp[yi-npix:yi+npix+1, xi-npix:xi+npix+1]
+                    region_mu = np.nanmean(region)
+                    region_std = np.nanstd(region)
+                    if abs(point - region_mu) < (nsigma * region_std):
+                        coldpix[yi, xi] = point
+                        
+            # Convolve, interpolating the NaN value, and re-mask based on the
+            # old data. 
+            
+            hotpix = np.logical_and(np.isfinite(self.data), np.isnan(coldpix))
+            coldpix = convolve(coldpix, Box2DKernel(2*npix+1))
+            data_tmp = np.where(hotpix, coldpix, data_tmp)
+        
+        # Either replace the attached data or return as an array.
+
+        if not replace:
+            return data_tmp
+        self.data = data_tmp
+        self.mask = np.isfinite(self.data)
+
     def get_spectrum(self, coords, x0=0.0, y0=0.0, inc=0.0, PA=0.0,
                      frame='sky', coord_type='cartesian', area=0.0,
                      beam_weighting=False, return_mask=False):
         """
         Return a spectrum at a position defined by a coordinates given either
         in sky-frame position (``frame='sky'``) or a disk-frame location
         (``frame='disk'``). The coordinates can be either in cartesian or
@@ -3925,15 +4003,15 @@
                                   r_cavity=r_cavity, r_taper=r_taper,
                                   q_taper=q_taper, z_func=z_func, mstar=mstar,
                                   dist=dist, resample=resample,
                                   beam_spacing=beam_spacing, r_min=r_min,
                                   r_max=r_max, PA_min=PA_min, PA_max=PA_max,
                                   exclude_PA=exclude_PA, abs_PA=abs_PA,
                                   mask_frame=mask_frame, mask=mask, unit=unit,
-                                  shadowed=shadowe, vrad_func=vrad_func)
+                                  shadowed=shadowed, vrad_func=vrad_func)
         rvals, velax, spectra, scatter = out
 
         # Generate the axes.
         if ax is None:
             fig, ax = plt.subplots()
 
         # Plot the figure.
```

### Comparing `gofish-1.6.4/setup.py` & `gofish-1.6.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="gofish",
-    version="1.6.4",
+    version="1.6.6",
     author="Richard Teague",
     author_email="rteague@mit.edu",
     description="Fishing for molecular line emission in protoplanetary disks.",
     url="https://github.com/richteague/gofish",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

