The files in this directory were downloaded from the datashader
repository at https://github.com/bokeh/datashader . The license
described in ../datashader_LICENSE.txt applies.

To run the census dashboard, use

python dashboard.py -c census.yml -o

where the -o denotes "out of core", meaning do not load all the data into memory.

The files have been slightly modified to work with the data in 
HDF5 format. The data are available here: https://caltech.box.com/s/ts15q85qlde76rzt993tng2dvw7chntl
