
## Installation of Python modules (from previous class)

If you don't have Anaconda or Miniconda, go to http://conda.pydata.org/miniconda.html and install the Python 3.5 64-bit version for your system. 

Make sure you've added the `bin` directory for Miniconda to your `PATH`. Then in a terminal window, execute this command:
```
conda create -n course python=3.5 astropy pandas seaborn glueviz jupyter pillow statsmodels
```
This creates a virtual environment named `course`. You can list your environments with `conda info -e`.

### Activate the virtual environment

In a bash-like shell:
```
source activate course
```

In a csh-like shell, the `activate` is not available. Look at the output of `conda info -e` for the path to your `course`
virtual environment. Then add it to your PATH environment variable. Or, use this UNIX one-liner:
```
setenv PATH `conda info -e | grep course | awk '{printf("%s/bin\n",$NF)}'`:$PATH
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
pip install ipywidgets --upgrade
```

## to make widgets work in the notebook

```
jupyter nbextension enable --py widgetsnbextension
```
