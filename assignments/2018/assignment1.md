---
layout: page
mathjax: true
permalink: /assignments/2018/assignment1/
---

In this assignment you will practice putting together a simple image classification pipeline, based on the k-Nearest Neighbor or the SVM/Softmax classifier. The goals of this assignment are as follows:

- understand the basic **Image Classification pipeline** and the data-driven approach (train/predict stages)
- understand the train/val/test **splits** and the use of validation data for **hyperparameter tuning**.
- develop proficiency in writing efficient **vectorized** code with numpy
- implement and apply a k-Nearest Neighbor (**kNN**) classifier
- implement and apply a Multiclass Support Vector Machine (**SVM**) classifier
- implement and apply a **Softmax** classifier
- implement and apply a **Two layer neural network** classifier
- understand the differences and tradeoffs between these classifiers
- get a basic understanding of performance improvements from using **higher-level representations** than raw pixels (e.g. color histograms, Histogram of Gradient (HOG) features)

### Working locally
Get the code as a zip file [here](https://drive.google.com/file/d/1nVNYdEgm2Z7Ze2gzuoz9JLdOTXtt3hxu/view?usp=sharing). As for the dependencies:

**Installing Python 3.5+:**
To use python3, make sure to install version 3.5 or 3.6 on your local machine. If you are on Mac OS X, you can do this using [Homebrew](https://brew.sh) with `brew install python3`. You can find instructions for Ubuntu [here](https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-local-programming-environment-on-ubuntu-16-04).

**Virtual environment:**
If you decide to work locally, we recommend using [virtual environment](http://docs.python-guide.org/en/latest/dev/virtualenvs/) for the project. If you choose not to use a virtual environment, it is up to you to make sure that all dependencies for the code are installed globally on your machine. To set up a virtual environment, run the following:

```bash
cd assignment1
sudo pip install virtualenv      # This may already be installed
virtualenv -p python3 .env       # Create a virtual environment (python3)
# Note: you can also use "virtualenv .env" to use your default python (usually python 2.7)
source .env/bin/activate         # Activate the virtual environment
pip install -r requirements.txt  # Install dependencies
# Work on the assignment for a while ...
deactivate                       # Exit the virtual environment
```

Note that every time you want to work on the assignment, you should run `source .env/bin/activate` (from within your `assignment1` folder) to re-activate the virtual environment, and `deactivate` again whenever you are done.

**Jupyter Notebooks:**
To use jupyter notebooks in the created virtual environment, follow
these instructions: [instructions](https://help.pythonanywhere.com/pages/IPythonNotebookVirtualenvs/)

**Download data:**
Once you have the starter code, you will need to download the CIFAR-10 dataset.
Run the following from the `assignment1` directory:

```bash
cd deep-learning-su/datasets
./get_datasets.sh
```

**Start IPython:**
After you have the CIFAR-10 data, you should start the IPython notebook server from the
`assignment1` directory. If you are unfamiliar with IPython, you should read our
[IPython tutorial](/ipython-tutorial).

**NOTE:** If you are working in a virtual environment on OSX, you may encounter
errors with matplotlib due to the [issues described here](http://matplotlib.org/faq/virtualenv_faq.html). You can work around this issue by starting the IPython server using the `start_ipython_osx.sh` script from the `assignment1` directory; the script assumes that your virtual environment is named `.env`.

### Submitting your work:
Whether you work on the assignment locally or using Terminal, once you are done
working run the `collectSubmission.sh` script; this will produce a file called
`assignment1.zip`. Then follow the instructions described [here](https://deep-learning-su.github.io/assignment-requirements/).

### Q1: k-Nearest Neighbor classifier (20 points)

The IPython Notebook **knn.ipynb** will walk you through implementing the kNN classifier.

### Q2: Training a Support Vector Machine (25 points)

The IPython Notebook **svm.ipynb** will walk you through implementing the SVM classifier.

### Q3: Implement a Softmax classifier (20 points)

The IPython Notebook **softmax.ipynb** will walk you through implementing the Softmax classifier.

### Q4: Two-Layer Neural Network (25 points)
The IPython Notebook **two\_layer\_net.ipynb** will walk you through the implementation of a two-layer neural network classifier.

### Q5: Higher Level Representations: Image Features (10 points)

The IPython Notebook **features.ipynb** will walk you through this exercise, in which you will examine the improvements gained by using higher-level representations as opposed to using raw pixel values.

### Q6: Cool Bonus: Do something extra! (+10 points)

Implement, investigate or analyze something extra surrounding the topics in this assignment, and using the code you developed. For example, is there some other interesting question we could have asked? Is there any insightful visualization you can plot? Or anything fun to look at? Or maybe you can experiment with a spin on the loss function? If you try out something cool we'll give you up to 10 extra points and may feature your results in the lecture.
