# SourceTracker2 with Diagnostics:
This is a python package that contains the original functions of sourcetracker (owned by Biota) as well as the added utility of the diagnostic function. This repo is used as a "All-in-one" back up package to the original. It is designed to be installed natively on users device.

For more information on SourceTracker2 please go to Biota github: 
https://github.com/biota/sourcetracker2

# Installation
```
conda create -n st2 -c biocore python=3.5 numpy scipy scikit-bio biom-format h5py hdf5 seaborn parso=0.1.1
conda activate st2
pip install --upgrade pip
pip install git+https://github.com/residentjordan/SourceTracker2-diagnostics.git@Update
```
# Verifying Installation
```sourcetracker2 gibbs -h```

# Example:
```sourcetracker2 gibbs -i OTU.txt -m map.txt -o output/ --diagnostics --draws_per_restart 2```
