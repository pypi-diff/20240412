# Comparing `tmp/AlgDiff-2.3.tar.gz` & `tmp/AlgDiff-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlgDiff-2.3.tar", last modified: Fri Jan  5 12:34:26 2024, max compression
+gzip compressed data, was "AlgDiff-2.4.tar", last modified: Fri Apr 12 07:15:15 2024, max compression
```

## Comparing `AlgDiff-2.3.tar` & `AlgDiff-2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2024-01-05 12:34:26.713127 AlgDiff-2.3/
-drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2024-01-05 12:34:26.709127 AlgDiff-2.3/AlgDiff/
--rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)       68 2023-06-15 14:57:11.000000 AlgDiff-2.3/AlgDiff/__init__.py
--rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)    48758 2024-01-05 12:10:08.000000 AlgDiff-2.3/AlgDiff/algebraicDifferentiator.py
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)        0 2023-08-16 10:06:53.000000 AlgDiff-2.3/AlgDiff/test.py
-drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2024-01-05 12:34:26.713127 AlgDiff-2.3/AlgDiff.egg-info/
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)    15520 2024-01-05 12:34:26.000000 AlgDiff-2.3/AlgDiff.egg-info/PKG-INFO
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)      276 2024-01-05 12:34:26.000000 AlgDiff-2.3/AlgDiff.egg-info/SOURCES.txt
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)        1 2024-01-05 12:34:26.000000 AlgDiff-2.3/AlgDiff.egg-info/dependency_links.txt
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)       19 2024-01-05 12:34:26.000000 AlgDiff-2.3/AlgDiff.egg-info/requires.txt
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)        8 2024-01-05 12:34:26.000000 AlgDiff-2.3/AlgDiff.egg-info/top_level.txt
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)     1458 2024-01-03 15:04:25.000000 AlgDiff-2.3/LICENSE
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)    15520 2024-01-05 12:34:26.713127 AlgDiff-2.3/PKG-INFO
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)    13062 2023-08-28 08:54:04.000000 AlgDiff-2.3/README.md
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)      871 2024-01-05 12:10:08.000000 AlgDiff-2.3/pyproject.toml
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)       79 2024-01-05 12:34:26.713127 AlgDiff-2.3/setup.cfg
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)     1144 2024-01-05 12:10:08.000000 AlgDiff-2.3/setup.py
+drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2024-04-12 07:15:15.669779 AlgDiff-2.4/
+drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2024-04-12 07:15:15.661779 AlgDiff-2.4/AlgDiff/
+-rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)       68 2023-06-15 14:57:11.000000 AlgDiff-2.4/AlgDiff/__init__.py
+-rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)    53323 2024-04-12 07:08:45.000000 AlgDiff-2.4/AlgDiff/algebraicDifferentiator.py
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)        0 2023-08-16 10:06:53.000000 AlgDiff-2.4/AlgDiff/test.py
+drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2024-04-12 07:15:15.669779 AlgDiff-2.4/AlgDiff.egg-info/
+-rw-r--r--   0 aothmane  (1000) aothmane  (1000)    15584 2024-04-12 07:15:15.000000 AlgDiff-2.4/AlgDiff.egg-info/PKG-INFO
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)      276 2024-04-12 07:15:15.000000 AlgDiff-2.4/AlgDiff.egg-info/SOURCES.txt
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)        1 2024-04-12 07:15:15.000000 AlgDiff-2.4/AlgDiff.egg-info/dependency_links.txt
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)       19 2024-04-12 07:15:15.000000 AlgDiff-2.4/AlgDiff.egg-info/requires.txt
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)        8 2024-04-12 07:15:15.000000 AlgDiff-2.4/AlgDiff.egg-info/top_level.txt
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)     1458 2024-01-03 15:04:25.000000 AlgDiff-2.4/LICENSE
+-rw-r--r--   0 aothmane  (1000) aothmane  (1000)    15584 2024-04-12 07:15:15.669779 AlgDiff-2.4/PKG-INFO
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)    13062 2023-08-28 08:54:04.000000 AlgDiff-2.4/README.md
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)      871 2024-04-12 07:08:45.000000 AlgDiff-2.4/pyproject.toml
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)       79 2024-04-12 07:15:15.669779 AlgDiff-2.4/setup.cfg
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)     1144 2024-04-12 07:08:45.000000 AlgDiff-2.4/setup.py
```

### Comparing `AlgDiff-2.3/AlgDiff/algebraicDifferentiator.py` & `AlgDiff-2.4/AlgDiff/algebraicDifferentiator.py`

 * *Files 10% similar despite different names*

```diff
@@ -169,33 +169,33 @@
         :type der: int
         :param method: Discretization scheme: "mid-point", "trapezoidal",\
             "analytic", "simpson rule", and "analytic trapezoidal".
         :type method: string
         :param reduceFilLength: Reduce or not the filter window length.
         :type reduceFilLength: bool
         :param redTol: Tolerance to be used when the filter length is reduced.
-        :type redTol: float.
+        :type redTol: float
         :param discreteSpectrum: If it is set, then the parameter \
             :math:`\\theta` used in the discretization is returned. See survey paper
             for more details.
         :type discreteSpectrum: bool
         
         :returns:
         	- coeff (dictionary) - Discretized filter in a dict where the keys are the derivative \
             		for which a filter has been discretized. Each element is a dict. with \
             		keys the used discretization methods. If the correction of the DC \
             		component has been enabled with the parameter corr of the class \
             		initialization, this output contains the corrected filter coefficients.
-        	- tau_1 (:py:class:`float`) - If redFilLength is set, tau_1 is the time where the filter \
+        	- tau_1 (`float <https://docs.python.org/3/library/functions.html#float>`_) - If redFilLength is set, tau_1 is the time where the filter \
         		window is reduced \
             		before at the left side of the interval. The estimation delay is reduced by tau_1.
-        	- tau_2 (:py:class:`float`) - If redFilLength is set, tau_2 is the time where the filter \
+        	- tau_2 (`float <https://docs.python.org/3/library/functions.html#float>`_) - If redFilLength is set, tau_2 is the time where the filter \
         	 	window is reduced\
             		before at the right side of the interval. This value does not affect the delay.
-        	- theta (:py:class:`float`) - If discreteSpectrum is set then the parameter\
+        	- theta (`float <https://docs.python.org/3/library/functions.html#float>`_) - If discreteSpectrum is set then the parameter\
         		 :math:`\\theta` is also returned.
         """
         self.checkParameters(der)
         theta0 = 0
         theta = theta0
         L0 = int(self.__T/self.__ts)
         red = ""
@@ -485,21 +485,23 @@
                 return self.__w,theta
             else:
                 return self.__w
 
     def get_integralKernel(self,t,nested=1):
         """
         This function returns the nested integral of the kernel of the algebraic with 
-        respect to the time variable. The integration is performed from 0 to t.
+        respect to the time variable. The integration is performed from 0 to t. Raises
+        and error if the order of the nested integral is higher than 2.
 
         :param t: Time instants where the step response should be evaluated.
-        :type t: numpy array
-        :param t: order of nested integrals
-        :type t: numpy int
-        :return: The value of the integral
+        :type t: numpy.ndarray
+        :param nested: order of nested integrals
+        :type nested: int
+        :return: 
+            - The value of the integral (`float <https://docs.python.org/3/library/functions.html#float>`_) - The value of the integral.
         """
         a = self.__alpha
         b = self.__beta
         theta = self.__theta
         N = self.__N
         T = self.__T
         def get_cNK_ab(a,b,N,k):
@@ -538,29 +540,29 @@
         using the discretization method given. If the filter was not\
         discretized before the function performs the discretization.\
         See the method discretize for more details on the discretization.
 
         :param k: Order of the derivative to be estimated.
         :type k: int
         :param x: Signal whose derivative has to be estimated.
-        :type x: numpy array
+        :type x: `numpy.ndarray <https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html>`_
         :param conv: Parameter to specify the type of convolution
                 the numpy conv function does. See the numpy documentation
                 for more details.
         :param method: Discretization method: "mid-point",
                 "trapezoidal", "analytic"
 
-        :type method: string
-        :type conv: string
+        :type method: str
+        :type conv: str
         :param reduceFilterLength: Specify whether or not the filter window
                 length should be reduced or not. See the discretize method for more
                 details.
         :type reduceFilterLength: bool
         :param redTol: Tolerance to be used when the filter length is reduced
-        :type redTol: float.
+        :type redTol: float
         :return: Estimated derivative in a numpy array with the same dimensions
             as the variable x
         """
         red = ""
         if redFilLength:
             red = "-red"
 
@@ -582,85 +584,93 @@
             return np.concatenate((np.zeros((N,)),dx2[:-N]))
 
 
     def get_alpha(self):
         """
         This function returns the parameter :math:`\\alpha`.
 
-        :return: :math:`\\alpha` as a float.
+        :return:
+            - :math:`\\alpha` (`float <https://docs.python.org/3/library/functions.html#float>`_) - The parameter :math:`\\alpha`.
         """
 
         return self.__alpha
 
     def get_beta(self):
         """
         This function returns the parameter :math:`\\beta`.
         
-        :return: :math:`\\beta` as a float.
+        :returns:
+            - :math:`\\beta` (`float <https://docs.python.org/3/library/functions.html#float>`_) - The parameter :math:`\\beta`.
         """
 
         return self.__beta
     
     def get_N(self):
         """
         This function returns the parameter :math:`N`.
 
-        :return: :math:`N` as a float.
+        :return:
+            - :math:`N` (`float <https://docs.python.org/3/library/functions.html#float>`_) - The parameter :math:`N`.
         """
 
         return self.__N
     
     def get_theta(self):
         """
         This function returns the parameter :math:`\\vartheta`.
 
-        :return: :math:`\\vartheta` as a float.
+        :return:
+            - :math:`\\vartheta` (`float <https://docs.python.org/3/library/functions.html#float>`_) - The parameter :math:`\\vartheta`.
         """
 
         return self.__theta
     
     def get_ts(self):
         """
         This function returns the sampling period.
 
-        :return: Sampling period as a float.
+        :return:
+            - :math:`t_{s}` (`float <https://docs.python.org/3/library/functions.html#float>`_) - The sampling period :math:`t_{s}`.
         """
 
         return self.__ts
 
     def get_T(self):
         """
         This function returns the filter window length of the algebraic differentiator.
 
-        :return: Filter window length as a float.
+        :return:
+            - :math:`T` (`float <https://docs.python.org/3/library/functions.html#float>`_) - The filter window length  :math:`T`.
         """
 
         return self.__T
 
     def get_degreeExactness(self,n):
         """
         This function returns the degree of exactness :math:`\gamma`\
                 when the :math:`n`-th derivative is approximated.
 
-        :return: Degree of exactness as an integer.
+        :return:
+            - :math:`\gamma` (`int <https://docs.python.org/3/library/functions.html#int>`_) - The degree of exactness  :math:`\gamma`.
         """
 
         if (self.__N==0) or (self.__thetaBool):
             gamma = n+self.__N+1
         else:
             gamma = n+self.__N
 
         return gamma
 
     def get_cutoffFreq(self):
         """
         This function returns the cutoff frequency :math:`\omega_c`\
         of the algebraic differentiator.
 
-        :return: Cutoff frequency as a float.
+        :return:
+            - :math:`\omega_c` (`float <https://docs.python.org/3/library/functions.html#float>`_) - The cutoff frequency  :math:`\omega_c`.
         """
 
         a,b,c = self.get_asymptotesAmpFilter(np.array([1.0]))
 
         return self.__wc
 
     def timeShift(self,t):
@@ -707,16 +717,17 @@
 
     def get_stepResponse(self,t):
         """
         This function returns the step response of the differentiator \
         evaluated at the time instants in t.
 
         :param t: Time instants where the step response should be evaluated.
-        :type t: numpy array
-        :return: Evaluated step response in a numpy array.
+        :type t: numpy.ndarray
+        :return: 
+            - h (`numpy.ndarray <https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html>`_) - Evaluated step response
         """
         response = np.zeros(t.shape)
         a = self.__alpha + 1
         b = self.__beta + 1
         for it in range(len(t)):
             if t[it]<=0:
                 response[it] = 0
@@ -734,16 +745,17 @@
 
     def evalKernel(self,t):
         """
         This function evaluates the kernel of the algebraic differentiator at\
         times t. It corresponds to the impulse response of the filter. 
 
         :param t: Time instants where the kernel should be evaluated.
-        :type t: numpy array
-        :return: Evaluated kernel in a numpy array with same dimensions as t.
+        :type t: `numpy.ndarray <https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html>`_
+        :return: 
+            - g (`numpy.ndarray <https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html>`_) -  Evaluated kernel in a  with same dimensions as t.
         """
 
         a = self.__alpha
         b = self.__beta
         g = 0
         # Evaluate the filter kernel
         for i in range(self.__N+1):
@@ -907,17 +919,14 @@
     def computeTfromWc(self,wc):
         """
         This function computes the filter window length for a desired
         cutoff frequency.
 
         :param wc: Cutoff frequency.
         :type wc: float
-
-        :returns:
-        	- T (:py:class:`float`) -  filter window length
         """
 
         kappa = np.abs(self.__beta-self.__alpha)
         mu = 1+np.minimum(self.__beta,self.__alpha)
         if self.__beta>=self.__alpha:
             sigma = 1
         else:
@@ -943,15 +952,17 @@
 
 
     def get_delay(self):
         """
         This function returns the estimation delay :math:`\delta_t` of the\
         the algebraic differentiator. 
 
-        :return:  :math:`\delta_t` as a float 
+        :return:
+            - :math:`\delta_t` (`float <https://docs.python.org/3/library/functions.html#float>`_) -  The delay :math:`\delta_t`\
+                of the continuous time differentiator 
         """
         if self.__N==0:
             delay = (self.__alpha+1)/(self.__alpha+self.__beta+2)*self.__T
         else:
             delay = (1-self.__theta)/2*self.__T
         return delay
 
@@ -1101,17 +1112,18 @@
         print("Cutoff Frequency in Hz: %3.6f"%(self.get_cutoffFreq()/2/np.pi))
         print("Discrete window length: %d"%(int(self.__T/self.__ts)))
 
     def get_ratioNyquistCutoff(self,k):
         """This function computes the ratio
         :math:`k_N=20\\log_{10}\\left(\\frac{\omega_N^k\\big|\mathcal{G}(\omega_N)\\big|}{\omega_c^k\Big|\mathcal{G}(\omega_c)\Big|}\\right)`, with :math:`\omega_N=\pi/t_s`, the Nyquist frequency and :math:`\omega_c` the                cutoff frequency.
 
-        :param k: Orders of derivatives to be estimated.
-        :type k: list of natural numbers
-        :return:  :math:`k_N` in a numpy array with same dimensions as the
+        :param k: Orders of derivatives to be estimated. Must be a list of natural numbers.
+        :type k: list
+        :return:  
+            -:math:`k_N` (`numpy.ndarray <https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html>`_) - :math:`k_N` with same dimensions as the
             variable k 
         """
 
         wc = self.get_cutoffFreq()
         wN = np.pi/self.__ts
         G, tmp = self.get_ampAndPhaseFilter(np.array([wc,wN]))
 
@@ -1122,19 +1134,19 @@
         :math:`\\mathcal{J}=\\frac{\\int_{0}^{\\Omega}\\left|{\\mathcal{F}\\left\\{g^{(n)}-\\hat{g} ^{(n)}\\right\\}(\\omega)}\\right|^2\\mathrm{d}\\omega}
         {\\int_{0}^{\\Omega}\\left|{\\mathcal{F}\\left\\{g^{(n)}\\right\\}(\\omega)}\\right|^2\\mathrm{d}\\omega}`. 
         Therein :math:`g` and :math:`\\hat{g}` are the continuous and discrete time differentiators, respectively. 
         A reasonable choice for :math:`\\Omega_N` is the Nyquist frequency :math:`\\pi/t_s`. 
         The integral is approximated using the trapezoidal rule.
 
         :param k: Order of derivative to be estimated.
-        :type k: integer
+        :type k: int
         :param Omega: Upper bound of integration interval.
         :type Omega: float
         :param n: The interval :math:`[0,\\Omega]` is divided into n parts. 
-        :type n: integer
+        :type n: int
         :return:  cost function :math:`\\mathcal{J}`
         """
 
         omega = np.linspace(0,Omega,n)
         amp,phase = self.get_ampAndPhaseFilter(omega)
         F = amp*np.exp(1j*phase)*(1j*omega)**k
         ampDisc,phaseDisc = self.get_ampSpectrumDiscreteFilter(omega,k,\
@@ -1152,21 +1164,21 @@
         :param der: The sought derivative.
         :type der: int
         
         :param tol: The tolerance that for reducing the filter length
         :type tol: float
         
         :returns:
-        	- tau1 (:py:class:`float`) - New starting point of the window. The value 0, i.e., the old
+        	- tau1 (`float <https://docs.python.org/3/library/functions.html#float>`_) - New starting point of the window. The value 0, i.e., the old
             		starting point, is taken as the reference.
-        	- tau2 (:py:class:`float`) - New end point of the window. The value 0, i.e., the old starting
+        	- tau2 (`float <https://docs.python.org/3/library/functions.html#float>`_) - New end point of the window. The value 0, i.e., the old starting
            	 	point, is taken as the reference.
-        	- d (:py:class:`numpy array`) - Distribution function used for the truncation.
-        	- t (:py:class:`numpy array`) - Times instants where distribution function has been evaluated.
-        	- n (:py:class:`int`) - Factor relating the sampling rate of the measurements and the
+        	- d (`numpy.ndarray <https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html>`_) - Distribution function used for the truncation.
+        	- t (`numpy.ndarray <https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html>`_) - Times instants where distribution function has been evaluated.
+        	- n (`int <https://docs.python.org/3/library/functions.html#int>`_) - Factor relating the sampling rate of the measurements and the
 			    sampling rate used for the evaluation of the distribution
 			    function.
         """
         # Compute the first moment of the n-th derivative of the kernel
         n = 10
         t = np.arange(0,self.__T,self.__ts/n)
         g = self.evalKernelDer(t,der)
@@ -1177,7 +1189,69 @@
         np.array([np.trapz(np.abs(self.evalKernelDer(t[:i],der)),x=t[:i])\
                   for i in range(1,len(t)+1)])/m0
 
         # Find values where to reduce window length
         tau1 = np.argmax(disFcn>=tol)
         tau2 = np.argmax(disFcn>=1-disFcn[tau1])
         return t[tau1], t[tau2], disFcn, t, n
+    
+    def exportFilterCoefficients2Ccode(self,n,method='mid-point',filename='g',header='G'):
+        """
+        Export the filter coefficients to a C header file.
+
+        This method exports the filter coefficients computed by the AlgebraicDifferentiator 
+        object to a C header file. The filter coefficients are discretized using the specified 
+        method and written to a C array in the header file. The sampling period and the 
+        filter coefficients are hard coded. The user should not adjust the filter coefficients
+        in the header file. Instead, the filter coefficients should be adjusted in the
+        Python code and the header file should be regenerated.
+        For an algebraic differentiator with window length T=20*ts, with ts the sampling period, 
+        the function `exportFilterCoefficients2Ccode` generates for n=1 the following header file:
+
+        .. code-block:: c
+        
+            #ifndef G1_H
+            #define G1_H
+
+            #define WINDOW_LENGTH_G1 20
+            #define TS_AlgDiff 0.0100000000
+            
+            static const double g1[] = {
+                0.123456789012345678901234567890,
+                0.234567890123456789012345678901,
+                // More coefficients...
+            };
+
+            #endif // G1_H
+            
+        :param n: The filter length.
+        :type n: int
+        :param method: The discretization method. Defaults to 'mid-point'.
+        :type method: str, optional   
+        :param filename: The base name of the header file. Defaults to 'g'.
+        :type filename: str, optional
+        :param header: The prefix for the header guard. Defaults to 'G'.
+        :type header: str, optional
+        
+        Returns:
+            None
+
+        
+        """
+        g = self.discretize(n,method=method)[n][method]
+        with open(filename+str(n)+'.h', 'w') as f:
+            # Write the array declaration
+            f.write('// This file is automatically generated. Do not modify.\n'.upper())
+            f.write('#ifndef '+header+str(n)+'_H\n')
+            f.write('#define '+header+str(n)+'_H\n\n')
+            f.write('#define WINDOW_LENGTH_G'+str(n)+' '+str(len(g))+'\n')
+            f.write('#define TS_AlgDiff %.10f\n\n'%self.__ts)
+            f.write('static const double AlgDiff_g'+str(n)+'[] = {\n')
+
+            # Write the array values
+            for value in g:
+                f.write('    %.30f,\n' % value)  # Adjust the precision as needed
+
+            # Close the array declaration
+            f.write('};\n\n')
+            f.write('#endif // '+header+str(n)+'_H\n')
+
```

### Comparing `AlgDiff-2.3/AlgDiff.egg-info/PKG-INFO` & `AlgDiff-2.4/AlgDiff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: AlgDiff
-Version: 2.3
+Version: 2.4
 Summary: AlgDiff is a Python class implementing all necessary tools for the design, analysis, and discretization of algebraic differentiators. An interface to Matlab is also provided.
 Home-page: https://github.com/aothmane-control/Algebraic-differentiators
-Download-URL: https://github.com/aothmane-control/Algebraic-differentiators/releases/tag/v2.3
+Download-URL: https://github.com/aothmane-control/Algebraic-differentiators/releases/tag/v2.4
 Author: Amine Othmane
 Author-email: Amine Othmane <amine.othmane@uni-saarland.de>
 License: Copyright 2024 Amine Othmane
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
@@ -22,14 +22,17 @@
 Keywords: numerical-differentiation ,fir-filters,orthogonal-polynomials,numerical-methods 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: scipy
+Requires-Dist: mpmath
+Requires-Dist: numpy
 
 [![PyPI version](https://badge.fury.io/py/AlgDiff.svg)](https://badge.fury.io/py/AlgDiff)
 # AlgDiff
 AlgDiff: A Python class that provides all necessary tools for the design, analysis, and discretization of algebraic differentiators. An interface to Matlab is also provided.
 This implementation was released as part of the survey [[1]](#1).  A tutorial for algebraic differentiators and this package can be found in [[6]](#6).
 
 The toolbox is licensed under the BSD-3-Clause License, which is suitable for both academic and industrial/commercial purposes.
```

### Comparing `AlgDiff-2.3/LICENSE` & `AlgDiff-2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `AlgDiff-2.3/PKG-INFO` & `AlgDiff-2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: AlgDiff
-Version: 2.3
+Version: 2.4
 Summary: AlgDiff is a Python class implementing all necessary tools for the design, analysis, and discretization of algebraic differentiators. An interface to Matlab is also provided.
 Home-page: https://github.com/aothmane-control/Algebraic-differentiators
-Download-URL: https://github.com/aothmane-control/Algebraic-differentiators/releases/tag/v2.3
+Download-URL: https://github.com/aothmane-control/Algebraic-differentiators/releases/tag/v2.4
 Author: Amine Othmane
 Author-email: Amine Othmane <amine.othmane@uni-saarland.de>
 License: Copyright 2024 Amine Othmane
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
@@ -22,14 +22,17 @@
 Keywords: numerical-differentiation ,fir-filters,orthogonal-polynomials,numerical-methods 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: scipy
+Requires-Dist: mpmath
+Requires-Dist: numpy
 
 [![PyPI version](https://badge.fury.io/py/AlgDiff.svg)](https://badge.fury.io/py/AlgDiff)
 # AlgDiff
 AlgDiff: A Python class that provides all necessary tools for the design, analysis, and discretization of algebraic differentiators. An interface to Matlab is also provided.
 This implementation was released as part of the survey [[1]](#1).  A tutorial for algebraic differentiators and this package can be found in [[6]](#6).
 
 The toolbox is licensed under the BSD-3-Clause License, which is suitable for both academic and industrial/commercial purposes.
```

### Comparing `AlgDiff-2.3/README.md` & `AlgDiff-2.4/README.md`

 * *Files identical despite different names*

### Comparing `AlgDiff-2.3/pyproject.toml` & `AlgDiff-2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "AlgDiff"
-version = "2.3"
+version = "2.4"
 authors = [
   { name="Amine Othmane", email="amine.othmane@uni-saarland.de" },
 ]
 description = "AlgDiff is a Python class implementing all necessary tools for the design, analysis, and discretization of algebraic differentiators. An interface to Matlab is also provided."
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `AlgDiff-2.3/setup.py` & `AlgDiff-2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "docs/source/usage.rst").read_text()
 
 setup(
   name = 'AlgDiff',
   packages = ['AlgDiff'],
-  version = '2.3',
+  version = '2.4',
   license='bsd-3-clause',
   description = 'AlgDiff is a Python class implementing all necessary tools for the design, analysis, and discretization of algebraic differentiators. An interface to Matlab is also provided.',
   
   long_description = long_description,
   long_description_content_type='text/x-rst',
   
   author = 'Amine Othmane',
   author_email = 'amine.othmane@uni-saarland.de',
   url = 'https://github.com/aothmane-control/Algebraic-differentiators',
-  download_url = 'https://github.com/aothmane-control/Algebraic-differentiators/releases/tag/v2.3',
+  download_url = 'https://github.com/aothmane-control/Algebraic-differentiators/releases/tag/v2.4',
   keywords = ['numerical-differentiation ', 'fir-filters', 'orthogonal-polynomials', 'numerical-methods '],
   install_requires=[
           'scipy',
           'mpmath',
           'numpy',
           'sphinx_rtd_theme'
       ],
```

