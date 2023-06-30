### Nice steps to process raw files using EK60

Example of basic echopype processing of EK60 files by Ruxandra in this -> [GitHub repository](https://github.com/OceanStreamIO/echopype-scratchpad/blob/main/echopype-scratchpad/one_off_notebook/Basic%20echopype%20processing%20of%20EK60%20files.ipynb).

**Main echopype workflow steps - for each raw file:**

- **Access** file directly from S3 via `ep.open_raw()` to create a converted EchoData object in memory
- **Add global and platform attributes** to EchoData object
- **Export** to a local Zarr dataset 
- **Processing** - Sv computation and denoising:
    - Before computing the volume backscattering strength (Sv) using `ep.calibrate.compute_Sv()` in echopype, it is essential to identify the waveform mode, as additional parameters need to be set specifically for Broadband (BB) mode.
    - Compute base Sv -> `ep.calibrate.compute_Sv()` -> (`import echopype as ep`)
    - Remove background noise -> `ep.preprocess.remove_noise()`
- Reduce data by computing Mean Volume Backscattering Strength (MVBS) -> `ep.preprocess.compute_MVBS()`
    - MVBS or cleaned Sv can be exported  to a local netcdf file
    - `xr.open_mfdataset()` -> (`import xarray as xr`) is used to open multiple netCDF files as a single xarray dataset
- Test for time reversals - a quality control test designed to identify instances in the echo sounder data where timestamps might be out of order -> See an example in the -> [GitHub repository](https://github.com/OSOceanAcoustics/echopype-examples/blob/main/notebooks/ms_PacificHake_EK60_cruisetracks.ipynb)
- Visualising echogram-> `epviz.create_echogram()` -> (`import echopype.visualize as epviz`)
- Particular example - Search for krill by creating a mask that keeps points with an Sv difference of 2-16 dB between the 120 kHz and 38 kHz channels.

A detailed walkthrough for EK60 data processing can be find also in the example by Raluca in this GitHub repository -> [GitHub repository](https://github.com/OceanStreamIO/echopype-scratchpad/blob/main/echopype-scratchpad/one_off_notebook/echopype_tour.ipynb)
