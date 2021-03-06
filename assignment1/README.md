# Assignment 1

## Overview

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

## Contents

### Roadmap

- [x] ~~Q1: k-Nearest Neighbor classifier~~ 2018/10/13
- [x] ~~Q2: Training a Support Vector Machine~~ 2018/10/15
- [x] ~~Q3: Implement a Softmax classifier~~ 2018/10/16
- [x] ~~Q4: Two-Layer Neural Network~~ 2018/10/16
- [x] ~~Q5: Higher Level Representations: Image Features~~ 2018/10/16

### Q1: k-Nearest Neighbor classifier (20 points)

The IPython Notebook [knn.ipynb](https://github.com/ECer23/cs231n.assignments/blob/master/assignment1/knn.ipynb) will walk you through implementing the kNN classifier.

### Q2: Training a Support Vector Machine (25 points)

The IPython Notebook [svm.ipynb](https://github.com/ECer23/cs231n.assignments/blob/master/assignment1/svm.ipynb) will walk you through implementing the SVM classifier.

### Q3: Implement a Softmax classifier (20 points)

The IPython Notebook [softmax.ipynb](https://github.com/ECer23/cs231n.assignments/blob/master/assignment1/softmax.ipynb) will walk you through implementing the Softmax classifier.

### Q4: Two-Layer Neural Network (25 points)
The IPython Notebook [two_layer_net.ipynb](https://github.com/ECer23/cs231n.assignments/blob/master/assignment1/two_layer_net.ipynb) will walk you through the implementation of a two-layer neural network classifier.

### Q5: Higher Level Representations: Image Features (10 points)

The IPython Notebook [features.ipynb](https://github.com/ECer23/cs231n.assignments/blob/master/assignment1/features.ipynb) will walk you through this exercise, in which you will examine the improvements gained by using higher-level representations as opposed to using raw pixel values.

## Setup

Get the code as a zip file [here](http://cs231n.github.io/assignments/2018/spring1718_assignment1.zip).

You can follow the setup instructions [here](http://cs231n.github.io/setup-instructions/).

### Download data:
Once you have the starter code (regardless of which method you choose above), you will need to download the CIFAR-10 dataset.
Run the following from the `assignment1` directory:

```bash
$ cd cs231n/datasets
$ ./get_datasets.sh
```

### Start IPython:
After you have the CIFAR-10 data, you should start the IPython notebook server from the
`assignment1` directory, with the `jupyter notebook` command. (See the [Google Cloud Tutorial](http://cs231n.github.io/gce-tutorial/) for any additional steps you may need to do for setting this up, if you are working remotely)

If you are unfamiliar with IPython, you can also refer to our
[IPython tutorial](/ipython-tutorial).

### Some Notes
**NOTE 1:** This year, the `assignment1` code has been tested to be compatible with python version `3.6` (it may work with other versions of `3.x`, but we won't be officially supporting them). You will need to make sure that during your virtual environment setup that the correct version of `python` is used. You can confirm your python version by (1) activating your virtualenv and (2) running `which python`.

**NOTE 2:** If you are working in a virtual environment on OSX, you may *potentially* encounter
errors with matplotlib due to the [issues described here](http://matplotlib.org/faq/virtualenv_faq.html). In our testing, it seems that this issue is no longer present with the most recent version of matplotlib, but if you do end up running into this issue you may have to use the `start_ipython_osx.sh` script from the `assignment1` directory (instead of `jupyter notebook` above) to launch your IPython notebook server. Note that you may have to modify some variables within the script to match your version of python/installation directory. The script assumes that your virtual environment is named `.env`.
