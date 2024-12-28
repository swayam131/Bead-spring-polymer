Reconstructing Chromatin 3D Structure and Modeling Gene Expression

Overview

This project aims to reconstruct the three-dimensional structure of chromatin from HiC contact maps using a Coarse-grain Bead-Spring Polymer model. Additionally, it determines gene expression levels based on the binding and unbinding rates of Enhancer-Promoter (E-P) interactions derived from the 3D chromatin conformation, utilizing a kinetic model.
## Getting Started

### Prerequisites
- [LAMMPS](https://lammps.org) installed for simulations.
- [MATLAB R2022a](https://www.mathworks.com/products/matlab.html) for the kinetic model.

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/ss131/Bead-spring-polymer.git

Workflow

1. Coarse-Grain Bead-Spring Polymer Model

The Bead-Spring Polymer model simulates the chromatin structure for the 6MB Sox9-Kcnj2 loci of the mESC wildtype cell line. This is achieved using the LAMMPS simulation package.

Key Files:

in.run: Input file for LAMMPS simulations.

poly.data: Data file containing simulation parameters and chromatin configurations.

Running the Simulation:

To execute the LAMMPS simulation, use the following command:

lmp_serial -in in.run > log &

This command initiates the simulation and redirects the output to the log file for monitoring.

2. Kinetic Model

The kinetic model calculates gene expression levels by modeling the rates of binding and unbinding interactions between enhancers and promoters, as derived from the 3D chromatin structure.

Key File:

Kinetic_model_sox9_wildtype: MATLAB script implementing the kinetic model.

Running the Kinetic Model:

This script is developed in MATLAB R2022a. It can be executed either through the MATLAB GUI or via the command line prompt.

Command Line Execution:

Open the terminal.

Navigate to the directory containing the script.

Run the script using the following command:

matlab -nodisplay -nosplash -r "run('Kinetic_model_sox9_wildtype'); exit;"

Notes

Ensure LAMMPS and MATLAB are installed and properly configured on your system before running the simulations and kinetic model.

For any issues or inquiries, refer to the documentation or contact the project administrator.
