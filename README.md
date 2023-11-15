# SPDFEM User Guide

Welcome to the SPDFEM (Simulation of Photonic Devices using Finite Element Method) package! This package enables you to simulate and analyze photonic devices using the Finite Element Method. This README file provides you with essential information on how to use the package effectively.

## Problem Statement
For an understanding of the problem that this software addresses, please refer to the [Problem Statement document](https://github.com/shmouses/SPDFM/blob/master/docs/ProblemStatement/ProblemStatement.pdf).

## System Requirement Specification (SRS)
To delve into the theoretical background and system requirements, consult the [SRS document](https://github.com/shmouses/SPDFM/blob/master/docs/SRS/SRS.pdf).

## Validation and Verification (V&V)
The validation and verification plan and report can be found respectively at:
- [Validation and Verification Plan](https://github.com/shmouses/SPDFM/blob/master/docs/VnVPlan/VnVPlan.pdf)
- [Validation and Verification Report](https://github.com/shmouses/SPDFM/blob/master/docs/VnV%20Report/VnV%20Report.pdf)

## Modular Design
Explore the modular design of the software in the [Design directory](https://github.com/shmouses/SPDFM/blob/master/docs/Design).

## Tutorial Jupyter Notebook
For newcomers to SPDFM, we highly recommend following the tutorial provided in the [Tutorial Jupyter notebook](https://github.com/shmouses/SPDFM/blob/master/src/SPDFM%20Tutorial%20.ipynb).

## System Requirements
Before running SPDFM, ensure that the following libraries are installed on your system:
- fenics 2019 1.0
- matplotlib
- numpy
- math
- time
- scipy

Please note that SPDFM is built upon the fenics toolbox and should be executed on a system running a Linux OS.

## Running a Simulation
To initiate a simulation using SPDFM, follow these steps:

1. Download or clone the `src` folder to your local system.
2. Run `main.py`.
3. You'll be prompted to provide a path to an input file containing material properties and light source illumination details. If the `src` folder is copied, you can use: `Input/Input_t1.txt`.
4. You'll be asked to provide the path to the `.xml` mesh file. Ensure that the mesh is readable by the Dolfin toolbox, which is embedded in Fenics. Example input: `Mesh/G_fill_t1.xml`.
5. Provide the path to the file indicating physical regions in the mesh. Example input: `Mesh/G_fill_pr_t1.xml`.
6. Similarly, provide the path to the file containing facet region information for the mesh. Example input: `Mesh/G_fill_fc_t1.xml`.
7. SPDFM will now perform calculations and save the real and imaginary parts of the electric field and electric current density in `.pvd` and `.vtk` files in the "FEM Output" directory.

## Testing
For testing specific parts of the code, you can execute `.py` files that start with "test_". To run `test_constparam.py` and `test_inputparam.py`, you should use the `pytest` library in Python.

For any issues, inquiries, or contributions, please feel free to contact the authors of the repository.

Happy simulating with SPDFEM!
