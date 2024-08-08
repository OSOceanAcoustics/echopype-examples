# Echopype examples notebooks

Jupyter notebooks demonstrating [Echopype](https://echopype.readthedocs.io) capabilities and usage.

- [OOI_eclipse.ipynb](OOI_eclipse.ipynb) - *Not Binder Friendly*. Pairing acoustic data from an upward-looking echosounder and shortwave irradiance measured by a pyrometer on a surface mooring to observe the movement response of zooplankton to a solar eclipse. 
- [ship_tracks.ipynb](ship_tracks.ipynb) - *Not Binder Friendly*. Subselect sections of echo data based on ship GPS data embedded in the echosounder raw files to demonstrate the power of label-aware data processing based on standardized netCDF data model.
- [krill_freq_diff.ipynb](krill_freq_diff.ipynb) - *Not Binder Friendly*. Perform frequency-differencing analysis to identify fluid-like zooplankton scatterers (likely krill) in ship echosounder data, and compute nautical acoustic scattering coefficient (NASC) based on the classification.
- [hake_mask.ipynb](hake_mask.ipynb) - *Binder Friendly*. Organize and apply externally generated masks that identify the occurrence of Pacific hake in ship echosounder data, and compute NASC based on the masked outputs.
- [glider_AZFP.ipynb](glider_AZFP.ipynb) - *Binder Friendly*. Process acoustic data from a Slocum glider by incorporating external position, motion, and environmental data and identify zooplankton shoals.

## Running the notebooks

The notebooks in this site can be run locally with a [conda](https://docs.conda.io) environment created following the [instructions in the repository README.md](https://github.com/OSOceanAcoustics/echopype-examples#run-the-notebooks-locally-on-your-machine).

If you want to try these notebooks on Binder, follow instructions [here](https://github.com/OSOceanAcoustics/echopype-examples#run-the-notebooks-on-the-cloud-via-binder). However, due to the limited resources on Binder, the execution of some notebooks may fail.

Please see the last cell in each notebook to see the version of Echopype and important dependencies the notebook was last run with.
