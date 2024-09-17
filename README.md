# Python for Geoscientists

A notebook-based introduction to python, jupyter notebooks and programming workflows with examples from python packages for the Earth Sciences.

## Description

Python has become a popular language for scientific computing, boasting a rich set of libraries relevant to geoscientists working with data. It has all the friendly features and conveniences you would expect of a modern programming language. The Python programming language offers adaptability and versatility to the types of analyses, modelling, and workflows that geoscientists utilise. The tools and workflows you will explore in this course are presented as Jupyter notebooks and can easily be adapted to your own needs.

## Getting started

We will use Google Colab to run this course. It is an interactive environment to create and run Python code.

Currently `pygplates` is not available to install on `pip`. So for notebooks running any GPlately or pygplates code, this cell will need to be run at the start of the notebook:

```sh
!pip install -q condacolab
import condacolab
condacolab.install()
```

## Installation

Conda packages are available if install GPlately and associated packages on your machine. Simply run,

```sh
conda install -c conda-forge gplately scikit-learn jupyter
```

If you don't already have conda installed, we recommend [miniforge](https://github.com/conda-forge/miniforge).


### Creating a new conda environment

We recommend creating a new conda environment inside which to install these dependencies. This avoids any potential conflicts in your base Python environment. In the example below we create a new environment called "my-env":

```sh
conda create -n my-env
conda activate my-env
conda install -c conda-forge gplately scikit-learn jupyter
```

my-env needs to be activated whenever you use GPlately: i.e. `conda activate my-env`.