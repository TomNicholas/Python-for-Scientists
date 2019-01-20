# Python for Science

A curated list of recommened Python frameworks, libraries, software and
resources, all particularly useful for scientific Python users.

Intended for students and researchers in the sciences who want to get
the most out of the open-source Python ecosystem.

Inspired by [awesome-python](https://github.com/vinta/awesome-python),
which is a great similar resource for anything else you might want to do
with Python!

There is a section of must-haves for beginners. (TODO)

Some libraries appear multiple times where they are useful in multiple
ways.


## Contents

- [Algebra](#algebra)
- [Animations](#animations)
- [Bayesian Analysis](#bayesian-analysis)
- [Code Quality](#code-quality)
- [Data Storage](#data-storage)
- [Dates and Times](#dates-and-times)
- [Debugging](#debugging)
- [Development Environments](#development-environments)
- [Documentation](#documentation)
- [Domain-specific](#domain-specific)
- [Gotchas](#gotchas)
- [GPU Acceleration](#gpu-acceleration)
- [Graphical Interfaces](#graphical-interfaces)
- [Job Scheduling](#job-scheduling)
- [Labelled data](#labelled-data)
- [Numerical Data](#numerical-data)
- [Optimisation](#optimisation)
- [Package Management](#package-management)
- [Parallelization](#parallelization)
- [Physical Units](#physical-units)
- [Plotting](#plotting)
- [Presentations](#presentations)
- [Profiling and Benchmarking](#profiling-and-benchmarking)
- [Speed](#speed)
- [Testing](#testing)
- [Visualisation](#visualisation)
- [Workflow](#workflow)


- - -


## Algebra

*Libraries for manipulation of symbolic algebra, analytic integration etc.*

* [SymPy]() -


## Animations

* [animatplot]() -


## Bayesian Analysis

* [pymc]() -


## Code Quality

* [PEP8]() -
* [flake8]() -
* [black]() -
* [structure](https://docs.python-guide.org/writing/structure/) - The officially recommended way to structure any python project.

## Data Storage

* [netcdf4]() -
* [xarray]() -
* [MITgcm]() -


## Dates and Times

* []() -


## Debugging

* [pdb]() - Python debugger


## Development Environments

* [PyCharm]() -
* [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/) - (follow-on from SPyder)


## Documentation

* [sphinx]() -
* [nbconvert]() -


## Domain-specific

* [astropy]() -
* [plasmapy]() -
* [psychopy]() -
* [cartopy]() -
* [geoviews]() -
* [pyrocko]() -
* [SpectroscoPyx]() -


## Forecasting

* [prophet]() -


## Gotchas

* [python-gotchas]() -


## GPU acceleration

* [py-cuda]() -
* [numba]() -


## Graphical interfaces

* [pyqt5]() -


## Job scheduling

* [experi]() -
* [papermill]() -


## Labelled data

* [pandas]() -
* [xarray]() -


## Numerical data

* [numpy]() -


## Optimisation problems

* [nlopt]() -


## Package Management

* [conda](https://conda.io/docs/index.html) - A package manager specifically intended for use by the scientific python community.
Developed by the authors of numpy to manage both python packages and the underlying C/Fortran libraries which make them fast.
Also obviates the need for system virtual environments.
* [anaconda](https://www.anaconda.com/) - Conda, but packaged with a wide range of useful scientific python libraries, including many from this list.
* [pip](https://pip.pypa.io/en/stable/) - The standard way to install python packages. Use when you can't use conda, but will play nicely together.
* [setuptools](https://setuptools.readthedocs.io/en/latest/) - For when you make your own module, and want to install it properly into your conda environment (so you never need to touch your `$PYTHONPATH`!)


## Parallelization

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

* [pint]() -
* [astropy.units]()


## Plotting

*Producing static plots of publication quality.*

* [matplotlib]() -
* [scientific-matplotlib]() -
* [seaborn]() -
* [xarray.plot]() -
* [colorcet]() -


## Presentations and sharing work

* [RISE]() -
* [Binder]() -
* [jupyter-rise]() -
* [nb_pdf_template]() -


## Profiling and benchmarking

* [py-spy]() -


## Speed

* [cython]() -
* [numba]() -
* [bottleneck]()


## Testing

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

* [animatplot]() -
* [mayavi]() -
* [cartopy]()
* [bokeh]() -
* [plotly]() -


## Workflow

* [ipython]() -
* [jupyter notebooks](https://jupyter.org/) -
* [jupyterlab](https://jupyterlab.readthedocs.io/en/stable/) -
* [papermill]() -
