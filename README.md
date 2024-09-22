This project focuses on reconstructing the three-dimensional structure of chromatin from Hi-C contact maps using a Bead-Spring Polymer model.

Workflow
Data File Creation:

Python Script 1 (straightchain.ipynb): Generates an initial straight-polymer chain, saving the molecule's starting coordinates.
Python Script 2 (contact_frequency_to_contact_probability.ipynb): Uses the Hi-C contact matrix data to create bond information, which is then used for generating input files for LAMMPS simulations.

Coarse-grain bead-spring simulation:

The LAMMPS input (in.main_2) and data files (data_nonoverlap_2.cfg) are used to simulate the chromatin's three-dimensional structure based on the given 2D Hi-C contact map.
