
## Installation of Python modules (from previous class)

If you don't have Anaconda or Miniconda, go to http://conda.pydata.org/miniconda.html and install the Python 3.5 64-bit version for your system. 

Make sure you've added the `bin` directory for Miniconda to your `PATH`. Then in a terminal window, execute this command:
```
conda create -n course python=3.5 astropy pandas seaborn glueviz jupyter pillow statsmodels
```
This creates a virtual environment named `course`. You can list your environments with `conda info -e`.

### Activate the virtual environment

For further conda installs to work, you must use a bash shell.
Then execute:
```
source activate course
```


### Install packages not available in conda

From your `course` virtual environment, install these additional packages:

```
pip install astroquery
pip install photutils
pip install aplpy
pip install ginga
```

## Additional installation of modules

```
conda install datashader
pip install statsmodels
pip install astroML
conda install scikit-learn
conda install pytables
pip install webargs
pip install ipywidgets=5.0.0
conda update notebook
```

## to make widgets work in the notebook

You must have ipywidgets at version 5.0.0 and notebook at 4.2.0.
Then execute:
```
jupyter nbextension enable --py widgetsnbextension
```

Widgets will work but will print a misleading error message.
