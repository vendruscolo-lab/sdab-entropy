Conformational Entropy as a Potential Liability of Computationally Designed Antibodies
======================================================================================

This repository contains the full analysis code to reproduce our results on the conformational landscape of designed single-domain antibodies, [published in Biomolecules](https://www.mdpi.com/2218-273X/12/5/718).

Reproducibility information
---------------------------
Simulations were run using GROMACS 2019.3 and PLUMED 2.6 (git commit 8859093) with 32 replicas. Analysis was performed in a Jupyter notebook using python 3.7.6, numpy 1.18.1 and mdtraj 1.9.3.

Dataset
-------
The full dataset including trajectories can be found on Zenodo. It includes the following data:

- `simulations/`: Gromacs `tpr` runtime files and PLUMED input
- `trajectories/`: `xtc` trajectories, deposited Gaussian hills, PLUMED post-processing script and computed total bias (to calculate the per-frame weight)
- `analysis/`: The analysis notebook `ana.ipynb`, template folder structures for the clustering procedure, and structures sampled from the trajectories and clusters
