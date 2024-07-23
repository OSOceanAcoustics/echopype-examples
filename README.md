# echopype-examples

[![Zenodo Badge](https://img.shields.io/badge/DOI-10.5281/zenodo.5618177-blue)](https://doi.org/10.5281/zenodo.5618177)
[![Jupyter Book Badge](https://jupyterbook.org/badge.svg)](https://tutorial.xarray.dev)
[![GitHub License](https://img.shields.io/github/license/OSOceanAcoustics/echopype-examples)](https://raw.githubusercontent.com/OSOceanAcoustics/echopype-examples/main/LICENSE)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/OSOceanAcoustics/echopype-examples/main?labpath=notebooks/index.ipynb)

This repository hosts demonstration examples for [Echopype](https://echopype.readthedocs.io/en/stable/), an open-source Python library that enables scalable and interoperabe water column sonar data processing. 

The examples are written as exectuable Jupyter Notebooks that you can easily run and modify on locally on your own machine or a cloud virtual machine.


## See all examples via JupyterBook
All notebooks are rendered at: https://osoceanacoustics.github.io/echopype-examples/


## Run the notebooks locally on your computer
If you want to run these notebooks on your local computer, follow the steps below:
- Clone and go into the repo
  ```shell
  # clone the repo
  git clone https://github.com/OSOceanAcoustics/echopype-examples.git

  # go into the repo folder
  cd echopype-examples
  ```
- Create a conda environment using the `environment.yml` file in the `conda` folder. We recommend using Mamba (see steps [here](https://github.com/conda-forge/miniforge#mambaforge) to install).
  ```shell
  # create an environment
  mamba env create -n echopype-examples -f conda/environment.yml

  # activate the environment
  conda activate echopype-examples
  ```
- Try out the notebooks in the `notebooks` folder!


## Run the notebooks on the cloud via Binder
You can run the notebooks directly on the cloud using Mybinder.org, by clicking the "launch binder" badge at the top of this page.

This will create a pre-configured JupyterLab with all the example notebooks under the `notebooks` folder. However, note that:
- It usually takes a few minutes to spin up Binder
- The computational resources are very minimal on Binder, so some example notebooks that handle many files may take a very long time or fail
- Any changes you make to the notebooks won't be saved permanently because Binder provides a temporary workspace


## Contribute to the example notebooks
Contributions are welcome and greatly appreciated!

The steps to set up a development environment is the same as the above. But:
- If you want to use the latest changes in the Echopype `main` branch, use `conda/environment-ep-main.yml` when creating the conda environment
- If you already have a functional Echopype development environment (see [here](https://echopype.readthedocs.io/en/stable/contributing.html#installation-for-echopype-development)) and want to use that, you can install additional packages needed for this repo by:
  ```shell
  conda install -c conda-forge geopandas cartopy datashader holoviews hvplot
  ```
  Note that it is often cleaner and easier to just create a new environment.


To build the JupyterBook locally:
```shell
# install jupyter book
conda install -c conda-forge jupyter-book

# go into the repo folder
cd echopype-examples

# build the jupyter book
jupyter-book build notebooks
```
