# echopype examples

<div>
  <a href="https://doi.org/10.5281/zenodo.5618177">
    <img src="https://img.shields.io/badge/DOI-10.5281/zenodo.5618177-blue" alt="DOI">
  </a>

  <a href="https://raw.githubusercontent.com/OSOceanAcoustics/echopype-examples/main/LICENSE">
    <img alt="GitHub License" src="https://img.shields.io/github/license/OSOceanAcoustics/echopype-examples">
  </a>
</div>

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/OSOceanAcoustics/echopype-examples/HEAD?labpath=https%3A%2F%2Fgithub.com%2FOSOceanAcoustics%2Fechopype-examples%2Fblob%2Fmain%2Fnotebooks%2Findex.ipynb)

This repository illustrates the functionalities of [echopype](https://echopype.readthedocs.io/en/stable/), an open-source Python library that enables interoperability and scalability of water column sonar data processing. 
The materials can be found within the [notebooks](https://github.com/OSOceanAcoustics/echopype-examples/tree/main/notebooks) folder in `.ipynb` files, which are [Jupyter notebooks](https://realpython.com/jupyter-notebook-introduction/). 
Open the [index.ipynb](https://github.com/OSOceanAcoustics/echopype-examples/blob/main/notebooks/index.ipynb) notebook to see an index of the existing example notebooks. 
To see the notebooks accurately rendered (GitHub notebook rendering has shortcomings), [open the index notebook at https://nbviewer.org](https://nbviewer.org/github/OSOceanAcoustics/echopype-examples/blob/main/notebooks/index.ipynb).

To actively explore and run the notebooks without downloading them or having to configure a Python environment locally, open them with https://mybinder.org:
- Click on the "launch binder" badge above to launch a sandbox copy. The typical start time is about 3 minutes. 
- Once binder finishes spinning up, try running the first notebook. Currently, some notebooks may fail to run to completion in binder due to memory demands that exceed what is available on binder.
- When you are done, just close the browser tab and the sandbox will be removed.

To run the notebooks locally in your computer, clone this repository and create a conda environment using the conda environment file [environment.yml](https://github.com/OSOceanAcoustics/echopype-examples/blob/main/binder/environment.yml) found in the `binder` folder:

```bash
conda env create -f environment.yml
```
