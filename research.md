# Computational Fluid Dynamics Research @ Georgia Tech

Highlights:
- 7 geometries modeled and analyzed on ANSYS Fluent
- Determmined pressure and velocity profiles across wings and airfoils
- Experience with mesh creation, setup troubleshooting, and results analysis

## CFD Analysis of Symmetric Airfoil w/ Parametric Sweep of AoA
Case study of the aerodynamic behavior of a NACA0012 airfoil at an airspeed of Mach 0.7. The flow was computed at angles of attack of 0, 1, 2, 3, 4, & 5. With the objective of understanding the relationship between change in angle of attack and change in flow behavior.

_Methodology_
* Geometry: NACA 0012
* Solver: SST k-omega
* Mesh: 36800 cells
* Boundary Conditions: Inlet Mach - 0.7  Inlet Pressure - 1000 Pa
* Assumptions: Steady, Inviscid, and Incompressible

<img src="assets/images/cfd_pressure.png" width="600">

<img src="assets/images/streamlines.png" width="600">

_Results_
The pressure and mach distributions over the airfoil demonstrate the principles of lift as well as the propagation of the boundary layer along the surface.
