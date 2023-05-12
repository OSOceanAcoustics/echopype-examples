# Echopype examples notebooks

Jupyter notebooks demonstrating [echopype](https://echopype.readthedocs.io) capabilities and usage.

- [echopype_tour.ipynb](echopype_tour.ipynb). A quick tour of core echopype capabilities.
- [ms_PacificHake_EK60_cruisetracks.ipynb](ms_PacificHake_EK60_cruisetracks.ipynb). Exploring ship echosounder data from the Pacific Hake survey. Goals:
    1. Illustrate a common workflow for echosounder data conversion, calibration and use.
    2. Extract and visualize echosounder data (EK60) with relative ease using geospatial and temporal filters. 
- [ms_OOI_EK60_mooringtimeseries.ipynb](ms_OOI_EK60_mooringtimeseries.ipynb). Wacthing a solar eclipse using an OOI moored echosounder. Goals:
    1. Illustrate a common workflow for echosounder data conversion, calibration and use.
    2. Demonstrate the ease to interoperate echosounder data (EK60) with those from a different instrument in a single computing environment. Without echopype, additional wrangling across more than one software systems is needed to achieve the same visualization and comparison.

## Running the notebooks

The notebooks in this site can be run with a [conda](https://docs.conda.io) environment created using the [instructions in the repository README.md](https://github.com/OSOceanAcoustics/echopype-examples#run-the-notebooks-locally-on-your-machine).

To actively explore and run the notebooks without downloading them or having to configure a Python environment locally, open them with https://mybinder.org to launch a sandbox copy via the "launch" icon (a rocket) on each notebook in this site, in the upper right. The typical start time is about 3 minutes. Once binder finishes spinning up, try running the first notebook. Currently, some notebooks may fail to run to completion in binder due to memory demands that exceed what is available on binder. When you are done, just close the browser tab and the sandbox will be removed.

Please see the last cell in each notebook to see which version of echopype and dependencies the notebook was last run with.
