# Kiwi Pycon 2014, 12 September 2014

## Tutorial: Python and the "pydata" ecosystem for data analysis

Contact: [Nicolas Fauchereau](mailto:Nicolas.Fauchereau@gmail.com)

--

### Table of contents

- [The Anaconda python distribution](#the-anaconda-python-distribution)
- [Installation of additional libraries](#installation-of-additional-libraries)
  - [Basemap](#basemap)
  - [Bokeh](#bokeh)
  - [Seaborn](#seaborn)
  - [mplD3](#mplD3)
  - [bearcart](#bearcart)
  - [folium](#folium)
- [Running the IPython notebooks](#running-the-ipython-notebooks)

## The Anaconda python distribution

For this tutorial, I recommend installing the **Anaconda Python distribution**. It is a completely free enterprise-ready Python distribution for large-scale data processing, predictive analytics, and scientific computing. It includes the python interpreter itself, the python standard library as well as a set of packages exposing data structures and methods for data manipulation and scientific computing and visualization. In particular it provides [Numpy](http://www.numpy.org/), [Scipy](http://www.scipy.org/), [Pandas](http://pandas.pydata.org/), [Matplotlib](http://matplotlib.org/), [scikit-learn](http://scikit-learn.org/stable/) and [statmodels](http://statsmodels.sourceforge.net/), i.e. all the main packages we will be using during the tutorial. The full list of packages is available at:

[http://docs.continuum.io/anaconda/pkgs.html](http://docs.continuum.io/anaconda/pkgs.html)

The Anaconda python distribution must be downloaded from:

[http://continuum.io/downloads](http://continuum.io/downloads)

For your platform.

Once you have installed Anaconda, you can update to the latest compatible versions of all the pre-installed packages by running:

```
$ conda update conda
```

Then

```
$ conda update anaconda
```

In a terminal.

You also need to install [pip](https://github.com/pypa/pip) to install packages from the [Python Package Index](http://pypi.python.org/pypi).

```
$ conda install pip
```

## Installation of additional libraries

While we might not have the time to cover them in depth during the tutorial, I would recommend that you have a look at a few extra libraries.

### Basemap

**Basemap** is a graphic library for plotting (static, publication quality) geographical maps (see [http://matplotlib.org/basemap/](http://matplotlib.org/basemap/)). **Basemap** is available directly in **Anaconda** using the conda package manager, install with:

```
$ conda install basemap
```

### Bokeh

[Bokeh]() is a new interactive plotting library developed by the team behind **anaconda**: it is thus installable with conda (if not already installed):

```
$ conda install bokeh
```

### Seaborn

[seaborn](http://web.stanford.edu/~mwaskom/software/seaborn/) is a Python visualization library based on matplotlib. It provides a high-level interface for drawing attractive statistical graphics. You should be able to install it with ```pip```:

```
$ pip install seaborn
```
or (if you want the bleeding edge version):

```
$ pip install git+git://github.com/mwaskom/seaborn.git#egg=seaborn
```

You may have to install 2 additional libraries for seaborn, `husl` and `moss`. If you experience failures during `seaborn` installation or when trying to import it, tr:  

```
$ pip install husl
$ pip install moss
```

### mplD3

[mplD3](http://mpld3.github.io/) aims at *bringing matplotlib to the browser*. It has been developed by Jake VanDerPlas. It is also installable by ```pip```:

```
$ pip install mpld3
```

### bearcart

[bearcart](https://github.com/wrobstory/bearcart) has been developed by [Rob Story](http://wrobstory.github.io/) and provides an interface to the rickshaw JavaScript library. It is also installable via ```pip```:

```
$ pip install bearcart
```

### folium

[folium](https://github.com/wrobstory/folium)  has been also been developed by [Rob Story](http://wrobstory.github.io/) to provide an interface to the [leaflet.js](http://leafletjs.com/) JavaScript mapping library. Install with:

```
$ pip install folium
```

## Running the IPython notebooks

The material of the tutorial is in the form of [IPython notebooks](http://ipython.org/notebook.html). In a nutshell an IPython notebook is a web-based (i.e. running in the browser) interactive computational environment where you can combine Python code execution, text, mathematics, plots and rich media into a single document, which makes it an ideal medium for teaching and exploring.

After uncompressing the archive of the repo (or after cloning it with ```git```), navigate to the corresponding directory (containing the ```*.ipynb``` files) and type:

```
$ ipython notebook
```

That should bring up the IPython notebook dashboard, you should be ready to go !
