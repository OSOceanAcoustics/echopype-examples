# Echopype examples notebooks

Jupyter notebooks demonstrating [echopype](https://echopype.readthedocs.io) capabilities and usage.


- [glider_AZFP.ipynb](glider_AZFP.ipynb) - *Binder Friendly*. Integrating External Glider Data and AZFP Data to Identify Zooplankton Shoals. Goals:
    1. Integrate environmental calibration parameters, motion data, and location information from external glider data into Echopype-processed AZFP data to calibrate backscatter data and improve spatial referencing.
    2. Identify Zooplankton Shoals using external Fisheries Acoustics on Echopype calibrated backscatter data.
- [hake_NASC.ipynb](hake_NASC.ipynb) - *Binder Friendly*. Computing Biomass-proxy of Pacific Hake. Goals:
    1. Illustrate a common workflow for echosounder data conversion, calibration, regridding, masking, and NASC computation.
    2. Demonstrate the ease of interfacing biological and seabed annotations with Echopype backscatter data using Echoregions.
- [krill_NASC.ipynb](krill_NASC.ipynb) - *Not Binder Friendly*. Computing Biomass-proxy of Pacific Hake. Goals:
    1. Illustrate a common workflow for echosounder data conversion, calibration, regridding, frequency differencing, and NASC computation.
    2. Demonstrate that Echopype efficiently scales customizable processing routines for large, multi-day datasets through seamless Dask integration.
- [OOI_eclipse.ipynb](OOI_eclipse.ipynb) - *Not Binder Friendly*. Watching a solar eclipse using an OOI moored echosounder. Goals:
    1. Illustrate a common workflow for echosounder data conversion, calibration and use.
    2. Demonstrate the ease to interoperate echosounder data (EK60) with those from a different instrument in a single computing environment. Without Echopype, additional wrangling across more than one software systems is needed to achieve the same visualization and comparison.
- [ship_track.ipynb](ship_track.ipynb) - *Not Binder Friendly*. Exploring ship echosounder data from the Pacific Hake survey. Goals:
    1. Illustrate a common workflow for echosounder data conversion, calibration and use.
    2. Extract and visualize echosounder data (EK60) with relative ease using geospatial and temporal filters. 


## Running the notebooks

The notebooks in this site can be run with a [conda](https://docs.conda.io) environment created using the [instructions in the repository README.md](https://github.com/OSOceanAcoustics/echopype-examples#run-the-notebooks-locally-on-your-machine).

To actively explore and run the notebooks without downloading them or having to configure a Python environment locally, open them with https://mybinder.org to launch a sandbox copy via the "launch" icon (a rocket) on each notebook in this site, in the upper right. The typical start time is about 3 minutes. Once binder finishes spinning up, try running the first notebook. Currently, some notebooks may fail to run to completion in binder due to memory demands that exceed what is available on binder. When you are done, just close the browser tab and the sandbox will be removed.

Please see the last cell in each notebook to see which version of echopype and dependencies the notebook was last run with.
