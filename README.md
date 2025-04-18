# Computational Systems Biology

## anaconda environments installation

`CSB1` used for L1
conda create --name CSB1 -c conda-forge python jupyterlab matplotlib pandas numpy biopython nglview

`CSB2` used for all others but L7
conda create --name CSB2 -c conda-forge python jupyterlab matplotlib pandas numpy scipy

`CSB3` used for L7
conda create --name CSB3 -c conda-forge python jupyterlab matplotlib pandas numpy=1.23.3 scipy cobra

## how to run

```sh
# cd into respective lab nb directory
conda activate CSB2 # or CSB3 for L07
jupyter lab

conda deactivate # to exit the conda env
```
