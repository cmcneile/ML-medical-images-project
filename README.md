# Project on building classifiers for medical images.

## Introduction

The aim of this project is develop classifiers for medical images,
such as X-rays. For example, the classifier is trained on images
of lungs, some of which may be labelled as having covid of being
healthy. The clasifier then should be able to determine whether a new x-ray
of a lung is healthy or the patient has covid. See
[this general review of classifiers of medical images](https://www.sciencedirect.com/science/article/pii/S093938891830120X).

## Tutorials

To learn about the basic idea of building image classifiers, please
work thorugh the following online tutorial.

* [Intro to Machine Learning](https://www.kaggle.com/learn/intro-to-machine-learning)
* Work through this kaggle tutorial on building an image classifier
  [Intro to Deep Learning](https://www.kaggle.com/learn/intro-to-deep-learning)
* [Computer Vision](https://www.kaggle.com/learn/computer-vision) 

The use of Jupyter notebooks is recommended to run python.

* https://jupyter.org/
* Google allows jupyter notebooks to run in their data centers [Google collab](https://colab.research.google.com/)


See this example of an image classifier for
[Brain Tumor Detection](https://www.kaggle.com/code/aniketkadam702030/brain-mri-inceptionv3/notebook).

##  Background videos

The University of Plymouth has access to linkedin videos.
See [here for information about access](https://www.plymouth.ac.uk/about-us/university-structure/service-areas/it-services/linkedin-learning)

* [building deep learning applications with keras 2-0](https://www.linkedin.com/learning/building-deep-learning-applications-with-keras-2-0/welcome?u=26140778
)
* [neural networks and convolutional neural networks essential training](https://www.linkedin.com/learning/neural-networks-and-convolutional-neural-networks-essential-training/welcome?u=26140778)

## Data sets

An important issue is finding a good data set.

* [kaggle](https://www.kaggle.com/)
* (https://openneuro.org/)
* (https://sites.duke.edu/mazurowski/resources/breast-cancer-mri-dataset/?s=09)

##  Model evaluation

* To evaluate the model the confusion matrix and recall and precision need to be computed. (See Confusion Matrix with Scikit-Learn and Python)[https://pieriantraining.com/confusion-matrix-with-scikit-learn-and-python/]
* (Interpretability versus explainability)[https://docs.aws.amazon.com/whitepapers/latest/model-explainability-aws-ai-ml/interpretability-versus-explainability.html]
* [Explainable Deep Learning: A Field Guide for the Uninitiated](https://arxiv.org/abs/2004.14545)

## Project plan

There are two basic choices of project. One investigates the energy consumption of the machine learning model. The other option estimate the uncertainty on the classifier using a technique called conformal
prediction. You only need to select one option.

### Project Plan  (green energy option)

* Write some code classify [hand written images of numbers](https://en.wikipedia.org/wiki/MNIST_database). Explore a few different networks and algorithms
[see here](https://keras.io/examples/vision/mnist_convnet/).
[and here](https://atmamani.github.io/projects/ml/mnist-digits-classification-using-logistic-regression-scikit-learn/).
Compute numbers
such as accuracy, precision and recall.
* Investigate the use of  [Code Carbon](https://codecarbon.io/) to measure the
energy use. Instructions on installing the python modules
are here https://pypi.org/project/codecarbon/. Are the numbers reasonable, can the numbers on energy used
be calibrated and tested?
* Use Code Carbon to measure the energy of efficiency of the digit classifiers.
* Do a literature search on energy consumption used by data science and AI.
Are there any lessons from thermodynamics on energy efficiency.
* Write and tune a classifier for the brain tumour images.
* Investigate the energy consumption of the brain tumour classifier.


### Project Plan  (uncertainty estimate)

* Write some code classify [hand written images of numbers](https://en.wikipedia.org/wiki/MNIST_database). Explore a few different networks and algorithms
[see here](https://keras.io/examples/vision/mnist_convnet/).
[and here](https://atmamani.github.io/projects/ml/mnist-digits-classification-using-logistic-regression-scikit-learn/).
Compute numbers
such as accuracy, precision and recall.
* Investigate the use of [Conformal prediction](https://en.wikipedia.org/wiki/Conformal_prediction) to compute the error on the classifier.
* The [mapie library](https://mapie.readthedocs.io/en/latest/) implements conformal prediction.

## Background reading (Books)

* [Book: Neural Networks and Deep Learning (Nielsen) ](https://eng.libretexts.org/Bookshelves/Computer_Science/Applied_Programming/Book%3A_Neural_Networks_and_Deep_Learning_(Nielsen))

* The Hundred-Page Machine Learning Book
by Andriy Burkov. You can read chapters for free at (http://themlbook.com/)

* Deep Learning by Ian Goodfellow, Yoshua Bengio, Aaron Courville

##  Futher Directions

The project can be extended in different ways

* [Explainable AI](https://www.ibm.com/topics/explainable-ai)

* [Green AI](https://hbr.org/2023/07/how-to-make-generative-ai-greener)
  See this python package that will estimate the carbon cost
  [Code Carbon] (https://codecarbon.io/)

