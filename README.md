# Computational Systems Biology

## anaconda environments installation

`CSB1` used for L1

```sh
conda create --name CSB1 -c conda-forge python jupyterlab matplotlib pandas numpy biopython nglview
```

`CSB2` used for all others but L7

```sh
conda create --name CSB2 -c conda-forge python jupyterlab matplotlib pandas numpy scipy
```

`CSB3` used for L7

```sh
conda create --name CSB3 -c conda-forge python jupyterlab matplotlib pandas numpy=1.23.3 scipy cobra
```

`CSB99` used for `L99_with_mn` (a wip/abandoned version of L99 final project)

```sh
conda create --name CSB99 -c conda-forge python jupyterlab matplotlib pandas numpy scipy manim
```

###### possibly need to `conda install python=3.1` to install `manim`

## how to run

```sh
# cd into respective lab nb directory
conda activate CSB2 # or CSB3 for L07
jupyter lab

conda deactivate # to exit the conda env
```
