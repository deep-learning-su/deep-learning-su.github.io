---
layout: page
title: Lab 1 - Data Preparation, Linear Classification
---

In this exercise we are going to learn about simple data curation practices, write vectorized code using numpy,
build and visualize a simple logistic regression model.

### Run online

**Recommended approach**: the lab excercise is available as a notebook in [Google Colab](https://colab.research.google.com/drive/1y5I-7pZylXr4V1qY5JDHuIWhCZ6YcfhC?usp=sharing). Open the link and click on `Copy to Drive`. After that you can start editing and running your code.

### Run locally

Download the notebook from [Google Colab](https://colab.research.google.com/drive/1y5I-7pZylXr4V1qY5JDHuIWhCZ6YcfhC?usp=sharing) by clicking on `File -> Download .ipynb`. After this you need to have Jupyter ready in order to run the notebook. requirements.txt is currently not available for this excercise so you are on your own to resolve the dependencies which are used.

**Installing Python 3.5+:**
To use python3, make sure to install version 3.5 or 3.6 on your local machine. If you are on Mac OS X, you can do this using [Homebrew](https://brew.sh) with `brew install python3`. You can find instructions for Ubuntu [here](https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-local-programming-environment-on-ubuntu-16-04).

**Virtual environment:**
If you decide to work locally, we recommend using [virtual environment](http://docs.python-guide.org/en/latest/dev/virtualenvs/) for the project. If you choose not to use a virtual environment, it is up to you to make sure that all dependencies for the code are installed globally on your machine. To set up a virtual environment, run the following:

**Version Managers:** During this course you will work on various different assignments and labs. To organize your python versions and virtualenvs take a look at the following version and package managers for python:
- [Pyenv](https://github.com/pyenv/pyenv)
- [Anaconda](https://www.anaconda.com/distribution/)


**Jupyter Notebooks:**
To use jupyter notebooks in the created virtual environment, follow
these [instructions](https://help.pythonanywhere.com/pages/IPythonNotebookVirtualenvs/)

