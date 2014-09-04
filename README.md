# Kiwi Pycon 2014, 12 September 2014

## Tutorial: Python and the "pydata" ecosystem for data analysis

[Nicolas Fauchereau](mailto:Nicolas.Fauchereau@gmail.com)

--

### Table of contents

- [The Anaconda python distribution](#the-anaconda-python-distribution)
- [Installation of additional libraries](#installation-of-additional-libraries)
  - [Basemap](#basemap)
  - [Vincent](#vincent)
  - [Folium](#folium)
  - [Seaborn](#seaborn)
- [conda: the package and environment manager](#installation-of-additional-libraries)
- [Running the IPython notebooks](#running-the-ipython-notebooks)

## The Anaconda python distribution

For this tutorial, I recommend installing the **Anaconda Python distribution**. It is a completely free enterprise-ready Python distribution for large-scale data processing, predictive analytics, and scientific computing. It includes the python interpreter itself, the python standard library as well as a set of packages exposing data structures and methods for data manipulation and scientific computing and visualization. In particular it provides [Numpy](http://www.numpy.org/), [Scipy](http://www.scipy.org/), [Pandas](http://pandas.pydata.org/), [Matplotlib](http://matplotlib.org/), [scikit-learn](http://scikit-learn.org/stable/) and [statmodels](http://statsmodels.sourceforge.net/), i.e. all the main packages we will be using during the tutorial. The full list of packages is available at:

[http://docs.continuum.io/anaconda/pkgs.html](http://docs.continuum.io/anaconda/pkgs.html)

The Anaconda python distribution must be downloaded from:

[http://continuum.io/downloads](http://continuum.io/downloads)

For your platform.

Once you have installed Anaconda, you can update to the latest compatible versions of all the pre-installed packages by running:

```
conda update conda
```

Then

```
conda update anaconda
```

In a terminal.

You also need to install [pip](https://github.com/pypa/pip) to install packages from the [Python Package Index](http://pypi.python.org/pypi).

```
conda install pip
```

## Installation of additional libraries

While we might not have the time to cover them in depth during the tutorial, I would recommend that you have a look at a few extra libraries.

### Basemap

**Basemap** is a graphic library for plotting (static, publication quality) geographical maps (see [http://matplotlib.org/basemap/](http://matplotlib.org/basemap/)). **Basemap** is available directly in **Anaconda** using the conda package manager, install with:

```
conda install basemap
```

### Seaborn

Seaborn

## Running the IPython notebooks

The material of the tutorial is in the form of [IPython notebooks](http://ipython.org/notebook.html). In a nutshell an IPython notebook is a web-based (i.e. running in the browser) interactive computational environment where you can combine Python code execution, text, mathematics, plots and rich media into a single document, which makes it an ideal medium for teaching and exploring.
