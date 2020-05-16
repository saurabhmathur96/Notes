---
title: Handwritten Digit Recognition with a Back-Propagation Network (1990)
---

# Handwritten Digit Recognition with a Back-Propagation Network (1990)
 Le Cun, Y., Boser, B., Denker, J. S., Henderson, D., Howard, R. E., Hubbard, W., and Jackel, L. D. 

This paper deals with the problem of handwritten digit recognition using Neural Networks. The key idea is that with carefully designed neural networks, complex tasks like image recognition can be done with minimal data preprocessing.
 
## Zipcode Recoginition 
The dataset that the authors used was of segmented images of handwritten zipcodes. It was provided by the US postal service and consisted of 9298 numbers across 10 classes of 0-9.
The zipcode dataset was suppemented by a set of 3349 prinited digits from 33 different fonts.

## Preprocessing
Zip codes were binarized, located and segmented. There were errors in doing the same as some digits were broken across multiple segments.

The image size was normalized by various linear transformations.

## The network 
A multi-layered neural network was used. All connections are adaptive, although highly contrained.

An interesting operation used in the network was the convolution.
In a convolution layer, each neuron is connected to a patch in a shared filter set. Each patch of the input image is convolved with different features thus given a feature map for each filter. This allows checking of a particular pattern in the entire pattern thus making sure that the location is disregarded.

## Results and conclusion