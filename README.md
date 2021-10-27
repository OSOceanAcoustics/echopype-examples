# echopype-examples

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/OSOceanAcoustics/echopype-examples/master)

## Purpose

This repository illustrates the functionalities of [echopype](https://echopype.readthedocs.io/en/stable/), an open-source Python library that enables interoperability and scalability in water column sonar data analysis. The materials can be found within the [notebooks](https://github.com/OSOceanAcoustics/echopype-examples/tree/main/notebooks) folder in `.ipynb` files, which are [Jupyter notebooks](https://realpython.com/jupyter-notebook-introduction/). Open the [index.ipynb](https://github.com/OSOceanAcoustics/echopype-examples/blob/main/notebooks/index.ipynb) notebook to see an index of the existing example notebooks. To see the notebooks accurately rendered (GitHub notebook rendering has shortcomings), [open the index notebook in https://nbviewer.org](https://nbviewer.org/github/OSOceanAcoustics/echopype-examples/blob/main/notebooks/index.ipynb).

To actively explore and run the notebooks without downloading them or having to configure a Python environment locally, open them with https://mybinder.org:
- Click on the "launch binder" badge above to launch a sandbox copy. The typical start time is about 3 minutes. 
- Once binder finishes spinning up, try running the first notebook. Currently, some notebooks may fail to run to completion in binder due to memory demands that exceed what is available on binder.
- When you are done, just close the browser tab and the sandbox will be removed.

To run the notebooks locally in your computer, clone this repository and create a conda environment using the conda environment file [environment.yml](https://github.com/OSOceanAcoustics/echopype-examples/blob/main/binder/environment.yml) found in the `binder` folder:
```bash
conda env create -f environment.yml
```
