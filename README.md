# Orbit-Propagator-with-Perturbations
High Precision Orbit Propagator for LEO satellites with perturbations and also including thrust
Orbit_Propagator_with_Perturbations
1-)Download the zip file in to your computer and extract it.
2-)Apply "Add to path---->Selected folders" for all folder in the zip.
3-)Check the "EOP.txt"(Earth Orientation Parameters) and "SW.txt"(Space Weather).Change them accordingly to your epoch and propagation time.
(https://celestrak.com/SpaceData/) In the code year of 2015 datas are used.
4-)Open "test_orbitpropagator.m"
5-)Read the comments and notes carefully.
6-)Enter the inputs with the following;
if input.THRUSTER='OFF',neccesary inputs are
forces,input.position,input.velocity,input.timestep,input.datetime,input.eop,input.sw,input.atmosmodel,input.F107,input.F107A,input.magnetindex
input.drymass,input.cd,input.dragarea,input.propagationtime1
if input.THRUSTER='ON',neccesary inputs are
forces,input.position,input.velocity,input.timestep,input.datetime,input.eop,input.sw,input.atmosmodel,input.F107,input.F107A,input.magnetindex
input.drymass,input.cd,input.dragarea,Tforces,input.fuelmass,input.thrustmag,input.thrustduration,input.thrusttimestep,input.beforethrust
input.afterthrust,input.propagationtime2
7-)Run the code.
8-)Outputs are seen in the workspace as an "out" struct and also 3D orbit is shown. 
