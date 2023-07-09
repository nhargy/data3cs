# data3cs
Data repository of the 3CS experimental setup.

** Download a specific directory from this repo using its url at: **https://download-directory.github.io/

Slack integration is active@3CS channel.


## Structure

Every study is broken down into several collection directories (and possibly sub-collections) inside which are HDF5 files relating to one sample are contained.
The contents of the collections are given in the 'STUDY.md' file, and names of the HDF5 files will usually be the code of the sample crystal they refere to (e.g. 'LiF_B2_141.hdf5').

### HDF5 Internal Structure

'sample_scan.hdf5' <br />
| <br />
| <br />
|_________________ 'spectra' <br />
|                | <br />
|                | <br />
|                |______________ '400' <br />
|                             | <br />
|                             |___________ '1.0sec' <br />
|                                       | <br />
|                                       |_______ 'sp_data' <br />
|                                       | <br />
|                                       |_______ 'bg_data' <br />
|                                       | <br />
|                                       |_______ 'powers' <br />
|                
|                
| <br />
| <br />
| <br />
|_________________ 'system' <br />
| <br />
| <br />
| <br />
|__________________ 'log' <br />
