# Comparing `tmp/curie-0.0.8.tar.gz` & `tmp/curie-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/curie-0.0.8.tar", last modified: Wed Aug 19 22:38:44 2020, max compression
+gzip compressed data, was "dist/curie-0.0.9.tar", last modified: Mon Nov 16 22:46:21 2020, max compression
```

## Comparing `curie-0.0.8.tar` & `curie-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jmorrell  (1000) jmorrell  (1000)        0 2020-08-19 22:38:44.000000 curie-0.0.8/
--rw-r--r--   0 jmorrell  (1000) jmorrell  (1000)     2433 2020-08-19 22:38:44.000000 curie-0.0.8/PKG-INFO
--rwxrwxrwx   0 jmorrell  (1000) jmorrell  (1000)     1784 2020-04-18 20:18:14.000000 curie-0.0.8/README.md
--rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)       33 2018-09-03 21:07:30.000000 curie-0.0.8/MANIFEST.in
--rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)     1073 2018-06-13 00:23:48.000000 curie-0.0.8/LICENSE
--rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)     1971 2020-08-19 22:37:52.000000 curie-0.0.8/setup.py
--rw-r--r--   0 jmorrell  (1000) jmorrell  (1000)       38 2020-08-19 22:38:44.000000 curie-0.0.8/setup.cfg
-drwxr-xr-x   0 jmorrell  (1000) jmorrell  (1000)        0 2020-08-19 22:38:44.000000 curie-0.0.8/curie/
--rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)    24220 2020-08-19 22:36:54.000000 curie-0.0.8/curie/decay_chain.py
--rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)    17923 2020-04-18 22:34:18.000000 curie-0.0.8/curie/stack.py
--rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)     4600 2020-03-24 21:15:30.000000 curie-0.0.8/curie/data.py
--rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)     9966 2020-04-20 21:55:27.000000 curie-0.0.8/curie/reaction.py
--rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)    46064 2020-08-05 21:49:03.000000 curie-0.0.8/curie/spectrum.py
--rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)    22597 2020-04-18 22:31:54.000000 curie-0.0.8/curie/compound.py
--rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)     1492 2020-08-19 22:37:39.000000 curie-0.0.8/curie/__init__.py
--rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)     9478 2020-04-18 22:30:19.000000 curie-0.0.8/curie/plotting.py
--rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)    23416 2020-06-04 21:42:25.000000 curie-0.0.8/curie/isotope.py
--rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)     9211 2020-03-29 22:45:41.000000 curie-0.0.8/curie/library.py
--rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)    18254 2020-03-29 20:37:12.000000 curie-0.0.8/curie/element.py
--rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)    28443 2020-06-02 19:31:47.000000 curie-0.0.8/curie/calibration.py
-drwxr-xr-x   0 jmorrell  (1000) jmorrell  (1000)        0 2020-08-19 22:38:44.000000 curie-0.0.8/curie.egg-info/
--rw-r--r--   0 jmorrell  (1000) jmorrell  (1000)     2433 2020-08-19 22:38:43.000000 curie-0.0.8/curie.egg-info/PKG-INFO
--rw-r--r--   0 jmorrell  (1000) jmorrell  (1000)      366 2020-08-19 22:38:43.000000 curie-0.0.8/curie.egg-info/SOURCES.txt
--rw-r--r--   0 jmorrell  (1000) jmorrell  (1000)        1 2020-08-19 22:38:43.000000 curie-0.0.8/curie.egg-info/dependency_links.txt
--rw-r--r--   0 jmorrell  (1000) jmorrell  (1000)        6 2020-08-19 22:38:43.000000 curie-0.0.8/curie.egg-info/top_level.txt
+drwxr-xr-x   0 jmorrell  (1000) jmorrell  (1000)        0 2020-11-16 22:46:21.000000 curie-0.0.9/
+-rw-r--r--   0 jmorrell  (1000) jmorrell  (1000)     2433 2020-11-16 22:46:21.000000 curie-0.0.9/PKG-INFO
+-rwxrwxrwx   0 jmorrell  (1000) jmorrell  (1000)     1784 2020-04-18 20:18:14.000000 curie-0.0.9/README.md
+-rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)       33 2018-09-03 21:07:30.000000 curie-0.0.9/MANIFEST.in
+-rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)     1073 2018-06-13 00:23:48.000000 curie-0.0.9/LICENSE
+-rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)     1971 2020-11-16 22:42:41.000000 curie-0.0.9/setup.py
+-rw-r--r--   0 jmorrell  (1000) jmorrell  (1000)       38 2020-11-16 22:46:21.000000 curie-0.0.9/setup.cfg
+drwxr-xr-x   0 jmorrell  (1000) jmorrell  (1000)        0 2020-11-16 22:46:21.000000 curie-0.0.9/curie/
+-rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)    24243 2020-10-23 21:49:59.000000 curie-0.0.9/curie/decay_chain.py
+-rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)    17923 2020-04-18 22:34:18.000000 curie-0.0.9/curie/stack.py
+-rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)     4600 2020-03-24 21:15:30.000000 curie-0.0.9/curie/data.py
+-rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)     9966 2020-04-20 21:55:27.000000 curie-0.0.9/curie/reaction.py
+-rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)    46043 2020-10-21 19:51:02.000000 curie-0.0.9/curie/spectrum.py
+-rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)    22597 2020-04-18 22:31:54.000000 curie-0.0.9/curie/compound.py
+-rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)     1492 2020-11-16 22:42:54.000000 curie-0.0.9/curie/__init__.py
+-rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)     9478 2020-04-18 22:30:19.000000 curie-0.0.9/curie/plotting.py
+-rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)    23416 2020-06-04 21:42:25.000000 curie-0.0.9/curie/isotope.py
+-rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)     9211 2020-03-29 22:45:41.000000 curie-0.0.9/curie/library.py
+-rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)    18254 2020-03-29 20:37:12.000000 curie-0.0.9/curie/element.py
+-rw-rw-r--   0 jmorrell  (1000) jmorrell  (1000)    28444 2020-10-21 22:41:58.000000 curie-0.0.9/curie/calibration.py
+drwxr-xr-x   0 jmorrell  (1000) jmorrell  (1000)        0 2020-11-16 22:46:21.000000 curie-0.0.9/curie.egg-info/
+-rw-r--r--   0 jmorrell  (1000) jmorrell  (1000)     2433 2020-11-16 22:46:21.000000 curie-0.0.9/curie.egg-info/PKG-INFO
+-rw-r--r--   0 jmorrell  (1000) jmorrell  (1000)      366 2020-11-16 22:46:21.000000 curie-0.0.9/curie.egg-info/SOURCES.txt
+-rw-r--r--   0 jmorrell  (1000) jmorrell  (1000)        1 2020-11-16 22:46:21.000000 curie-0.0.9/curie.egg-info/dependency_links.txt
+-rw-r--r--   0 jmorrell  (1000) jmorrell  (1000)        6 2020-11-16 22:46:21.000000 curie-0.0.9/curie.egg-info/top_level.txt
```

### Comparing `curie-0.0.8/PKG-INFO` & `curie-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curie
-Version: 0.0.8
+Version: 0.0.9
 Summary: Curie is a python toolkit to aid in the analysis of experimental nuclear data.
 Home-page: https://github.com/jtmorrell/curie
 Author: Jonathan Morrell
 Author-email: jmorrell@berkeley.edu
 License: MIT
 Description: # Curie
```

### Comparing `curie-0.0.8/README.md` & `curie-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `curie-0.0.8/LICENSE` & `curie-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `curie-0.0.8/setup.py` & `curie-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 		_install.run(self)
 		self.execute(_post_install, (self.install_lib,), msg="Downloading nuclear data files...")
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='curie',
-	  version='0.0.8',
+	  version='0.0.9',
 	  description='Curie is a python toolkit to aid in the analysis of experimental nuclear data.',
 	  long_description=long_description,
 	  long_description_content_type="text/markdown",
 	  url='https://github.com/jtmorrell/curie',
 	  author='Jonathan Morrell',
 	  author_email='jmorrell@berkeley.edu',
 	  license='MIT',
```

### Comparing `curie-0.0.8/curie/decay_chain.py` & `curie-0.0.9/curie/decay_chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -489,16 +489,16 @@
 
 				df['isotope'] = [self._filter_name(i) for i in df['isotope']]
 				df = df[df['isotope'].isin(self.isotopes)]
 
 				if len(df):
 					start = (sp.start_time-EoB).total_seconds()*self._r_lm('s')
 					stop = start+(sp.real_time*self._r_lm('s'))
-
-			counts.append(pd.DataFrame({'isotope':df['isotope'], 'start':start, 'stop':stop, 'counts':df['decays'], 'unc_counts':df['unc_decays']}))
+			if len(df):
+				counts.append(pd.DataFrame({'isotope':df['isotope'], 'start':start, 'stop':stop, 'counts':df['decays'], 'unc_counts':df['unc_decays']}))
 
 		self.counts = pd.concat(counts, sort=True, ignore_index=True).sort_values(by=['start']).reset_index(drop=True)
 
 
 	@property	
 	def R_avg(self):
 		df = []
@@ -634,29 +634,29 @@
 			self.A0[ip] *= fit[n]
 
 		self.counts = self.counts
 
 		A_norm = np.array([self.A0[i] for i in A0_isotopes])
 		return A0_isotopes, A_norm, cov*(A_norm/fit)**2
 		
-	def plot(self, time=None, max_plot=None, max_label=10, **kwargs):
+	def plot(self, time=None, max_plot=10, max_label=10, **kwargs):
 		"""Plot the activities in the decay chain
 
 		Plots the activities as a function of time for all radioactive
 		isotopes in the decay chain.  Can plot along a specified time
 		grid, else the time will be inferred from the half-life of the
 		parent isotope, or any count information given to self.counts.
 
 		Parameters
 		----------
 		time : array_like, optional
 			Time grid along which to plot.  Units must be the same as the decay chain.
 
 		max_plot : int, optional
-			Maximum number of isotope activities to plot in the decay chain. Default, None.
+			Maximum number of isotope activities to plot in the decay chain. Default, 10.
 
 		max_label : int, optional
 			Maximum number of isotope activities to label in the legend. Default, 10.
 
 		Other Parameters
 		----------------
 		**kwargs
@@ -719,20 +719,20 @@
 				label = Isotope(istp).TeX if n<max_label else None
 				line, = ax.plot(plot_time, A*mult, label=label)
 
 				if self.counts is not None:
 					df = self.counts[self.counts['isotope']==istp]
 					if len(df):
 						x, y, yerr = df['start'].to_numpy(), df['activity'].to_numpy(), df['unc_activity'].to_numpy()
-						idx = np.where((0.4*y>yerr)&(yerr>0.0)&(np.isfinite(yerr)))
-						if len(x[idx]>0):
-							x, y, yerr = x[idx], y[idx], yerr[idx]
-						idx = np.where((self.activity(istp, x)-y)**2/yerr**2<10.0)
-						if len(x[idx]>0):
-							x, y, yerr = x[idx], y[idx], yerr[idx]
+						# idx = np.where((0.4*y>yerr)&(yerr>0.0)&(np.isfinite(yerr)))
+						# if len(x[idx]>0):
+						# 	x, y, yerr = x[idx], y[idx], yerr[idx]
+						# idx = np.where((self.activity(istp, x)-y)**2/yerr**2<10.0)
+						# if len(x[idx]>0):
+						# 	x, y, yerr = x[idx], y[idx], yerr[idx]
 					
 						ax.errorbar(x, y*mult, yerr=yerr*mult, ls='None', marker='o', color=line.get_color(), label=None)
 
 
 
 		ax.set_xlabel('Time ({})'.format(self.units))
 		ax.set_ylabel('Activity ({}Bq)'.format(lb_or))
```

### Comparing `curie-0.0.8/curie/stack.py` & `curie-0.0.9/curie/stack.py`

 * *Files identical despite different names*

### Comparing `curie-0.0.8/curie/data.py` & `curie-0.0.9/curie/data.py`

 * *Files identical despite different names*

### Comparing `curie-0.0.8/curie/reaction.py` & `curie-0.0.9/curie/reaction.py`

 * *Files identical despite different names*

### Comparing `curie-0.0.8/curie/spectrum.py` & `curie-0.0.9/curie/spectrum.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 	>>> sp.cb = 'example_calib.json'
 	>>> sp.fit_config = {'bg':'quadratic', 'xrays':False}
 	>>> sp.saveas('eu_calib_7cm.Chn')
 	>>> sp = ci.Spectrum('eu_calib_7cm.Chn')
 
 	"""
 
-	def __init__(self, filename, **kwargs):
+	def __init__(self, filename=None, **kwargs):
 		self.filename = filename
 		if 'cb' in kwargs:
 			if type(kwargs['cb']==str):
 				self._cb = Calibration(kwargs['cb'])
 			else:
 				self._cb = copy.deepcopy(kwargs['cb'])
 		else:
@@ -103,14 +103,15 @@
 							'step':0.00, 'bg':'snip', 'skew_fit':False,
 							'step_fit':False, 'SNR_min':4.0, 'A_bound':1.0,
 							'mu_bound':1.0, 'sig_bound':1.0, 'xrays':False,
 							'pk_width':7.5, 'E_min':75.0, 'I_min':0.05,
 							'dE_511':3.5, 'multi_max':8}
 		if 'fit_config' in kwargs:
 			self.fit_config = kwargs['fit_config']
+		self._ortec_metadata = {}
 
 		if filename is not None:
 			if os.path.exists(filename):
 				print('Reading Spectrum {}'.format(filename))
 				if filename.endswith('.Spe'):
 					self._read_Spe(filename)
 				elif filename.endswith('.Chn'):
@@ -122,23 +123,24 @@
 			else:
 				raise ValueError('File does not exist: {}'.format(filename))
 
 		if 'isotopes' in kwargs:
 			self.isotopes = kwargs['isotopes']
 		else:
 			self.isotopes = []
+
 		self._peaks = None
 		self._fits = None
 		self._geom_corr = 1.0
 		self._atten_corr = None
 
 		self._gmls = None
 
+
 	def _read_Spe(self, filename):
-		self._ortec_metadata = {}
 
 		with open(filename) as f:
 			ln = f.readline()
 			while ln:
 				if ln.startswith('$'):
 					section = ln.strip()[1:-1]
 					if section=='DATA':
@@ -152,15 +154,14 @@
 
 		self.start_time = dtm.datetime.strptime(self._ortec_metadata['DATE_MEA'][0], '%m/%d/%Y %H:%M:%S')
 		self.live_time, self.real_time = tuple(map(float, self._ortec_metadata['MEAS_TIM'][0].split()))
 
 		self.cb.engcal = list(map(float, self._ortec_metadata['MCA_CAL'][-1].split(' ')[:-1]))
 
 	def _read_Chn(self, filename):
-		self._ortec_metadata = {}
 
 		with open(filename, 'rb') as f:
 			det_no = np.frombuffer(f.read(6), dtype='i2')[1]
 			sts = np.frombuffer(f.read(2), dtype='S2')[0].decode('utf-8')
 
 			self.real_time, self.live_time = tuple(map(float, 0.02*np.frombuffer(f.read(8), dtype='i4')))
```

### Comparing `curie-0.0.8/curie/compound.py` & `curie-0.0.9/curie/compound.py`

 * *Files identical despite different names*

### Comparing `curie-0.0.8/curie/__init__.py` & `curie-0.0.9/curie/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,12 +49,12 @@
 from .decay_chain import DecayChain
 
 from .library import Library
 from .reaction import Reaction
 
 from .stack import Stack
 
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 __all__ = ['download', 'colormap', 'set_style', 
           'Isotope', 'Element', 'Compound', 
           'Spectrum', 'Calibration', 'DecayChain', 
           'Library', 'Reaction', 'Stack']
```

### Comparing `curie-0.0.8/curie/plotting.py` & `curie-0.0.9/curie/plotting.py`

 * *Files identical despite different names*

### Comparing `curie-0.0.8/curie/isotope.py` & `curie-0.0.9/curie/isotope.py`

 * *Files identical despite different names*

### Comparing `curie-0.0.8/curie/library.py` & `curie-0.0.9/curie/library.py`

 * *Files identical despite different names*

### Comparing `curie-0.0.8/curie/element.py` & `curie-0.0.9/curie/element.py`

 * *Files identical despite different names*

### Comparing `curie-0.0.8/curie/calibration.py` & `curie-0.0.9/curie/calibration.py`

 * *Files 0% similar despite different names*

```diff
@@ -596,15 +596,15 @@
 		idx = np.where((0.33*y>yerr)&(yerr>0.0)&(np.isfinite(yerr)))
 		x, y, yerr = x[idx], y[idx], yerr[idx]
 		fn = lambda x, *A: self.eff(x, A)
 
 		p0 = spectra[0].cb.effcal
 		p0 = p0.tolist() if len(p0)==7 else p0.tolist()+[0.5, 0.001]
 		p0[0] = max([min([p0[0]*np.average(y/self.eff(x, p0), weights=(self.eff(x, p0)/yerr)**2),4.99]),0.0001])
-		bounds = ([0.0, 0.0, 0.1, 0.0, 0.0, 0.001, 1E-12], [5, 100, 5, 50, 5, 5, 0.1])
+		bounds = ([0.0, 0.0, 0.1, 0.0, 0.0, 0.001, 1E-12], [12, 100, 6, 50, 6, 6, 0.2])
 
 		if any([sp.fit_config['xrays'] for sp in spectra]):
 			try:
 				fit5, unc5 = curve_fit(fn, x, y, sigma=yerr, p0=p0[:5], bounds=(bounds[0][:5], bounds[1][:5]))
 				fit7, unc7 = curve_fit(fn, x, y, sigma=yerr, p0=fit5.tolist()+p0[5:], bounds=bounds)
 				
 				chi7 = np.sum((y-self.eff(x, fit7))**2/yerr**2)
```

### Comparing `curie-0.0.8/curie.egg-info/PKG-INFO` & `curie-0.0.9/curie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curie
-Version: 0.0.8
+Version: 0.0.9
 Summary: Curie is a python toolkit to aid in the analysis of experimental nuclear data.
 Home-page: https://github.com/jtmorrell/curie
 Author: Jonathan Morrell
 Author-email: jmorrell@berkeley.edu
 License: MIT
 Description: # Curie
```

