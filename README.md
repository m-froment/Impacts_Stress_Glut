# Impacts_Stress_Glut

***
### Dataset for article: Numerical Modelling of Impact Seismic Sources Using the Stress Glut Theory
### Froment M., Lognonné P., Larmat C., Lei Z., Rougier E. and Kawamura T. 
Uploaded in March 2023
***

This dataset contains material models, geometries and simulation parameters used for the simulations presented in the work "Numerical Modelling of Impact Seismic Sources Using the Stress Glut Theory" by Froment M., Lognonné P., Larmat C., Lei Z., Rougier E. and Kawamura T..

Simulations are run with the Hybrid Optimization Software Suite (HOSS) (https://www.lanl.gov/orgs/ees/hoss/index.shtml) and with the SPECFEM3D software (https://specfem.org/).

### HOSS 
Description of the files:

* geo_vertical.jou : CUBIT journal file for generating a 45 degrees cylindrical sector for the simulation of vertical impacts.
* geo_oblique.jou : CUBIT journal file for generating a 180 degrees cylindrical sector for the simulation of oblique impacts.
* initial_and_boundary_conditions.txt : Simulation parameters, boundary and initial conditions used to run oblique and vertical impact simulations.
* EOS.txt : Curves and parameters defining the Equation of State of the target material (GROUND).
* EOS_i.txt : Parameters defining the Tillotson Equation of State of the impactor material (IMPACTOR).
* H7H.txt : Curves and parameters defining the strength of the target material (GROUND).
* H7H_i.txt : Curves and parameters defining the strength of the impactor material (GROUND).

### SPECFEM3D
Description of the files:

* Mesh_Par_File : Parameter file for the generation of the cartesian mesh.
* interfaces.dat : File defining the layering of the SPECFEM3D geometry.
* interface_top.dat : File defining the topography of the top surface.
* SPECFEM_input_parameters.txt : Various parameters used in SPECFEM3D's main parameter file, Par_File.
* FORCESOLUTION_X : Parameter file defining a impulsive horizontal force source.
* FORCESOLUTION_Z : Parameter file defining a impulsive vertical force source.
* triangle_source.dat : Source time function of the impulsive force.
* CMTSOLUTION_MXX, CMTSOLUTION_MYY, CMTSOLUTION_MZZ, CMTSOLUTION_MZX : Parameter files defining the four Moment Tensor sources necessary to simulate the impact seismic signal of an oblique or vertical impact. Their source time function is a Heaviside.
