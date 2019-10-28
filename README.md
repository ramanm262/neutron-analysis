# neutron-analysis
Code used for preparation and analysis of neutron monitor data. No method in this repository definitively provides evidence of neutron precursor signals or impulsive event solar neutron signals. But feel free to check for yourself.

## Instructions for use

First, run GOES_access_data.ipynb to obtain an easy-to-read (for the computer) table of SEP-producing flare data from GOES.
Next, run both functions in NMDB_access_data.ipynb. For each of the two functions, put all downloaded files from that function into a unique directory. This should give you two directories: one for GLE-based neutron data and one for X-ray-flare-based neutron data.
Then, run whatever analyses you like.

#### Principal component analysis
Run NMDB_PCA.ipynb. This requires GLE-based data from NMDB_access_data.ipynb.

#### Autocorrelation analysis
Run NMDB_autocorrelationn.ipynb. This requires either GLE-based data or flare-based data.

#### Superposed epoch analysis
Run NMDB_SEA.ipynb. This requires flare-based data from NMDB_access_data.ipynb and flare timing data from GOES_access_data.ipynb.
