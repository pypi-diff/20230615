# Comparing `tmp/psapy-0.4.tar.gz` & `tmp/psapy-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\psapy-0.4.tar", last modified: Sat Aug 22 15:37:06 2020, max compression
+gzip compressed data, was "psapy-0.5.tar", last modified: Thu Jun 15 01:18:19 2023, max compression
```

## Comparing `psapy-0.4.tar` & `psapy-0.5.tar`

### file list

```diff
@@ -1,17 +1,25 @@
-drwxrwxrwx   0        0        0        0 2020-08-22 15:37:06.763791 psapy-0.4/
--rw-rw-rw-   0        0        0      915 2020-08-22 15:37:06.763791 psapy-0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2020-08-22 15:37:06.763791 psapy-0.4/psapy/
--rw-rw-rw-   0        0        0     1738 2020-06-25 22:03:48.352846 psapy-0.4/psapy/BHPExample.py
--rw-rw-rw-   0        0        0    16033 2020-08-07 17:48:56.082791 psapy-0.4/psapy/BeggsandBrill.py
--rw-rw-rw-   0        0        0     1129 2017-11-24 13:52:29.000000 psapy-0.4/psapy/DB_Example.py
--rw-rw-rw-   0        0        0    10099 2017-12-12 01:27:14.000000 psapy-0.4/psapy/FluidProps.py
--rw-rw-rw-   0        0        0     1591 2017-11-12 16:02:14.000000 psapy-0.4/psapy/GasProp.py
--rw-rw-rw-   0        0        0     9548 2020-06-25 22:00:16.322438 psapy-0.4/psapy/Hagendornandbrown.py
--rw-rw-rw-   0        0        0     5821 2020-06-27 04:08:15.405439 psapy-0.4/psapy/OilProps.py
--rw-rw-rw-   0        0        0     2549 2017-12-12 01:20:58.000000 psapy-0.4/psapy/Solving_Intersections.py
--rw-rw-rw-   0        0        0     2227 2020-08-22 15:35:11.809446 psapy-0.4/psapy/Vogel.py
--rw-rw-rw-   0        0        0     2645 2017-11-12 16:44:09.000000 psapy-0.4/psapy/WaterProps.py
--rw-rw-rw-   0        0        0        0 2020-06-27 05:24:22.558153 psapy-0.4/psapy/__init__.py
--rw-rw-rw-   0        0        0       34 2017-11-11 13:39:54.000000 psapy-0.4/psapy/test.py
--rw-rw-rw-   0        0        0       40 2020-08-06 13:40:43.753504 psapy-0.4/setup.cfg
--rw-rw-rw-   0        0        0     1077 2020-08-22 15:36:39.536796 psapy-0.4/setup.py
+drwxr-xr-x   0 alejandroprimeranavarro   (501) staff       (20)        0 2023-06-15 01:18:19.841324 psapy-0.5/
+-rw-r--r--   0 alejandroprimeranavarro   (501) staff       (20)     1063 2023-06-15 01:11:57.000000 psapy-0.5/LICENSE.txt
+-rw-r--r--   0 alejandroprimeranavarro   (501) staff       (20)      908 2023-06-15 01:18:19.841379 psapy-0.5/PKG-INFO
+-rw-r--r--   0 alejandroprimeranavarro   (501) staff       (20)       52 2023-06-15 01:11:57.000000 psapy-0.5/README.md
+drwxr-xr-x   0 alejandroprimeranavarro   (501) staff       (20)        0 2023-06-15 01:18:19.840601 psapy-0.5/psapy/
+-rw-r--r--   0 alejandroprimeranavarro   (501) staff       (20)     1738 2023-06-15 01:11:57.000000 psapy-0.5/psapy/BHPExample.py
+-rw-r--r--   0 alejandroprimeranavarro   (501) staff       (20)    16033 2023-06-15 01:11:57.000000 psapy-0.5/psapy/BeggsandBrill.py
+-rw-r--r--   0 alejandroprimeranavarro   (501) staff       (20)     1129 2023-06-15 01:11:57.000000 psapy-0.5/psapy/DB_Example.py
+-rw-r--r--   0 alejandroprimeranavarro   (501) staff       (20)    10099 2023-06-15 01:11:57.000000 psapy-0.5/psapy/FluidProps.py
+-rw-r--r--   0 alejandroprimeranavarro   (501) staff       (20)     1591 2023-06-15 01:11:57.000000 psapy-0.5/psapy/GasProp.py
+-rw-r--r--   0 alejandroprimeranavarro   (501) staff       (20)     9333 2023-06-15 01:11:57.000000 psapy-0.5/psapy/Hagendornandbrown.py
+-rw-r--r--   0 alejandroprimeranavarro   (501) staff       (20)     5821 2023-06-15 01:11:57.000000 psapy-0.5/psapy/OilProps.py
+-rw-r--r--   0 alejandroprimeranavarro   (501) staff       (20)     2549 2023-06-15 01:11:57.000000 psapy-0.5/psapy/Solving_Intersections.py
+-rw-r--r--   0 alejandroprimeranavarro   (501) staff       (20)     2227 2023-06-15 01:18:00.000000 psapy-0.5/psapy/Vogel.py
+-rw-r--r--   0 alejandroprimeranavarro   (501) staff       (20)     2645 2023-06-15 01:11:57.000000 psapy-0.5/psapy/WaterProps.py
+-rw-r--r--   0 alejandroprimeranavarro   (501) staff       (20)        0 2023-06-15 01:11:57.000000 psapy-0.5/psapy/__init__.py
+-rw-r--r--   0 alejandroprimeranavarro   (501) staff       (20)       34 2023-06-15 01:11:57.000000 psapy-0.5/psapy/test.py
+drwxr-xr-x   0 alejandroprimeranavarro   (501) staff       (20)        0 2023-06-15 01:18:19.841193 psapy-0.5/psapy.egg-info/
+-rw-r--r--   0 alejandroprimeranavarro   (501) staff       (20)      908 2023-06-15 01:18:19.000000 psapy-0.5/psapy.egg-info/PKG-INFO
+-rw-r--r--   0 alejandroprimeranavarro   (501) staff       (20)      427 2023-06-15 01:18:19.000000 psapy-0.5/psapy.egg-info/SOURCES.txt
+-rw-r--r--   0 alejandroprimeranavarro   (501) staff       (20)        1 2023-06-15 01:18:19.000000 psapy-0.5/psapy.egg-info/dependency_links.txt
+-rw-r--r--   0 alejandroprimeranavarro   (501) staff       (20)       27 2023-06-15 01:18:19.000000 psapy-0.5/psapy.egg-info/requires.txt
+-rw-r--r--   0 alejandroprimeranavarro   (501) staff       (20)        6 2023-06-15 01:18:19.000000 psapy-0.5/psapy.egg-info/top_level.txt
+-rw-r--r--   0 alejandroprimeranavarro   (501) staff       (20)       79 2023-06-15 01:18:19.841638 psapy-0.5/setup.cfg
+-rw-r--r--   0 alejandroprimeranavarro   (501) staff       (20)     1047 2023-06-15 01:18:12.000000 psapy-0.5/setup.py
```

### Comparing `psapy-0.4/PKG-INFO` & `psapy-0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-Metadata-Version: 1.1
-Name: psapy
-Version: 0.4
-Summary: Production System Analysis
-Home-page: https://github.com/orkahub/production_systems_analysis
-Author: Orkahub Energy
-Author-email: orkahub@gmail.com
-License: MIT
-Download-URL: https://github.com/orkahub/production_systems_analysis/archive/v_04.tar.gz
-Description: UNKNOWN
-Keywords: RESERVOIR,ENERGY,OIL,GAS,PRODUCTION,VLP,IPR
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Metadata-Version: 2.1
+Name: psapy
+Version: 0.5
+Summary: Production System Analysis
+Home-page: https://github.com/orkahub/production_systems_analysis
+Author: Orkahub Energy
+Author-email: orkahub@gmail.com
+License: MIT
+Download-URL: https://github.com/orkahub/production_systems_analysis/archive/v_03.tar.gz
+Keywords: RESERVOIR,ENERGY,OIL,GAS,PRODUCTION,VLP,IPR
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+License-File: LICENSE.txt
+
+UNKNOWN
+
```

### Comparing `psapy-0.4/psapy/BHPExample.py` & `psapy-0.5/psapy/BHPExample.py`

 * *Files identical despite different names*

### Comparing `psapy-0.4/psapy/BeggsandBrill.py` & `psapy-0.5/psapy/BeggsandBrill.py`

 * *Files identical despite different names*

### Comparing `psapy-0.4/psapy/DB_Example.py` & `psapy-0.5/psapy/DB_Example.py`

 * *Files identical despite different names*

### Comparing `psapy-0.4/psapy/FluidProps.py` & `psapy-0.5/psapy/FluidProps.py`

 * *Files identical despite different names*

### Comparing `psapy-0.4/psapy/GasProp.py` & `psapy-0.5/psapy/GasProp.py`

 * *Files identical despite different names*

### Comparing `psapy-0.4/psapy/Hagendornandbrown.py` & `psapy-0.5/psapy/Hagendornandbrown.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,216 +1,216 @@
-# coding=utf-8
-import FluidProps
-import math
-
-
-def Pgrad(P, T, oil_rate, wtr_rate, Gor, gas_grav, oil_grav, wtr_grav, d, angle):
-    """Function to Calculate the Flowing Pressure Gradient by the Method of Beggs and Brill"""
-    #P          pressure, psia
-    #T          temperature, °F
-    #oil_rate   oil flowrate, stb/d
-    #wtr_rate   water flowrate, stb/d
-    #Gor        producing gas-oil ratio, scf/stb
-    #gas_grav   gas specific gravity
-    #oil_grav   API oil gravity
-    #wtr_grav   water specific gravity
-    #d          pipe I.D., in.
-    #angle      angle of pipe inclination in degrees
-    #               90° = vertical
-    #               0°  = horizontal
-
-    print( 'P', P, ' T ', T, ' WOR ', oil_rate/wtr_rate, ' GOR ', Gor)
-    
-    #Set constants
-    pi = math.pi   #4 * math.atan(1)                                               #Define pi
-    Psep = 114.7                                                        #Separator pressure, psia
-    Tsep = 50                                                           #Separator temperature, °F
-   
-    #Convert pipe angle from degrees to radians
-    angle = angle * pi / 180
-    
-    #Calculate fluid properties
-    Z = FluidProps.zfact((T + 460) / FluidProps.Tc(gas_grav), P / FluidProps.Pc(gas_grav))               #Gas compressibility factor
-    if T==145.0:
-        print ('error')
-       
-    Wor = wtr_rate / oil_rate                                           #Water-oil ratio, stb/stb
-    TDS = FluidProps.salinity(wtr_grav)                                            #Water salinity, wt% total dissolved solids
-    Pb = FluidProps.Pbub(T, Tsep, Psep, gas_grav, oil_grav, Gor)                   #Bubble point pressure, psia
-    Rso = FluidProps.sol_gor(T, P, Tsep, Psep, Pb, gas_grav, oil_grav)             #Solution gas-oil ratio, scf/stb
-    Rsw = FluidProps.sol_gwr(P, T, TDS)                                            #Solution gas_water ratio, scf/stb
-    Bo = FluidProps.oil_fvf(T, P, Tsep, Psep, Pb, Rso, gas_grav, oil_grav)         #Oil formation volume factor, rb/stb
-    Bw = FluidProps.wtr_fvf(P, T, TDS)                                             #Water formation volume factor, rb/stb
-    Bg = FluidProps.gas_fvf(P, T, gas_grav)                                        #Gas formation volume factor, ft_/scf
-    muo = FluidProps.oil_visc(T, P, Tsep, Psep, Pb, Rso, gas_grav, oil_grav)       #Oil viscosity, cp
-    muw = FluidProps.wtr_visc(P, T, TDS)                                           #Water viscosity, cp
-    mug = FluidProps.gvisc(P, (T + 460), Z, gas_grav)                                #Gas viscosity, cp
-    rhoo = FluidProps.oil_dens(T, P, Tsep, Psep, Pb, Bo, Rso, gas_grav, oil_grav)  #Oil density, lb/ft_
-    rhow = 62.368 * wtr_grav / Bw                                                  #Water density, lb/ft_
-    rhog = 2.699 * gas_grav * P / (T + 460) / Z                                    #Gas density, lb/ft_
-    sigo = FluidProps.oil_tens(P, T, oil_grav)                                     #Gas-oil interfacial tension, dynes/cm
-    sigw = FluidProps.wtr_tens(P, T)                                               #Gas-water interfacial tension, dynes/cm
-   
-    #Volume fraction weighted liquid properties
-    rhol = (Bw * Wor * rhow + Bo * rhoo) / (Bw * Wor + Bo)              #Liquid density
-    mul = (Bw * Wor * rhow) / (Bw * Wor * rhow + Bo * rhoo) * muw + (Bo * rhoo) / (Bw * Wor * rhow + Bo * rhoo) * muo             #Liquid viscosity
-    sigl = (Bw * Wor * rhow) / (Bw * Wor * rhow + Bo * rhoo) * sigw + (Bo * rhoo) / (Bw * Wor * rhow + Bo * rhoo) * sigo           #Gas-liquid interfacial tension
-    
-    #Calculate downhole fluid flowrates in ft_/s
-    qo = Bo * oil_rate / 15387                                          #Oil flowrate
-    qw = Bw * Wor * oil_rate / 15387                                    #Water flowrate
-    ql = qo + qw                                                        #Liquid flowrate
-    if ((Gor - Rso) < 0):                                        #If gas flowrate is negative, set to zero
-        qg = 0
-    else:
-        qg = Bg * (Gor - Rso - Rsw * Wor) * oil_rate / 86400
-    
-        
-    #Calculate fluid superficial velocities in ft/s
-    Axs = pi / 4 * (d / 12) ** 2                                         #X-sectional area of pipe, ft_
-    usl = ql / Axs                                                      #Liquid superficial velocity
-    usg = qg / Axs                                                      #Gas superficial velocity
-    um = usl + usg                                                      #Mixture superficial velocity
-    
-
-    #Determine flow regime
-    A= 1.071 -((0.2218*um**2)/(d))
-
-    if A<0.13:
-        A=0.13
-    B= usg/(um)
-
-    if B-A>=0:
-        ## use Griffing Lquid holp up Correlation 
-        us=0.8*0.3048
-        x=(1+um/us)**2-4*usg/us
-        HL=1-0.5*(1+um/us-math.sqrt(x))
-
-    else:
-        ## Use H&B holdup correlation
-        ## Calculate liquid viscosity number and coefficient
-        g=32.174 
-        NL=0.15726*mul*(1/(rhol*sigl**3))**0.25
-        CNL=0.061*NL**3-0.0929*NL**2+0.0505*NL+0.0019
-        #print ' CNL ', CNL  
-        ##CNL=(0.0019+0.0322*NL-0.6642*NL**2+4.9951*NL**3)/(1-10.0147*NL+33.8696*NL**2+277.2817*NL**3)
-
-        #if NL<== 0.002:
-        #    CNL=0.0019
-        #if NL>= 0.4:
-        #    CNL=0.0115
-
-        #Calculate liquid, gas velocity number and pipe diametre number
-        # 0
-        NLv=1.938*usl*(rhol/(sigl))**0.25  
-        NGv=1.938*usg*(rhol/(sigl))**0.25  
-        ND=120.872*d/12*math.sqrt(rhol/(sigl))
-
-        if NGv==0:
-            H=0
-        else:   
-            H=NLv/(NGv**0.575)*(P/14.7)**0.1*CNL/ND
-    
-        H_Phi=math.sqrt((0.047+(1123.32)*H+729489.64*H**2)/(1+1097.1556*H+722153.97*H**2))
-
-        B=NGv*(NLv**0.38)/(ND**2.14)
-
-        if B<=0.025:
-            PHI=27170*B**3-317.52*B**2+0.5472*B+0.9999
-        if (B>0.025 and B<=0.055):
-            PHI=-5333.33*B**2+58.524*B+0.1171
-        if B>0.055:
-            PHI=2.5714*B+1.5962
-
-        HL=H_Phi*PHI
-
-     #Liquid velocity number
-    laml = usl / um                                                     #Input liquid fraction
-    lamg = 1 - laml                                                     #Input gas fraction
-    L1 = 316 * laml ** 0.302                                             #Dimensionless constants
-    L2 = 0.0009252 * laml ** -2.4684
-    L3 = 0.1 * laml ** -1.4516
-    L4 = 0.5 * laml ** -6.738
-
-    yl=HL
-    yg=1-HL
-
-    #Calculate fluid mixture properties
-    rhom = rhol * laml + rhog * lamg                                      #Input fraction weighted density, lb/ft_
-    #mum = mul * laml + mug * lamg                                        #Input fraction weighted viscosity, cp
-    mum=mul**yl*mug**(yg)
-    rhobar = rhol * yl + rhog * yg                                       #In-situ average density, lb/ft_
-    
-    #Calculate friction factor
-    Nre = 1488 * rhom * um * (d / 12) / mum                              #Reynolds number
-    fn = Fric(Nre, 0.0006)   
-    #print 'friction ' , fn , ' Nre ', Nre     ,' HL ' ,HL , ' Oil ', oil_rate ,' water ', wtr_rate , ' Pressure ', P                                      #No-slip friction factor
-    x = laml / HL ** 2
-    if ((x > 1) and (x < 1.2)):
-        s = math.log(2.2 * x - 1.2)
-    else:
-        s = math.log(x) / (-0.0523 + 3.182 * math.log(x) - 0.8725 * (math.log(x)) ** 2 + 0.01853 * (math.log(x)) ** 4)
-    
-    ftp = fn * math.exp(s)                                                    #Two-phase friction factor
-    
-    #Calculate gradients
-    Pgrad_pe = rhobar * math.sin(angle) / 144                                 #Potential energy pressure gradient, psi/ft
-    Pgrad_f = 2 * ftp * rhom * um ** 2 / 32.17 / (d / 12) / 144           #Frictional pressure gradient, psi/ft
-    Ek = um * usg * rhobar / 32.17 / P / 144                              #Kinetic energy factor
-    return (Pgrad_pe + Pgrad_f) / (1 - Ek)                               #Overall pressure gradient, psi/ft
-
-
-
-def Fric(Nre, eps):
-    """Calculate Fanning Friction Factor using the Chen Equation """
-    try:
-        math.log
-        Temp = -4 * math.log10((eps / 3.7065) - (5.0452 / Nre) * math.log10((eps ** 1.1098 / 2.8257) + (7.149 / Nre) ** 0.8981) ) 
-    except Exception as inst:
-         print(type(inst))    # the exception instance
-         print(inst.args)     # arguments stored in .args
-         print(inst)       
-    
-    return (1 / Temp) ** 2
-
-
-
-
-def Pwf_q(FWHP, FWHT,Oil_Rate,Water_Rate,GOR,GasGrav,API, WaterGrav, ID, Angle, Depth, FBHT):
-    """Function to calculate the Pwf as function of rate"""
-    DPs = []          ## Start as the empty list
-    Temps=[]
-    Press=[]
-    PressList=[]
-    DepthList=[]
-    i=0
-    PressList.append(FWHP)
-    Temps.append(FWHT)
-    DepthList.append(0)
-    DPs.append(0)
-    nSteps=60
-    i=1
-    Tgrad= (FBHT-FWHT)/ Depth
-
-    while (i<= nSteps):
-    
-        DeltaD= Depth/nSteps*i
-        DepthList.append(DeltaD) 
-    
-        T=FWHT+Tgrad*DeltaD
-        Temps.append(T)
-        p=PressList[i-1]+DPs[i-1]*(DepthList[i]-DepthList[i-1])     
-        dp= Pgrad(p,T,Oil_Rate,Water_Rate,GOR,GasGrav,API, WaterGrav, ID, Angle)
-        DPs.append(dp)
-        
-        PressList.append(p)
-        i=i+1
-
-    return PressList[-1]
-
-
-
-
-
-
-
+# coding=utf-8
+import FluidProps
+import math
+
+
+def Pgrad(P, T, oil_rate, wtr_rate, Gor, gas_grav, oil_grav, wtr_grav, d, angle):
+    """Function to Calculate the Flowing Pressure Gradient by the Method of Beggs and Brill"""
+    #P          pressure, psia
+    #T          temperature, °F
+    #oil_rate   oil flowrate, stb/d
+    #wtr_rate   water flowrate, stb/d
+    #Gor        producing gas-oil ratio, scf/stb
+    #gas_grav   gas specific gravity
+    #oil_grav   API oil gravity
+    #wtr_grav   water specific gravity
+    #d          pipe I.D., in.
+    #angle      angle of pipe inclination in degrees
+    #               90° = vertical
+    #               0°  = horizontal
+
+    print( 'P', P, ' T ', T, ' WOR ', oil_rate/wtr_rate, ' GOR ', Gor)
+    
+    #Set constants
+    pi = math.pi   #4 * math.atan(1)                                               #Define pi
+    Psep = 114.7                                                        #Separator pressure, psia
+    Tsep = 50                                                           #Separator temperature, °F
+   
+    #Convert pipe angle from degrees to radians
+    angle = angle * pi / 180
+    
+    #Calculate fluid properties
+    Z = FluidProps.zfact((T + 460) / FluidProps.Tc(gas_grav), P / FluidProps.Pc(gas_grav))               #Gas compressibility factor
+    if T==145.0:
+        print ('error')
+       
+    Wor = wtr_rate / oil_rate                                           #Water-oil ratio, stb/stb
+    TDS = FluidProps.salinity(wtr_grav)                                            #Water salinity, wt% total dissolved solids
+    Pb = FluidProps.Pbub(T, Tsep, Psep, gas_grav, oil_grav, Gor)                   #Bubble point pressure, psia
+    Rso = FluidProps.sol_gor(T, P, Tsep, Psep, Pb, gas_grav, oil_grav)             #Solution gas-oil ratio, scf/stb
+    Rsw = FluidProps.sol_gwr(P, T, TDS)                                            #Solution gas_water ratio, scf/stb
+    Bo = FluidProps.oil_fvf(T, P, Tsep, Psep, Pb, Rso, gas_grav, oil_grav)         #Oil formation volume factor, rb/stb
+    Bw = FluidProps.wtr_fvf(P, T, TDS)                                             #Water formation volume factor, rb/stb
+    Bg = FluidProps.gas_fvf(P, T, gas_grav)                                        #Gas formation volume factor, ft_/scf
+    muo = FluidProps.oil_visc(T, P, Tsep, Psep, Pb, Rso, gas_grav, oil_grav)       #Oil viscosity, cp
+    muw = FluidProps.wtr_visc(P, T, TDS)                                           #Water viscosity, cp
+    mug = FluidProps.gvisc(P, (T + 460), Z, gas_grav)                                #Gas viscosity, cp
+    rhoo = FluidProps.oil_dens(T, P, Tsep, Psep, Pb, Bo, Rso, gas_grav, oil_grav)  #Oil density, lb/ft_
+    rhow = 62.368 * wtr_grav / Bw                                                  #Water density, lb/ft_
+    rhog = 2.699 * gas_grav * P / (T + 460) / Z                                    #Gas density, lb/ft_
+    sigo = FluidProps.oil_tens(P, T, oil_grav)                                     #Gas-oil interfacial tension, dynes/cm
+    sigw = FluidProps.wtr_tens(P, T)                                               #Gas-water interfacial tension, dynes/cm
+   
+    #Volume fraction weighted liquid properties
+    rhol = (Bw * Wor * rhow + Bo * rhoo) / (Bw * Wor + Bo)              #Liquid density
+    mul = (Bw * Wor * rhow) / (Bw * Wor * rhow + Bo * rhoo) * muw + (Bo * rhoo) / (Bw * Wor * rhow + Bo * rhoo) * muo             #Liquid viscosity
+    sigl = (Bw * Wor * rhow) / (Bw * Wor * rhow + Bo * rhoo) * sigw + (Bo * rhoo) / (Bw * Wor * rhow + Bo * rhoo) * sigo           #Gas-liquid interfacial tension
+    
+    #Calculate downhole fluid flowrates in ft_/s
+    qo = Bo * oil_rate / 15387                                          #Oil flowrate
+    qw = Bw * Wor * oil_rate / 15387                                    #Water flowrate
+    ql = qo + qw                                                        #Liquid flowrate
+    if ((Gor - Rso) < 0):                                        #If gas flowrate is negative, set to zero
+        qg = 0
+    else:
+        qg = Bg * (Gor - Rso - Rsw * Wor) * oil_rate / 86400
+    
+        
+    #Calculate fluid superficial velocities in ft/s
+    Axs = pi / 4 * (d / 12) ** 2                                         #X-sectional area of pipe, ft_
+    usl = ql / Axs                                                      #Liquid superficial velocity
+    usg = qg / Axs                                                      #Gas superficial velocity
+    um = usl + usg                                                      #Mixture superficial velocity
+    
+
+    #Determine flow regime
+    A= 1.071 -((0.2218*um**2)/(d))
+
+    if A<0.13:
+        A=0.13
+    B= usg/(um)
+
+    if B-A>=0:
+        ## use Griffing Lquid holp up Correlation 
+        us=0.8*0.3048
+        x=(1+um/us)**2-4*usg/us
+        HL=1-0.5*(1+um/us-math.sqrt(x))
+
+    else:
+        ## Use H&B holdup correlation
+        ## Calculate liquid viscosity number and coefficient
+        g=32.174 
+        NL=0.15726*mul*(1/(rhol*sigl**3))**0.25
+        CNL=0.061*NL**3-0.0929*NL**2+0.0505*NL+0.0019
+        #print ' CNL ', CNL  
+        ##CNL=(0.0019+0.0322*NL-0.6642*NL**2+4.9951*NL**3)/(1-10.0147*NL+33.8696*NL**2+277.2817*NL**3)
+
+        #if NL<== 0.002:
+        #    CNL=0.0019
+        #if NL>= 0.4:
+        #    CNL=0.0115
+
+        #Calculate liquid, gas velocity number and pipe diametre number
+        # 0
+        NLv=1.938*usl*(rhol/(sigl))**0.25  
+        NGv=1.938*usg*(rhol/(sigl))**0.25  
+        ND=120.872*d/12*math.sqrt(rhol/(sigl))
+
+        if NGv==0:
+            H=0
+        else:   
+            H=NLv/(NGv**0.575)*(P/14.7)**0.1*CNL/ND
+    
+        H_Phi=math.sqrt((0.047+(1123.32)*H+729489.64*H**2)/(1+1097.1556*H+722153.97*H**2))
+
+        B=NGv*(NLv**0.38)/(ND**2.14)
+
+        if B<=0.025:
+            PHI=27170*B**3-317.52*B**2+0.5472*B+0.9999
+        if (B>0.025 and B<=0.055):
+            PHI=-5333.33*B**2+58.524*B+0.1171
+        if B>0.055:
+            PHI=2.5714*B+1.5962
+
+        HL=H_Phi*PHI
+
+     #Liquid velocity number
+    laml = usl / um                                                     #Input liquid fraction
+    lamg = 1 - laml                                                     #Input gas fraction
+    L1 = 316 * laml ** 0.302                                             #Dimensionless constants
+    L2 = 0.0009252 * laml ** -2.4684
+    L3 = 0.1 * laml ** -1.4516
+    L4 = 0.5 * laml ** -6.738
+
+    yl=HL
+    yg=1-HL
+
+    #Calculate fluid mixture properties
+    rhom = rhol * laml + rhog * lamg                                      #Input fraction weighted density, lb/ft_
+    #mum = mul * laml + mug * lamg                                        #Input fraction weighted viscosity, cp
+    mum=mul**yl*mug**(yg)
+    rhobar = rhol * yl + rhog * yg                                       #In-situ average density, lb/ft_
+    
+    #Calculate friction factor
+    Nre = 1488 * rhom * um * (d / 12) / mum                              #Reynolds number
+    fn = Fric(Nre, 0.0006)   
+    #print 'friction ' , fn , ' Nre ', Nre     ,' HL ' ,HL , ' Oil ', oil_rate ,' water ', wtr_rate , ' Pressure ', P                                      #No-slip friction factor
+    x = laml / HL ** 2
+    if ((x > 1) and (x < 1.2)):
+        s = math.log(2.2 * x - 1.2)
+    else:
+        s = math.log(x) / (-0.0523 + 3.182 * math.log(x) - 0.8725 * (math.log(x)) ** 2 + 0.01853 * (math.log(x)) ** 4)
+    
+    ftp = fn * math.exp(s)                                                    #Two-phase friction factor
+    
+    #Calculate gradients
+    Pgrad_pe = rhobar * math.sin(angle) / 144                                 #Potential energy pressure gradient, psi/ft
+    Pgrad_f = 2 * ftp * rhom * um ** 2 / 32.17 / (d / 12) / 144           #Frictional pressure gradient, psi/ft
+    Ek = um * usg * rhobar / 32.17 / P / 144                              #Kinetic energy factor
+    return (Pgrad_pe + Pgrad_f) / (1 - Ek)                               #Overall pressure gradient, psi/ft
+
+
+
+def Fric(Nre, eps):
+    """Calculate Fanning Friction Factor using the Chen Equation """
+    try:
+        math.log
+        Temp = -4 * math.log10((eps / 3.7065) - (5.0452 / Nre) * math.log10((eps ** 1.1098 / 2.8257) + (7.149 / Nre) ** 0.8981) ) 
+    except Exception as inst:
+         print(type(inst))    # the exception instance
+         print(inst.args)     # arguments stored in .args
+         print(inst)       
+    
+    return (1 / Temp) ** 2
+
+
+
+
+def Pwf_q(FWHP, FWHT,Oil_Rate,Water_Rate,GOR,GasGrav,API, WaterGrav, ID, Angle, Depth, FBHT):
+    """Function to calculate the Pwf as function of rate"""
+    DPs = []          ## Start as the empty list
+    Temps=[]
+    Press=[]
+    PressList=[]
+    DepthList=[]
+    i=0
+    PressList.append(FWHP)
+    Temps.append(FWHT)
+    DepthList.append(0)
+    DPs.append(0)
+    nSteps=60
+    i=1
+    Tgrad= (FBHT-FWHT)/ Depth
+
+    while (i<= nSteps):
+    
+        DeltaD= Depth/nSteps*i
+        DepthList.append(DeltaD) 
+    
+        T=FWHT+Tgrad*DeltaD
+        Temps.append(T)
+        p=PressList[i-1]+DPs[i-1]*(DepthList[i]-DepthList[i-1])     
+        dp= Pgrad(p,T,Oil_Rate,Water_Rate,GOR,GasGrav,API, WaterGrav, ID, Angle)
+        DPs.append(dp)
+        
+        PressList.append(p)
+        i=i+1
+
+    return PressList[-1]
+
+
+
+
+
+
+
 #print(Pgrad(150,101,100,50,300,0.65,35,1.07,2.44,90))
```

### Comparing `psapy-0.4/psapy/OilProps.py` & `psapy-0.5/psapy/OilProps.py`

 * *Files identical despite different names*

### Comparing `psapy-0.4/psapy/Solving_Intersections.py` & `psapy-0.5/psapy/Solving_Intersections.py`

 * *Files identical despite different names*

### Comparing `psapy-0.4/psapy/Vogel.py` & `psapy-0.5/psapy/Vogel.py`

 * *Files identical despite different names*

### Comparing `psapy-0.4/psapy/WaterProps.py` & `psapy-0.5/psapy/WaterProps.py`

 * *Files identical despite different names*

