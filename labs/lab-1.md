---
layout: page
title: Lab 1 - Data Preparation, Linear Classification and Tensorflow Basics 
---

In this exercise we are going to learn about simple data curation practices, write vectorized code using numpy, 
build and visualize a simple logistic regression model and touch the basics of Tensorflow.

### Setting up a local environment 

Get the code as a zip file [here](https://drive.google.com/open?id=1swb5tzc9gkJhMvGYFZ-7kB8jVxF_yhr3). As for the dependencies:


**Installing Python 3.5+:**
To use python3, make sure to install version 3.5 or 3.6 on your local machine. If you are on Mac OS X, you can do this using [Homebrew](https://brew.sh) with `brew install python3`. You can find instructions for Ubuntu [here](https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-local-programming-environment-on-ubuntu-16-04).

**Virtual environment:**
If you decide to work locally, we recommend using [virtual environment](http://docs.python-guide.org/en/latest/dev/virtualenvs/) for the project. If you choose not to use a virtual environment, it is up to you to make sure that all dependencies for the code are installed globally on your machine. To set up a virtual environment, run the following:

```bash
cd lab1
sudo pip install virtualenv      # This may already be installed
virtualenv -p python3 .lab1      # Create a virtual environment (python3)
# Note: you can also use "virtualenv .env" to use your default python (usually python 2.7)
source .lab1/bin/activate         # Activate the virtual environment
pip install -r requirements.txt  # Install dependencies
# Work on the lab1 for a while ...
deactivate                       # Exit the virtual environment
```


**Version Managers:** During this course you will work on various different assignments and labs. To organize your python versions and virtualenvs take a look at the following version and package managers for python:
- [Pyenv](https://github.com/pyenv/pyenv)
- [Anaconda](https://www.anaconda.com/distribution/)


**Jupyter Notebooks:**
To use jupyter notebooks in the created virtual environment, follow
these [instructions](https://help.pythonanywhere.com/pages/IPythonNotebookVirtualenvs/)

### Lab 1 Notebooks
The downloaded zip file contains two notebook files: 

- `python_numpy_tutorial.ipynb`
- `lab-1.ipynb`

Place them in the directory or a subdirectory of the root of your Jupyter Notebook server. Open both of them through Jupyter Notebook's web interface (usually `localhost:8888`). 

If you still don't feel confident with the syntax of Python and how to use vectorized operations go through the content of `python_numpy_tutorial.ipynb`. 

The actual tasks for this exercise reside in the `lab-1.ipynb` notebook. Follow the instructions inside to complete the problems.
