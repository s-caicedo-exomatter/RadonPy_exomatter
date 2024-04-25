Fists create a conda environment:

```shell
conda install conda-build
conda create -n radonpy2 python=3.11
conda activate radonpy2
```

Add channels if necessary:
```shell
conda config --add channels conda-forge
```

Install requirements, including `rdkit` and `LAMMPS`. One that is not really specified in the github site is `dftd3`, but for the tutorial was necessary, so it is safer to install it:
```shell
conda install -c conda-forge/label/libint_dev -c conda-forge -c psi4 rdkit resp dftd3-python mdtraj matplotlib xtb-python openbabel ase lammps
```

We can clone the forked `radonpy` repository and include it in the conda installation in development mode using:
1. **Conda-develop:**
```shell
conda deactivate
conda-develop <path to cloned Radonpy_exomatter git repo> -n radonpy2
```
2. **PiP:** This one needs a `setup.py` file, which is provided by radonpy
```shell
conda activate radonpy2
pip install -e <path to cloned Radonpy_exomatter git repo>
```
