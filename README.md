# Python for Scientists

A curated list of recommended Python frameworks, libraries, software and
resources, all particularly useful for scientific Python users.

Intended for students and researchers in the sciences who want to get
the most out of the open-source Python ecosystem.
Aims to provide a list of tools useful for common tasks for scientists,
without mentioning things which they are unlikely ever to need
(e.g. authentication, databases, networking, NLP).

There is a section of [must-haves for beginners](#beginner-recommendations).

List inspired by [awesome-python](https://github.com/vinta/awesome-python),
which is a great similar resource for anything else you might want to do
with Python!

Some libraries appear multiple times where they are useful in multiple
ways.


- [Python-for-Scientists](#python-for-scientists)
    - [Algebra](#algebra)
    - [Animations](#animations)
    - [Bayesian Analysis](#bayesian-analysis)
    - [Better Scientific Software](#better-scientific-software)
    - [Code Quality](#code-quality)
    - [Data Storage](#data-storage)
    - [Debugging](#debugging)
    - [Development Environments](#development-environments)
    - [Documentation](#documentation)
    - [Domain-Specific Tools](#domain-specific-tools)
    - [Error Handling](#error-handling)
    - [Forecasting](#forecasting)
    - [Gotchas](#gotchas)
    - [GPU Acceleration](#gpu-acceleration)
    - [Graphical Interfaces](#graphical-interfaces)
    - [Job Scheduling](#job-scheduling)
    - [Labelled Data](#labelled-data)
    - [Mathematical Library Functions](#mathematical-library-functions)
    - [Numerical Data](#numerical-data)
    - [Optimisation Problems](#optimisation-problems)
    - [Package Management](#package-management)
    - [Paper Writing](#paper-writing)
    - [Parallelization](#parallelization)
    - [Physical Units](#physical-units)
    - [Plotting](#plotting)
    - [Presentations and Sharing Work](#presentations-and-sharing-work)
    - [Profiling and Benchmarking](#profiling-and-benchmarking)
    - [Scripting](#scripting)
    - [Speed](#speed)
    - [Statistics](#statistics)
    - [Testing](#testing)
    - [Visualisation](#visualisation)
    - [Workflow](#workflow)
- [Beginner Recommendations](#beginners-recommendations)


- - -


## Algebra

*Libraries for manipulation of symbolic algebra, analytic integration etc.*

* [SymPy](https://www.sympy.org/en/index.html) - SymPy is a Python library for symbolic mathematics.
It aims to become a full-featured computer algebra system (CAS) while keeping the code as simple as possible in order to be comprehensible and easily extensible.
* [sagemath](http://www.sagemath.org/) - Mathematical software system with features covering multiple aspects of mathematics, including algebra, combinatorics, numerical mathematics, number theory, and calculus.


## Animations

* [animatplot](https://animatplot.readthedocs.io/en/stable/) - A wrapper around `matplotlib`'s `funcanimation` module - makes it very easy to animate matplotlib plots.
* [Line Chart Animation Tutorial](https://holypython.com/python-visualization-tutorial/guide-to-python-animations-animating-line-charts/) - A practical tutorial for creating Animated Line Charts with Matplotlib's Animation module.
* [Bar Chart Animation Tutorial](https://holypython.com/python-visualization-tutorial/creating-bar-chart-animations/) - A practical tutorial for creating Animated Bar Charts with Matplotlib's Animation module.


## Bayesian Analysis

* [pymc3](https://docs.pymc.io/) - Package for Bayesian statistical modeling and probabilistic machine learning which focuses on advanced Markov chain Monte Carlo and variational fitting algorithms.
* [arviz](https://arviz-devs.github.io/arviz/index.html) - Exploratory analysis of Bayesian models.


## Better Scientific Software

* [Better Scientific Software](https://bssw.io/) - Articles and resources on how to write better scientific software.


## Code Quality

*Tools to help you write neat and error-free python code*

* [PEP8](https://www.python.org/dev/peps/pep-0008/) - The official style guide for python code.
* [structure](https://docs.python-guide.org/writing/structure/) - The officially recommended way to structure any python project.
* [flake8](http://flake8.pycqa.org/en/latest/) - A command-line tool which will tell you where you've violated PEP8's recommendations.
* [pyflakes](https://pypi.org/project/pyflakes/) - Similar to flake8, but instead checks for logistic errors (e.g. unused module imports).
* [pycodestyle](https://media.readthedocs.org/pdf/pycodestyle/latest/pycodestyle.pdf) - A wrapper for flake8 and pyflakes which runs them both.
* [pylint](http://pylint.pycqa.org/en/latest/intro.html) - A tool that checks for errors in Python code, tries to enforce a coding standard and looks for code smells.


## Data Storage

* [netcdf4-python](http://unidata.github.io/netcdf4-python/) - netCDF is a popular file format for multidimensional data, developed by the weather and forecasting community. Use this format unless you have a good reason not to.
netcdf4-python is a Python interface to the netCDF C library.
* [xarray](http://xarray.pydata.org/en/stable/io.html#netcdf) - xarray's data model is based on netCDF, and provides the easiest way of reading and writing netCDF4 files in python.
Will also load the data lazily, which is extremely useful when dealing with large amounts of data.
* [Zarr](https://github.com/zarr-developers/zarr-python) - Zarr is a data format designed to work efficiently for very large datasets, accessed in parallel. If you normally use netCDF but want to scale up your analysis, have a look at Zarr.
* [xmitgcm](https://xmitgcm.readthedocs.io/en/latest/) - A python package for reading MITgcm binary MDS files into xarray data structures.
Included as an example of how to go about loading unusual binary file formats into xarray data structures intelligently.
* [SQLite Tutorials](https://holypython.com/python-sqlite-tutorial/) - SQLite Tutorials with Python examples, demonstrations and database tips.


## Debugging

* [pdb](https://docs.python.org/3/library/pdb.html) - The Python debugger. Part of the python standard library.


## Development Environments

*Programs to write code into. The main choice is between a software-engineering style IDE, and one intended specifically for scientific users.*

* [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/) - An IDE which incorporates Jupyter notebooks.
* [PyCharm](https://www.jetbrains.com/pycharm/) - Very powerful IDE for python. Use if you want the full powers a software engineer would expect.
Has a professional version, which is free for students.
* [spyder](https://www.spyder-ide.org/) - MatLab-like development environment for scientific python users.


## Documentation

* [sphinx](http://www.sphinx-doc.org/en/master/) - Sphinx is a tool that makes it easy to create intelligent and beautiful documentation, from the docstrings in your code.
Originally created for documenting the python language itself.
* [nbconvert](https://nbconvert.readthedocs.io/en/latest/) - Convert jupyter notebooks to other formats such as PDF, LaTeX, HTML.


## Domain-Specific Tools

*Libraries of tools developed for python users in various fields of science.*

* [astropy](http://www.astropy.org/) - Various tools and functionality for astronomy and astrophysics.
* [Biopython](https://biopython.org/) - Tools for biological computation.
* [geoviews](http://geoviews.org/) - Makes it easy to explore and visualize geographical, meteorological, and oceanographic datasets, such as those used in weather, climate, and remote sensing research.
* [MetPy](https://unidata.github.io/MetPy/latest/) - MetPy is a collection of tools in Python for reading, visualizing and performing calculations with weather data.
* [NetworkX](http://networkx.github.io/)  - A package for the creation, manipulation, and study of the structure, dynamics, and functions of complex networks.
* [nilearn](http://nilearn.github.io/) - Machine learning for Neuro-Imaging in python.
* [Parcels](http://oceanparcels.org/) - Track particles along circulating ocean currents.
* [PlasmaPy](http://docs.plasmapy.org/en/stable/) - Various tools for plasma physics.
* [ProDy](http://prody.csb.pitt.edu/) - Package for protein structural dynamics analysis.
* [psychopy](http://www.psychopy.org/) - An open-source application allowing you run a wide range of neuroscience, psychology and psychophysics experiments.
* [pyrocko](https://pyrocko.org/) - A seismology toolkit for python.
* [QuTIP](http://qutip.org/) - QuTiP is open-source software for simulating the dynamics of open quantum systems.
* [radis](https://github.com/radis/radis) - A package for infrared molecular spectroscopy
* [scikit-beam](https://github.com/scikit-beam/scikit-beam) - Data analysis tools for X-Ray, Neutron and Electron sciences
* [scikit-spectra](http://hugadams.github.io/scikit-spectra/) - A community developed python package for spectroscopy.
* [SunPy](https://sunpy.org/) - SunPy is a data-analysis environment specializing in providing the software necessary to analyze solar and heliospheric data in Python.
* [TomoPy](https://tomopy.readthedocs.io/en/latest/) - Package for tomographic data processing and image reconstruction.


## Error Handling

* [errors](https://docs.python.org/3/tutorial/errors.html) - How to properly raise and handle errors in python.
* [warnings](https://docs.python.org/3/library/warnings.html) - Throw proper warnings instead of using print statements. Python standard library module.
* [logging](https://docs.python.org/3/library/logging.html) - Standard library module for properly logging information about what's going on as your code runs.


## Forecasting

* [prophet](https://facebook.github.io/prophet/) - Tool for producing high quality forecasts for time series data that has multiple seasonality with linear or non-linear growth.
Developed by Facebook.


## Gotchas

* [python-gotchas](https://github.com/satwikkansal/wtfpython) - A collection of surprising Python snippets and lesser-known features.
* [100 Python Tips & Tricks](https://holypython.com/100-python-tips-tricks/) - 100 Essential Python Tips with interesting Examples


## GPU Acceleration

* [cupy](https://cupy.chainer.org/) - An implementation of a NumPy-compatible multi-dimensional array on CUDA.
* [numba](http://numba.pydata.org/numba-doc/0.13/CUDAJit.html) - Numba can compile python functions into CUDA code.


## Graphical Interfaces

* [pyqt5](http://pyqt.sourceforge.net/Docs/PyQt5/) - Library which lets you use the Qt GUI framework (itself written in C++) from python.
* [PySimpleGui](http://pyqt.sourceforge.net/Docs/PyQt5/) - A simple library for creating GUI programs with Python very quickly.
* [Practical PySimpleGui Tutorials](https://holypython.com/python-gui-tutorial/) - Useful PySimpleGui Tutorials with Python Examples


## Job Scheduling

* [experi](https://experi.readthedocs.io/en/latest/) - An interface for managing computational experiments with many independent variables.
* [lancet](http://ioam.github.io/lancet/) - Launch jobs, organize the output, and dissect the results.
* [papermill](https://papermill.readthedocs.io/en/latest/) - A  tool for parameterizing, executing, and analyzing multiple Jupyter Notebooks.


## Labelled Data

* [pandas](https://pandas.pydata.org/) - Major library for data analysis, made more powerful through the use of labelled data.
* [xarray](http://xarray.pydata.org/en/stable/) - N-dimensional labelled arrays and datasets.
Allows you to perform operations with incredible ease and clarity:
  ```python
  average_temp = data['temperature'].sel('longitude'=40).mean(dim='time')
  ```

## Mathematical Library Functions

* [scipy](https://docs.scipy.org/doc/scipy/reference/) - The standard resource for all kinds of mathematical functions.
* [xrft](https://xrft.readthedocs.io/en/latest/) - Discrete Fourier transform operations for xarray data structures.


## Numerical Data

* [numpy](http://www.numpy.org/) - The fundamental package for numerical computation in python.
So ubiquitous that it might as well be part of python's standard library at this point.
Ultimately just a contiguous-in-memory C array, wrapped very nicely with python.


## Optimisation Problems

* [nlopt](https://github.com/stevengj/nlopt) - Library for nonlinear optimization, wrapping many algorithms for global and local, constrained or unconstrained, optimization.


## Package Management

*Keep track of module dependencies, python versions, and virtual environments.*

* [conda](https://conda.io/docs/index.html) - A package manager specifically intended for use by the scientific python community.
Developed by the authors of numpy to manage both python packages and the underlying C/Fortran libraries which make them fast.
Also obviates the need for system virtual environments.
* [anaconda](https://www.anaconda.com/) - Conda, but packaged with a wide range of useful scientific python libraries, including many from this list.
* [pip](https://pip.pypa.io/en/stable/) - The standard way to install python packages. Use when you can't use conda, but will play nicely together.
* [setuptools](https://setuptools.readthedocs.io/en/latest/) - For when you make your own module, and want to install it properly into your conda environment (so you never need to touch your `$PYTHONPATH`!)


## Paper Writing

* [tikzplotlib](https://github.com/nschloe/tikzplotlib) - A converter that takes a matplotlib figure and spits out a TikZ/PGFplots figure for smooth integration into LaTeX.
Much better than having to try and alter details of a png image later on.
* [Scientific Writing](https://github.com/natj/sci_writing) - Not python, but a few useful tips on scientific writing.


## Parallelization

*Use all the cores of your machine, and scale up to clusters!*

* [dask](https://dask.org/) - Tools for splitting up computations and executing them across many processors in parallel.
[dask.array](http://docs.dask.org/en/latest/array.html) in particular provides a numpy-like interface to a chunked-in-memory array.
Dask is especially useful for analysing datasets which are larger than your RAM.
* [xarray](http://xarray.pydata.org/en/stable/) - Employs dask behind the scenes to parallelize most operations.
  Simply load your dataset in "chunks" and xarray will operate on each chunk in parallel:
  ```python
  # Load data in chunks
  ds = open_dataset('data.nc', chunks={'space': 100}

  # Will operate on each spatial chunk in parallel using dask
  ds['density'].mean(dim='time')
  ```


## Physical Units

*Keep track of which physical units your numbers are written in.*

* [pint](https://pint.readthedocs.io/en/0.9/) - Package to define, operate and manipulate physical quantities.
* [astropy.units](http://docs.astropy.org/en/stable/units/) - Submodule of astropy which handles units. Units multiply numpy arrays directly.


## Plotting

*Producing static plots of publication quality. (For 3D plots see the *Visualisation* section)*

* [matplotlib](https://matplotlib.org/) - A 2D plotting library which produces publication quality figures in a variety of hardcopy formats and interactive environments across platforms.
The standard way to plot data in python.
* [anatomy of matplotlib](https://github.com/matplotlib/AnatomyOfMatplotlib) - Tutorials on how to use matplotlib.
* [matplotlib guide](https://realpython.com/python-matplotlib-guide/) - Article explaining how matplotlib is intended to be used, and will help clarify the differences between figures and axes, object-oriented approach, MATLAB-like stateful approach, interactivity etc. Also good because it gives clear best practice recommendations.
* [scientific-matplotlib](https://github.com/garrettj403/SciencePlots) - Matplotlib stylesheets for scientific plots.
* [seaborn](https://seaborn.pydata.org/) - A  data visualisation library based on matplotlib. Produces much prettier plots than out-of-the-box matplotlib will.
* [xarray.plot](http://xarray.pydata.org/en/stable/plotting.html) - Submodule of xarray which makes plotting into a one-line job: `data['density'].plot()`.
* [colorcet](http://colorcet.pyviz.org/) - A set of useful [perceptually uniform](https://arxiv.org/abs/1509.03700) colormaps for plotting scientific data.
* [Hexbin](https://holypython.com/python-visualization-tutorial/creating-hexbin-charts/) - Hexbin plotting tutorials.
* [Pcolor](https://holypython.com/python-visualization-tutorial/pcolor-and-pcolormesh/) - Pcolor and Pcolormesh tutorials
* [Wordcloud](https://holypython.com/python-visualization-tutorial/word-cloud-visualization/) - Wordcloud Visualization with Python examples
* [holoviews](https://holoviews.org/) - A much more modern plotting library, useful for all sorts of scientific data. Interactive, scalable, and animatable.


## Presentations and Sharing Work

* [Binder](https://mybinder.org/) - Online Jupyter Notebook hosting for GitHub repositories.
Allows users to run Jupyter notebooks from GitHub repositories in the cloud, without Python installed locally.
* [nb_pdf_template](https://github.com/t-makaro/nb_pdf_template) - A more accurate representation of jupyter notebooks when converting to pdfs.
* [RISE](https://rise.readthedocs.io/en/docs_hot_fixes/) - A plugin for Jupyter which turns notebooks into slick presentations.
* [jupyter-rise](https://github.com/binder-examples/jupyter-rise) - Automatically launch the RISE plugin from Binder. Great for giving presentations remotely.


## Profiling and benchmarking

* [py-spy](https://github.com/benfred/py-spy) - A profiler for python code which doesn't interfere with the running process.
* [pytest-benchmark](https://pytest-benchmark.readthedocs.io/en/stable/) - A pytest fixture for benchmarking code.


## Scripting

*Tools which are likely to be useful when writing python scripts to automate common tasks.*

* [click](https://palletsprojects.com/p/click/) - Run your scripts from the command line, with as little extra code as possible.
* [dateutil](https://dateutil.readthedocs.io/en/stable/) - Provides powerful extensions to the standard datetime module available in Python.
* [gitpython](https://gitpython.readthedocs.io/en/stable/) - Interact with git from python. Useful for tasks like checking if your simulation code has uncommitted changes before executing it.
* [pathlib](https://docs.python.org/3/library/pathlib.html) - Use this anytime you want to do anything with a file path. Obviates the need for `os` and `sys` most of the time.
A module in the python standard library.
* [Event Scheduling](https://holypython.com/how-to-schedule-tasks-with-py-files-python-manual-automated/) - Event scheduling script examples for Python 


## Speed

*Python inevitably sacrifices some speed to gain increased clarity.
Scientific programs usually have one or two functions which do 90% of the work, and there are various ways to dramatically speed these up.
Use in conjunction with parallelization through dask if you want as much speed as possible.*

* [cython](https://cython.org/) - A compiler which allows you to write snippets of C code into your python for massive speed increases.
* [F2PY](https://docs.scipy.org/doc/numpy/f2py/) - For calling fast, compiled Fortran subroutines from Python (part of SciPy)
* [numba](https://numba.pydata.org/) - *Automatic* generation of fast compiled C code from Python functions.
* [bottleneck](https://kwgoodman.github.io/bottleneck-doc/) - A collection of fast numpy array functions written in C.
* [Theano](http://www.deeplearning.net/software/theano/) - Allows you to define, optimize, and evaluate mathematical expressions involving multi-dimensional arrays efficiently.


## Statistics

* [statsmodels](http://www.statsmodels.org/stable/index.html) - Provides classes and functions for the estimation of many different statistical models, as well as for conducting statistical tests, and statistical data exploration.


## Testing

*Check that your code actually does what you think it will do!*

* [pytest](https://docs.pytest.org/en/latest/) - The standard unit testing framework for python.
Essential - if you're not unit-testing your calculations then you are merely hoping that they are actually doing what you think they are.
`pytest` does a lot of magic behind the scenes to make it as simple as possible to use, with no boilerplate.
* [pytest-clarity](https://github.com/darrenburns/pytest-clarity) - A plugin which improves the readability of pytest output.
* [hypothesis](https://hypothesis.readthedocs.io/en/latest/) - Hypothesis testing for python.
Normal tests check that your function behaves as expected for some specific input.
Hypothesis tests check that your function behaves as expected for any input of some type, e.g. any string, or [any numpy array](https://hypothesis.readthedocs.io/en/latest/numpy.html).
Basically magic, compatible with pytest, and the algorithms used in the implementation are very interesting.
* [cosmic-ray](https://cosmic-ray.readthedocs.io/en/latest/) - Mutation testing in python. Checks that your test coverage is robust by randomly changing pieces of your code and checking that this change is actually caught by a test failing.
* [flaky](https://pypi.org/project/flaky/) - pytest plugin for automatically re-running inconsistent ("flaky") tests.


## Visualisation

*There are currently many competing visualisation libaries in python.*

* [animatplot](https://animatplot.readthedocs.io/en/stable/) - A wrapper around `matplotlib`'s `funcanimation` library - makes it very easy to animate matplotlib plots.
* [mayavi](http://docs.enthought.com/mayavi/mayavi/) - 3D scientific data visualization and plotting in Python.
* [cartopy](https://scitools.org.uk/cartopy/docs/latest/) -  A library for cartographic projections and plots, with matplotlib support.
* [bokeh](https://bokeh.pydata.org/en/latest/) - Bokeh is an interactive visualization library that targets modern web browsers for presentation.
* [K3D-jupyter](https://github.com/K3D-tools/K3D-jupyter) - K3D-jupyter is a new 3D plotting library which uses WebGL to create interactive plots in jupyter notebooks. Very powerful and fast, with some [seriously impressive examples](https://k3d-jupyter.readthedocs.io/en/latest/showcase/index.html). However as of early 2020 the [documentation](https://k3d-jupyter.readthedocs.io/en/latest/index.html) is a little lacking.
* [plotly](https://plot.ly/python/) - Plotly's Python graphing library makes interactive, publication-quality graphs online.
* [holoviews](http://holoviews.org/) - Stop plotting your data - annotate your data and let it visualize itself.
* [ipyvolume](https://ipyvolume.readthedocs.io/en/latest/index.html#built-on-ipywidgets) - 3d plotting for Python in the Jupyter notebook.
* [vispy](http://vispy.org/index.html) - Interactive scientific visualisation in python.
* [vtk](https://pypi.org/project/vtk/) - Low-level VTK interface
* [vista](https://docs.pyvista.org/) - Streamlined interface to VTK - mainly a wrapper for VTK package
* [yt](http://yt-project.org/) - Very powerful software suite for analysing and visualising volumetric data.
Written by astrophysicists, but since applied to many other domains.

## Workflow

*Don't just write and run python scripts. Tools to make your workflow faster, clearer, and easier to come back to later.*

* [ipython](https://ipython.readthedocs.io/en/stable/) - Run python interactively, like MatLab! Forms the backend of Jupyter notebooks.
* [jupyter notebooks](https://jupyter.org/) - In-browser notebooks comprised of cells which can contain markdown, images, or executable python code! Incredibly valuable for data exploration, presentation and recording work. The perfect format to email to a supervisor for feedback. Can be version-controlled with git so also useful for reproducibility and backing up your work.
* [jupyterlab](https://jupyterlab.readthedocs.io/en/stable/) - A development environment in which you can write Jupyter notebooks.
The spiritual successor to spyder, in that it is designed specifically for scientists.
* [papermill](https://papermill.readthedocs.io/en/latest/) - A  tool for parameterizing, executing, and analyzing multiple Jupyter Notebooks.


# Beginner Recommendations

* First, [install python](https://www.scaler.com/topics/python/how-to-install-python-in-windows/) through anaconda, which will also give you the packages you're about to use.
* Write your code in either `pycharm` (if you want a professional IDE), `spyder` or  `jupyterlab` (if you're used to MatLabs' environment).
* Become familiar with `numpy`, the fundamental numeric object in python, and `matplotlib`, the standard way to plot.
* Next, wrap your data into clearer, higher-level objects with either `Pandas` or `xarray` (use `xarray` if your data has more than one dimension).
* Before writing new analysis functions, check if someone has already solved your problem for you in `scipy` , or in one of python's domain-specific scientific software packages.
* As soon as you start writing your own analysis functions, test they're correct with unit tests written with `pytest`.
* Analyse your data interactively with `ipython`, and record your work in a `Jupyter notebook`.
* Plot your results with `holoviews`.
