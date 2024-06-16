# echopype examples

[![Zenodo Badge](https://img.shields.io/badge/DOI-10.5281/zenodo.5618177-blue)](https://doi.org/10.5281/zenodo.5618177)
[![Jupyter Book Badge](https://jupyterbook.org/badge.svg)](https://tutorial.xarray.dev)
[![GitHub License](https://img.shields.io/github/license/OSOceanAcoustics/echopype-examples)](https://raw.githubusercontent.com/OSOceanAcoustics/echopype-examples/main/LICENSE)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/OSOceanAcoustics/echopype-examples/main?labpath=notebooks/index.ipynb)

This repository hosts demonstration examples for [Echopype](https://echopype.readthedocs.io/en/stable/), an open-source Python library that enables scalable and interoperabe water column sonar data processing. 

The examples are written as exectuable Jupyter Notebooks that you can easily run and modify on locally on your own machine or on the cloud.


### Quick glance via JupyterBook
You can take a quick glance of the example notebooks at: https://osoceanacoustics.github.io/echopype-examples/


### Run the notebooks locally on your own machine
If you want to run these notebooks on your own machine, we recommend the following steps:
- Clone and go into the repo
  ```shell
  # clone the repo
  git clone https://github.com/OSOceanAcoustics/echopype-examples.git

  # go into the repo folder
  cd echopype-examples
  ```
- Create a conda environment using the `environment.yml` file in the `conda` folder. We recommend using mamba (see steps [here](https://github.com/conda-forge/miniforge#mambaforge) to install).
  ```shell
  # create an environment
  mamba env create -n echopype-examples -f binder/environment.yml

  # activate the environment
  conda activate echopype-examples
  ```
- Try out the notebooks in the `notebooks` folder!


### Run the notebooks on the cloud via Binder
You can run the notebooks directly on the cloud using Mybinder.org, by:
- clicking the "launch binder" bdage at the top of this page, or
- clicking the "launch" icon (a rocket) on the upper right corner of each notebook in the JupyterBook

This will create a pre-configured JupyterLab with all the example notebooks under the `notebooks` folder. However, note that:
- It usually takes a few minutes to spin up the Binder
- The computational resources are very minimal on Binder, so the notebooks that handle many files may take very long or fail
- Any changes you make will not be saved


### Contribute to the example notebooks!
If you are interested in improving the existing notebooks or contributing new ones, awesome!

The steps to set up a development environment is the same as the above. But: - If you want to use the latest changes in the Echopype repo, use `environment-ep-main.yml` when creating the conda environment
- If you already have a functional Echopype development environment (see [here](https://echopype.readthedocs.io/en/stable/contributing.html#installation-for-echopype-development)) and want to use that, you can install additional packages needed for this repo by:
  ```
  conda install -c conda-forge geopandas cartopy datashader holoviews hvplot
  ```

To build the JupyterBook locally:
```shell
# install jupyter book
conda install -c conda-forge jupyter-book

# go into the repo folder
cd echopype-examples

# build the jupyter book
jupyter-book build notebooks
```
