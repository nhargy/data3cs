# data3cs
Data repository of the 3CS experimental setup.

** Download a specific directory from this repo using its url at: **https://download-directory.github.io/

Slack integration is active@3CS channel.


## Structure

Every study is broken down into several collection directories (and possibly sub-collections) inside which are HDF5 files relating to one sample are contained.
The contents of the collections are given in the 'STUDY.md' file, and names of the HDF5 files will usually be the code of the sample crystal they refere to (e.g. 'LiF_B2_141.hdf5').

### HDF5 Internal Structure

**Super groups:**
1. 'spectra' : data from sample exposures
2. 'system' : metadata of experimental setup, power correlation measurements
3. 'log' : sytem log

**'spectra'**
Groups: wavelength => orientation => exposure time (e.g. '400' => '0' => '10.0sec')
The datasets available are:
1. 'sp_data' : matrix of spectrum data
2. 'bg_data' : matrix of background data
3. 'powers' : array of power samples for sp_data
