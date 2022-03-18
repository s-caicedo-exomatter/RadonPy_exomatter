<p align="center">
  <img height="250" src="https://github.com/RadonPy/RadonPy/blob/main/logo.png" alt="radonpy">
</p>

## Overview
RadonPy is the first open-source Python library for fully automated calculation for a comprehensive set of polymer properties, using all-atom classical MD simulations. For a given polymer repeating unit with its chemical structure, the entire process of the MD simulation can be carried out fully automatically, including molecular modelling, equilibrium and non-equilibrium MD simulations, automatic determination of the completion of equilibration, scheduling of restarts in case of failure to converge, and property calculations in the post-process step. In this first release, the library comprises the calculation of 15 properties, such as thermal conductivity, density, specific heat capacity, thermal expansion coefficient, refractive index, and so on, at the amorphous state.

## Requirement
- Python 3.7, 3.8, 3.9
- LAMMPS >= 3Mar20
- rdkit >= 2020.03
- psi4 >= 1.5
- resp
- dftd3
- mdtraj >= 1.9
- scipy
- matplotlib

## Installation and Usage

## Features
- Fully automated all-atom classical MD calculation for polymeric materials
	- Conformation search
	- RESP cherge calculation
	- Electronic property calculation (HOMO, LUMO, dipole moment, polarizability)
	- Generator of a polymer chain
	- Generator of a simulation cell
	- Run for equilibration MD
	- Checking archivement of equilibrium
	- Run for non-equilibrium MD (NEMD)
	- Calculation of physical properties from the MD calculation results
	- Using LAMMPS and Psi4 as calculation engines of MD and DFT calculations
- Implementation of presets to allow for proper and easy execution of polymer MD calculations
	- Equilibration MD
	- Calculation of thermal conductivity with NEMD
- Easy installation
    - Only using open-source software
- Tools for polymer informatics
	- Force field descriptor
	- Generator of macrocyclic oligomer for descriptor construction of polymers
	- Full and substruct match function for polymer SMILES
	- Extractor of mainchain in a polymer backbone
	- Monomerization of oligomer SMILES
	- Emulator of polymer classification in PoLyInfo

## Publications
1. Y. Hayashi, J. Shiomi, J. Morikawa, R. Yoshida, "RadonPy: Automated Physical Property Calculation using All-atom Classical Molecular Dynamics Simulations for Polymer Informatics," arXiv

## Contributors
- Yoshihiro Hayashi (The Institute of Statistical Mathematics)

## Copyright and licence
©Copyright 2022 The RadonPy project, all rights reserved.
Released under the `BSD-3 license`.


![Radon_ikaho](https://user-images.githubusercontent.com/83273612/158885745-224f6e7a-4b1d-46f4-b5c6-80455827c904.png)

