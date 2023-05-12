# echopype examples

<div>
  <a href="https://doi.org/10.5281/zenodo.5618177">
    <img src="https://img.shields.io/badge/DOI-10.5281/zenodo.5618177-blue" alt="DOI">
  </a>

  <a href="https://raw.githubusercontent.com/OSOceanAcoustics/echopype-examples/main/LICENSE">
    <img alt="GitHub License" src="https://img.shields.io/github/license/OSOceanAcoustics/echopype-examples">
  </a>
</div>

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/OSOceanAcoustics/echopype-examples/main?labpath=notebooks/index.ipynb)

This repository illustrates the functionalities of [echopype](https://echopype.readthedocs.io/en/stable/), an open-source Python library that enables interoperability and scalability of water column sonar data processing. 
The materials are presented as [Jupyter notebooks](https://realpython.com/jupyter-notebook-introduction/) (`.ipynb` files) in the [notebooks](https://github.com/OSOceanAcoustics/echopype-examples/tree/main/notebooks) folder.
 
## View the notebook collection rendered as a JupyterBook
**Click [here](https://osoceanacoustics.github.io/echopype-examples/) to see the notebooks accurately rendered with a clean and convenient organization.**

## Run the notebooks in Binder
To actively explore and run the notebooks without downloading them or having to configure a Python environment locally, open them with [Binder](https://mybinder.org) either by clicking on the "launch binder" badge above to launch a sandbox copy or the "launch" icon (a rocket) on the upper right corner of each notebook in the JupyterBook. 

The typical Binder start time is about 3 minutes. Once Binder finishes spinning up, try running the first notebook. Below are a few things to bear in mind:
- The [index.md](https://github.com/OSOceanAcoustics/echopype-examples/blob/main/notebooks/index.md) file contains an index of the existing example notebooks with brief descriptions
- Currently, some notebooks may fail to run to completion in Binder due to memory demands that exceed what is available on Binder
- When you are done, just close the browser tab and the sandbox will be removed

## Run the notebooks locally on your machine
To run the notebooks locally in your computer, clone this repository (`git clone https://github.com/OSOceanAcoustics/echopype-examples.git`) and create a conda environment using the conda environment file [environment.yml](https://github.com/OSOceanAcoustics/echopype-examples/blob/main/binder/environment.yml) found in the `binder` folder:

```bash
conda env create -f environment.yml
```

This will create a new environment called `echopype.

## Set up a development environment to test and develop the notebooks and build the JupyterBook locally

First, clone this repository (see section above). Then, decide what kind of `echopype` environment you'd like to use.
### Use the latest echopype release
To test and develop notebooks using the latest echopype release:
- Follow the instructions above to create a conda environment.
- Activate the new environment. Assuming you used the default environment name: `conda activate echopype`
- Install `jupyter-book`: `conda install -c conda-forge jupyter-book`
### Use the current echopype development branch
To test and develop notebooks with the latest `echopype` development branch, go through the following steps:
- Install an [echopype development environment](https://echopype.readthedocs.io/en/stable/contributing.html#installation-for-echopype-development). First, run this conda create command (or better yet, use [`mamba`](https://mamba.readthedocs.io) instead of `conda`):
  ```bash
  conda create -c conda-forge -n echopype --yes python=3.9 --file https://raw.githubusercontent.com/OSOceanAcoustics/echopype/dev/requirements.txt --file https://raw.githubusercontent.com/OSOceanAcoustics/echopype/dev/requirements-dev.txt --file https://raw.githubusercontent.com/OSOceanAcoustics/echopype/dev/docs/requirements.txt
  ```
- Activate the new environment: `conda activate echopype`
- Install additional packages:
  ```bash
  conda install -c conda-forge geopandas cartopy datashader holoviews hvplot
  ```
- Run `pip install -e ".[plot]"`

### Building the JupyterBook locally
Regardless of which `echopype` environment you built:

- Activate the new `echopype` environment
- `cd` to your `echopype-examples` repository clone base folder, eg, `/path/to/clone/echopype-examples`
- Build the jupyter book: `jupyter-book build notebooks`
