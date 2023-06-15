# Comparing `tmp/atooms_dynamics-1.0.0-py2.py3-none-any.whl.zip` & `tmp/atooms_dynamics-1.1.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 13513 bytes, number of entries: 14
+Zip file size: 14231 bytes, number of entries: 14
 -rw-rw-r--  2.0 unx      159 b- defN 21-Oct-30 16:47 atooms/__init__.py
--rw-rw-r--  2.0 unx      108 b- defN 22-Jan-22 16:31 atooms/dynamics/__init__.py
--rw-rw-r--  2.0 unx     5422 b- defN 22-Apr-27 16:09 atooms/dynamics/api.py
+-rw-rw-r--  2.0 unx       51 b- defN 23-Jun-15 21:16 atooms/dynamics/__init__.py
+-rw-rw-r--  2.0 unx     6037 b- defN 22-Nov-17 11:29 atooms/dynamics/api.py
 -rw-rw-r--  2.0 unx     1075 b- defN 22-Feb-17 20:47 atooms/dynamics/base.py
 -rw-rw-r--  2.0 unx      579 b- defN 22-Jan-16 16:37 atooms/dynamics/helpers.py
 -rw-rw-r--  2.0 unx     9680 b- defN 22-Jan-29 20:16 atooms/dynamics/kernels_hard.f90
--rw-rw-r--  2.0 unx     3315 b- defN 22-Apr-27 16:17 atooms/dynamics/kernels_soft.f90
--rw-rw-r--  2.0 unx    10033 b- defN 22-Apr-27 14:59 atooms/dynamics/newtonian.py
--rw-rw-r--  2.0 unx     3754 b- defN 22-Jan-29 20:14 atooms/dynamics/stochastic.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Apr-27 16:27 atooms_dynamics-1.0.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3537 b- defN 22-Apr-27 16:27 atooms_dynamics-1.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 22-Apr-27 16:27 atooms_dynamics-1.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       23 b- defN 22-Apr-27 16:27 atooms_dynamics-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1172 b- defN 22-Apr-27 16:27 atooms_dynamics-1.0.0.dist-info/RECORD
-14 files, 38967 bytes uncompressed, 11555 bytes compressed:  70.3%
+-rw-rw-r--  2.0 unx     4232 b- defN 23-Jun-15 21:16 atooms/dynamics/kernels_soft.f90
+-rw-rw-r--  2.0 unx    11462 b- defN 23-Jun-15 21:16 atooms/dynamics/newtonian.py
+-rw-rw-r--  2.0 unx     3788 b- defN 23-Jun-15 21:16 atooms/dynamics/stochastic.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jun-15 21:29 atooms_dynamics-1.1.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3640 b- defN 23-Jun-15 21:29 atooms_dynamics-1.1.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jun-15 21:29 atooms_dynamics-1.1.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       23 b- defN 23-Jun-15 21:29 atooms_dynamics-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1171 b- defN 23-Jun-15 21:29 atooms_dynamics-1.1.0.dist-info/RECORD
+14 files, 42007 bytes uncompressed, 12273 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: atooms/dynamics/newtonian.py
 Comment: 
 
 Filename: atooms/dynamics/stochastic.py
 Comment: 
 
-Filename: atooms_dynamics-1.0.0.dist-info/LICENSE
+Filename: atooms_dynamics-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: atooms_dynamics-1.0.0.dist-info/METADATA
+Filename: atooms_dynamics-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: atooms_dynamics-1.0.0.dist-info/WHEEL
+Filename: atooms_dynamics-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: atooms_dynamics-1.0.0.dist-info/top_level.txt
+Filename: atooms_dynamics-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: atooms_dynamics-1.0.0.dist-info/RECORD
+Filename: atooms_dynamics-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## atooms/dynamics/__init__.py

```diff
@@ -1,2 +1,2 @@
-from .newtonian import VelocityVerlet, NosePoincare, EventDriven
-from .stochastic import LangevinOverdamped
+from .newtonian import *
+from .stochastic import *
```

## atooms/dynamics/api.py

```diff
@@ -1,47 +1,54 @@
 import os
 import numpy
 import random
 
-from atooms.core.utils import setup_logging, mkdir
+from atooms.core.utils import setup_logging, mkdir, rmf
 from atooms.models import f90
 from atooms.simulation import Simulation
 from atooms.trajectory import Trajectory, TrajectoryXYZ, change_species
 from atooms.simulation.observers import write_config, write_thermo, Scheduler, target_rmsd
 
 from .newtonian import VelocityVerlet, NosePoincare
 from .stochastic import LangevinOverdamped
 
+def _clear_logging():
+    import logging
+    log = logging.getLogger()
+    for h in log.handlers[-2:]:
+        log.removeHandler(h)
 
-# The two runners differ only because of the backend and the
-# corresponding input parameters. To reduce the boilerplate we could
-# proceed as for postprocessing or with landscape
-# TODO: factory / facade?
+# TODO: some parts can be refactored via factory / facade?
 
 def md(file_inp, file_out, method='velocity-verlet', model=None,
-       T=-1.0, Q=5.0, nsteps=0, interval_thermostat=5000, config_number=0,
-       rmsd=-1.0, thermo_number=0, thermo_interval=0, verbose=False,
-       seed=1, skin=0.3, dt=0.002, block='', parallel=False):
+       T=-1.0, Q=5.0, nsteps=0, checkpoint_interval=0, config_number=0,
+       thermo_number=0, thermo_interval=0,
+       thermo_fields='steps,temperature,potential energy per particle,pressure,conserved energy,rmsd',
+       interval_thermostat=5000, rmsd=-1.0, verbose=False, seed=1,
+       skin=0.3, dt=0.002, block='', parallel=False, fmt=None,
+       restart=False, dry=False):
     """
     Molecular dynamics simulation
     """
 
     # Initialize
     random.seed(seed)
     numpy.random.seed(seed)
 
-    mkdir(os.path.dirname(file_out))
-    
     # Always log to file
+    mkdir(os.path.dirname(file_out))
+    if not restart:
+        rmf(file_out + '.log')
     setup_logging(level=20, filename=file_out + '.log')
     if verbose:
         setup_logging(level=20)
 
     # Read initial state
-    with Trajectory(file_inp) as th:
+    # We read the last config of file_inp
+    with Trajectory(file_inp, fmt=fmt) as th:
         system = th[-1]
 
     # Setup interaction
     system = change_species(system, 'F')
     if system.number_of_dimensions == 3:
         system.interaction = f90.Interaction(model, helpers='helpers_3d.f90', parallel=parallel)
     else:
@@ -66,42 +73,46 @@
         system.temperature = T
 
     # Fix targeting
     if rmsd > 0 and nsteps == 0:
         nsteps = int(1e7)
 
     # Simulation
-    sim = Simulation(bck, output_path=file_out, steps=nsteps, enable_speedometer=True)
+    sim = Simulation(bck, output_path=file_out, steps=nsteps,
+                     enable_speedometer=True, restart=restart,
+                     checkpoint_interval=checkpoint_interval)
+    sim.checkpoint_variables = ['species', 'position', 'velocity',
+                                'radius', 'position_unfolded']
     sim.trajectory_class = TrajectoryXYZ
     if method == 'massive-thermostat':
         sim.add(massive_thermostat, interval_thermostat, T)
 
-    # Writing
+    # Writing trajectory file
     if config_number == 0:
         if len(block) > 0:
             sim.add(write_config, Scheduler(block=[int(_) for _ in block.split(',')]))
     else:
         sim.add(write_config, Scheduler(calls=config_number))
 
+    # Writing thermodynamic data
+    thermo_fields = thermo_fields.split(',')
+    _func = {'conserved energy': lambda x: x.backend.conserved_energy}
     if thermo_number > 0:
-        sim.add(write_thermo, Scheduler(calls=thermo_number))
+        sim.add(write_thermo, Scheduler(calls=thermo_number), fields=thermo_fields, functions=_func)
     elif thermo_interval > 0:
-        sim.add(write_thermo, Scheduler(thermo_interval))
+        sim.add(write_thermo, Scheduler(thermo_interval), fields=thermo_fields, functions=_func)
 
+    # Targeting
     if rmsd > 0:
-        sim.add(target_rmsd, Scheduler(50000), rmsd)
+        sim.add(target_rmsd, Scheduler(5000), rmsd)
 
     # Run
-    sim.run()
-
-    # Write final configuration
-    with Trajectory(file_out + '.chk.xyz', 'w', fmt='xyz') as th:
-        th.variables = ['id', 'pos', 'vel']
-        th.precision = 12
-        th.write(sim.system)
+    if not dry:
+        sim.run()
+        _clear_logging()
 
     return sim
 
 
 def ld(file_inp, file_out, method='overdamped', model=None, T=-1.0,
        nsteps=0, interval_thermostat=5000, config_number=0, rmsd=-1.0,
        thermo_number=0, thermo_interval=0, verbose=False, skin=0.3,
@@ -116,15 +127,15 @@
         random = numpy.random.default_rng(seed=seed)
     elif random in ['MT', 'MT19937']:
         random = numpy.random
     else:
         raise ValueError('unknown random generator {}'.format(random))
 
     mkdir(os.path.dirname(file_out))
-    
+
     # Always log to file
     setup_logging(level=20, filename=file_out + '.log')
     if verbose:
         setup_logging(level=20)
 
     # Read initial state
     with Trajectory(file_inp) as th:
@@ -160,14 +171,15 @@
         sim.add(write_thermo, Scheduler(thermo_interval))
 
     if rmsd > 0:
         sim.add(target_rmsd, Scheduler(50000), rmsd)
 
     # Run
     sim.run()
+    _clear_logging()
 
     # Write final configuration
     with Trajectory(file_out + '.chk.xyz', 'w', fmt='xyz') as th:
         th.variables = ['id', 'pos', 'vel']
         th.precision = 12
         th.write(sim.system)
```

## atooms/dynamics/kernels_soft.f90

```diff
@@ -91,9 +91,31 @@
        pimm = pi + dt * (ekin - (epot_old+epot)/2 + (H_0 - ndim*ndf*T*(log(s)+1)))
        s = s * (1+pimm/(4*Q)*dt)**2
        pi = pimm / (1+pimm/(4*Q)*dt)
        vel = vel + forces / mass * dt / 2
        vel = vel * s_old / s
     end if
   end subroutine evolve_nose_poincare
+
+  subroutine rescale_berendsen(T, mass_T, P, mass_P, box, pos, vel, mass, virial)
+    double precision, intent(in)    :: T, P, mass_T, mass_P, mass(:,:), virial
+    double precision, intent(inout) :: pos(:,:), vel(:,:), box(:)
+    double precision                :: ekin,temp,pres,chi_pres,chi_temp
+    integer                         :: i, ndim, npart
+    ndim = size(pos,1)
+    npart = size(pos,2)
+    ekin = sum([(sum(mass(:,i) * vel(:,i)**2) / 2, i=1,size(pos,2))])
+    temp = ekin * 2.d0 / (ndim*(npart-1))
+    if (P > 0) then
+       !pres = (npart * temp + virial / ndim) / product(box)
+       pres = (npart * T + virial / ndim) / product(box)
+       chi_pres = (1 - mass_P * (P - pres))**(1.d0/3)
+       box = box * chi_pres
+       pos = pos * chi_pres
+    end if
+    if (T > 0) then
+       chi_temp = sqrt(1 + mass_T*(T/temp - 1.d0))
+       vel = vel * chi_temp
+    end if
+  end subroutine rescale_berendsen
   
 end module methods
```

## atooms/dynamics/newtonian.py

```diff
@@ -4,14 +4,16 @@
 import math
 import numpy
 import logging
 import f2py_jit
 from atooms.system import Thermostat
 from .base import _Dynamics
 
+__all__ = ['VelocityVerlet', 'NosePoincare', 'EventDriven', 'Berendsen']
+
 _log = logging.getLogger(__name__)
 _f90_kernel_soft = os.path.join(os.path.dirname(__file__), 'kernels_soft.f90')
 _f90_kernel_hard = os.path.join(os.path.dirname(__file__), 'kernels_hard.f90')
 
 
 class VelocityVerlet(_Dynamics):
 
@@ -33,52 +35,42 @@
 timestep: {}
 """.format(self.__class__, self.timestep)
 
     def run(self, steps):
         # Dump the arrays before we start. This can be done at each
         # run() call because we ask for views, and this does not incur
         # into overhead.
-        _box = self.system.dump('cell.side', dtype='float64', view=True)
-        _pos = self.system.dump('particle.position', dtype='float64', order='F', view=True)
-        _vel = self.system.dump('particle.velocity', dtype='float64', order='F', view=True)
-        _ids = self.system.dump('particle.species', dtype='int32', view=True)
-        _rad = self.system.dump('particle.radius', dtype='float64', view=True)
-        _pos_unf = self.system.dump('particle.position_unfolded', order='F', view=True)
+        _box = self.system.view('cell.side', dtype='float64')
+        _pos = self.system.view('particle.position', dtype='float64', order='F')
+        _vel = self.system.view('particle.velocity', dtype='float64', order='F')
+        _ids = self.system.view('particle.species', dtype='int32')
+        _rad = self.system.view('particle.radius', dtype='float64')
+        _pos_unf = self.system.view('particle.position_unfolded', order='F')
         # Masses have to be replicated along the spatial dimensions to keep the vector syntax
         # The None indexing syntax adds a new dimension to the array
-        _mas = self.system.dump('particle.mass', dtype='float64', view=True)
+        _mas = self.system.view('particle.mass', dtype='float64')
         _mas = numpy.repeat(_mas[:, numpy.newaxis], len(_box), axis=1)
         _mas = numpy.transpose(_mas, (1, 0))
         if self._reference_energy is None:
             self._reference_energy = self.system.total_energy()
 
         # Build f90 kernel module
         f90 = f2py_jit.jit(_f90_kernel_soft)
 
         # Main loop
         for _ in range(steps):
-            f90.methods.evolve_velocity_verlet(1,
-                                               self.timestep,
+            f90.methods.evolve_velocity_verlet(1, self.timestep,
                                                self.system.interaction.forces,
-                                               _box,
-                                               _pos,
-                                               _pos_unf,
-                                               _vel,
-                                               _ids,
-                                               _mas)
+                                               _box, _pos, _pos_unf,
+                                               _vel, _ids, _mas)
             self.system.compute_interaction('forces')
-            f90.methods.evolve_velocity_verlet(2,
-                                               self.timestep,
+            f90.methods.evolve_velocity_verlet(2, self.timestep,
                                                self.system.interaction.forces,
-                                               _box,
-                                               _pos,
-                                               _pos_unf,
-                                               _vel,
-                                               _ids,
-                                               _mas)
+                                               _box, _pos, _pos_unf,
+                                               _vel, _ids, _mas)
 
         self.conserved_energy = self.system.total_energy(cache=True) - self._reference_energy
 
 
 class NosePoincare(_Dynamics):
 
     def __init__(self, system, timestep=0.001, temperature=-1.0, mass=5.0):
@@ -88,14 +80,16 @@
         self.conserved_energy = 0.0
         self.timestep = timestep
 
         # Thermostat
         if system.thermostat is None:
             assert temperature > 0.0
             system.thermostat = Thermostat(temperature, mass=mass)
+        elif temperature > 0.0:
+            system.thermostat.temperature = temperature
 
         # We compute the initial potential energy
         self.system.compute_interaction('forces')
         self._reference_energy = None
 
     def __str__(self):
         return """
@@ -105,23 +99,23 @@
 temperature: {}
 """.format(self.timestep, self.system.thermostat.temperature)
 
     def run(self, steps):
         # Dump the arrays before we start. This can be done at each
         # run() call because we ask for views, and this does not incur
         # into overhead.
-        _box = self.system.dump('cell.side', dtype='float64', view=True)
-        _pos = self.system.dump('particle.position', dtype='float64', order='F', view=True)
-        _vel = self.system.dump('particle.velocity', dtype='float64', order='F', view=True)
-        _ids = self.system.dump('particle.species', dtype='int32', view=True)
-        _rad = self.system.dump('particle.radius', dtype='float64', view=True)
-        _pos_unf = self.system.dump('particle.position_unfolded', order='F', view=True)
+        _box = self.system.view('cell.side', dtype='float64')
+        _pos = self.system.view('particle.position', dtype='float64', order='F')
+        _vel = self.system.view('particle.velocity', dtype='float64', order='F')
+        _ids = self.system.view('particle.species', dtype='int32')
+        _rad = self.system.view('particle.radius', dtype='float64')
+        _pos_unf = self.system.view('particle.position_unfolded', order='F')
         # Masses have to be replicated along the spatial dimensions to keep the vector syntax
         # The None indexing syntax adds a new dimension to the array
-        _mas = self.system.dump('particle.mass', dtype='float64', view=True)
+        _mas = self.system.view('particle.mass', dtype='float64')
         _mas = numpy.repeat(_mas[:, numpy.newaxis], len(_box), axis=1)
         _mas = numpy.transpose(_mas, (1, 0))
         # Make sure the thermostat coordinates are 0-dim arrays
         # TODO: this calls for coords/moms to be added to Thermostat
         thermostat = self.system.thermostat
         # Reference energy
         ndim = self.system.number_of_dimensions
@@ -134,47 +128,37 @@
                 ndf * thermostat.temperature * math.log(thermostat.coordinate)
 
         # Build f90 kernel module
         f90 = f2py_jit.jit(_f90_kernel_soft)
 
         # Main loop
         for _ in range(steps):
-            f90.methods.evolve_nose_poincare(1,
-                                             self.timestep,
+            f90.methods.evolve_nose_poincare(1, self.timestep,
                                              self.system.interaction.forces,
                                              0.0, 0.0,
                                              thermostat.temperature,
                                              thermostat.coordinate,
                                              thermostat.momentum,
                                              thermostat.mass,
                                              self._reference_energy,
-                                             _box,
-                                             _pos,
-                                             _pos_unf,
-                                             _vel,
-                                             _ids,
-                                             _mas)
+                                             _box, _pos, _pos_unf,
+                                             _vel, _ids, _mas)
             epot_old = self.system.interaction.energy
             self.system.compute_interaction('forces')
             epot_new = self.system.interaction.energy
-            f90.methods.evolve_nose_poincare(2,
-                                             self.timestep,
+            f90.methods.evolve_nose_poincare(2, self.timestep,
                                              self.system.interaction.forces,
                                              epot_old, epot_new,
                                              thermostat.temperature,
                                              thermostat.coordinate,
                                              thermostat.momentum,
                                              thermostat.mass,
                                              self._reference_energy,
-                                             _box,
-                                             _pos,
-                                             _pos_unf,
-                                             _vel,
-                                             _ids,
-                                             _mas)
+                                             _box, _pos, _pos_unf,
+                                             _vel, _ids, _mas)
 
         energy = self.system.total_energy(cache=True) + \
             thermostat.momentum**2 / (2*thermostat.mass) + \
             ndf * thermostat.temperature * math.log(thermostat.coordinate)
         self.conserved_energy = thermostat.coordinate * (energy - self._reference_energy)
 
 
@@ -200,25 +184,75 @@
     def run(self, steps):
         # Build f90 kernel module
         f90 = f2py_jit.jit(_f90_kernel_hard)
         # TODO: Inlining with 0.6.0 gives a seg fault
         # f90 = f2py_jit.jit(f2py_jit.inline(_f90_kernel_hard))  #, extra_args='--opt="-fbounds-check"')
 
         # Dump variables
-        box = self.system.dump('cell.side', view=True)
-        pos = self.system.dump('particle.position', order='F', view=True)
-        unf = self.system.dump('particle.position_unfolded', order='F', view=True)
-        vel = self.system.dump('particle.velocity', order='F', view=True)
-        ids = self.system.dump('particle.species', dtype='int32', view=True)
-        rad = self.system.dump('particle.radius', view=True)
+        box = self.system.view('cell.side')
+        pos = self.system.view('particle.position', order='F')
+        unf = self.system.view('particle.position_unfolded', order='F')
+        vel = self.system.view('particle.velocity', order='F')
+        ids = self.system.view('particle.species', dtype='int32')
+        rad = self.system.view('particle.radius')
         if not self._init:
             self._coltime = numpy.ndarray(len(self.system.particle))
             self._partner = numpy.ndarray(len(self.system.particle), dtype='int32')
-            f90.methods.run(pos, unf, vel, rad*2, box[0], self.timestep, 0, self._coltime, self._partner)
+            f90.methods.run(pos, unf, vel, rad*2, box[0],
+                            self.timestep, 0, self._coltime, self._partner)
             self._init = True
 
         # Main loop
         virial = f90.methods.run(pos, unf, vel, rad*2, box[0], self.timestep, steps, self._coltime, self._partner)
         self.system.interaction.virial = virial * self.system.number_of_dimensions
 
 
 EventDriven = EventDrivenAllenTildesley
+
+
+class Berendsen(_Dynamics):
+
+    def __init__(self, system, timestep=0.001):
+        _Dynamics.__init__(self, system)
+        self.timestep = timestep
+        self.system.compute_interaction('forces')
+        self._T, self._mass_T = -1.0, 1.0
+        self._P, self._mass_P = -1.0, 1.0
+        if system.thermostat is not None:
+            self._T = system.thermostat.temperature
+            self._mass_T = system.thermostat.mass
+        if system.barostat is not None:
+            self._P = system.barostat.pressure
+            self._mass_P = system.barostat.mass
+
+    def run(self, steps):
+        # Get variables
+        box = self.system.view('cell.side', dtype='float64')
+        pos = self.system.view('particle.position', dtype='float64', order='F')
+        vel = self.system.view('particle.velocity', dtype='float64', order='F')
+        ids = self.system.view('particle.species', dtype='int32')
+        rad = self.system.view('particle.radius', dtype='float64')
+        pos_unf = self.system.view('particle.position_unfolded', order='F')
+        # Masses have to be replicated along the spatial dimensions to keep the vector syntax
+        # The None indexing syntax adds a new dimension to the array
+        mas = self.system.view('particle.mass', dtype='float64')
+        mas = numpy.repeat(mas[:, numpy.newaxis], len(box), axis=1)
+        mas = numpy.transpose(mas, (1, 0))
+
+        # Compile module
+        f90 = f2py_jit.jit(_f90_kernel_soft)
+
+        # Main loop
+        for _ in range(steps):
+            f90.methods.evolve_velocity_verlet(1, self.timestep,
+                                               self.system.interaction.forces,
+                                               box, pos, pos_unf, vel,
+                                               ids, mas)
+            self.system.compute_interaction('forces')
+            f90.methods.evolve_velocity_verlet(2, self.timestep,
+                                               self.system.interaction.forces,
+                                               box, pos, pos_unf, vel,
+                                               ids, mas)
+            virial = self.system.virial(cache=True, per_particle=False)
+            f90.methods.rescale_berendsen(self._T, self._mass_T,
+                                          self._P, self._mass_P, box,
+                                          pos, vel, mas, virial)
```

## atooms/dynamics/stochastic.py

```diff
@@ -9,14 +9,16 @@
 import numpy
 import copy
 import logging
 
 from atooms.core.utils import Timer
 from .helpers import mean_square_displacement
 
+__all__ = ['LangevinOverdamped']
+
 _log = logging.getLogger(__name__)
 
 
 class LangevinOverdamped(object):
 
     def __init__(self, system, timestep=0.001, friction=1.0,
                  temperature=1.0, fixed_cm=True, random=None):
```

## Comparing `atooms_dynamics-1.0.0.dist-info/METADATA` & `atooms_dynamics-1.1.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: atooms-dynamics
-Version: 1.0.0
-Summary: UNKNOWN
+Version: 1.1.0
+Summary: Newtonian and stochastic dynamics backends for atooms
 Home-page: https://framagit.org/atooms/dynamics
 Author: Daniele Coslovich
 Author-email: daniele.coslovich@umontpellier.fr
 License: GPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: atooms-models (>=1.0.6)
-Requires-Dist: atooms (>=3.5.0)
+Requires-Dist: atooms (>=3.17.1)
 Requires-Dist: numpy
 
 # Dynamics
 
 [![pypi](https://img.shields.io/pypi/v/atooms-dynamics.svg)](https://pypi.python.org/pypi/atooms-dynamics/)
 [![version](https://img.shields.io/pypi/pyversions/atooms-dynamics.svg)](https://pypi.python.org/pypi/atooms-dynamics/)
 [![license](https://img.shields.io/pypi/l/atooms-pp.svg)](https://en.wikipedia.org/wiki/GNU_General_Public_License)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/git/https%3A%2F%2Fframagit.org%2Fatooms%2Fdynamics/HEAD?labpath=docs%2Findex.ipynb)
 [![pipeline](https://framagit.org/atooms/dynamics/badges/master/pipeline.svg)](https://framagit.org/atooms/dynamics/badges/master/pipeline.svg)
 [![coverage report](https://framagit.org/atooms/dynamics/badges/master/coverage.svg)](https://framagit.org/atooms/dynamics/-/commits/master)
 
-Netwonian and stochastic dynamics backends for atooms.
+Newtonian and stochastic dynamics backends for atooms.
 
 ## Quick start
 
 Run a molecular dynamics simulation of a Lennard-Jones system from an existing xyz file
 ```python
 from atooms.trajectory import Trajectory
 from atooms.simulation import Simulation
@@ -64,14 +65,15 @@
 ## Features
 
 Integration algorithms (work in progress)
 
 - Netwonian dynamics
   - velocity-Verlet
   - Nose-Poincaré
+  - Berendsen thermostat/barostat
   - event-driven
 - Stochastic dynamics
   - overdamped Langevin dynamics
 
 ## Documentation
 
 Check out the [tutorial](https://atooms.frama.io/dynamics/tutorial) for more examples and the [public API](https://atooms.frama.io/postprocessing/api/dynamics) for full details.
```

