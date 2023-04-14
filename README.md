# 2D-contours dataset

In this repository, we publish our 2D, closed and planar contour datasets used to train and test the Deep learning model presented in our paper entitled
"DeepGCSS: a robust and explainable contour classifier providing Generalized Curvature Scale Space features".

For our tests, we use MPEG-7 and MNIST digits datasets. For both datasets, we proceed an arc-length re-parametrization of contours. 
A brief description of the datasets and their preprocessing is available in details in this repository. 

### MPEG-7 contours dataset:
We extract contours from the MPEG-7 database which consists of 70 types of objects each having 20 different shapes, for a total of 1400 shapes. The database is challenging due to the presence of examples that are visually dissimilar from other members of their class and examples that are highly similar to members of other classes.

<img src="Images/mpeg7.PNG" width=400 >
Figure 1: Dataset: On the left MPEG-7 image dataset; On the right MPEG7
contour datase

### MNIST 2D contours dataset: 
The MNIST database of handwritten digits (available in the following link: http://yann.lecun.com/exdb/mnist/) is a subset of a larger set available from MNIST. It contains 70000 images. We introduce our proposed algorithm \ref{contour_extract} where we call $bwboundaries$ function implemented in Matlab in order to extract external contours from this image dataset.
We divide the obtained set into 60000 contours for training and 10000 contours for validation.

<img src="Images/mnist.png " width=400 >
Figure 2: MNIST Dataset: On the top some samples from the MNIST image
dataset; On the bottom corresponding MNIST contour dataset

Contours are reparametrized using the arc length parametrization 

Other than MPEG-7 exisiting contour dataset

<img src="Images/Algorithm1.PNG" width=550 >

For testing the DeepGCSS model  we first use MNIST digits dataset in order to compare our results with ContourCNN that chooses to use this same set. For extracting contours from this image datasets, we use (algorithm1) where we call bwboundaries function implemented in Matlab.

