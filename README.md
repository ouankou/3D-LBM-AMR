# 3D-LBM-AMR
3D LBM code with adaptive mesh refinement

DESCRIPTION OF APPLICATION
--------------------------

Solves the 3D incompressible Navier-Stokes equations using the lattice Boltzmann method. The data structure allows for adapative local mesh refinements during the transient simulation.

![Alt text](3D LBM AMR/AMR.png?raw=true "Vorticity based refinement on 2D cylinder case")

![Alt text](3D LBM AMR/AMR2.png?raw=true "Vorticity based refinement on 2D cylinder case")

# Build

```bash
cd src
g++-10 -L/usr/lib/gcc/x86_64-linux-gnu/10 -lgomp -fopenmp -lpthread -foffload=nvptx-none Node.cpp Source.cpp -o amr.out
```
