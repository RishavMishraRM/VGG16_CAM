# VGG16_CAM


# Implementation of the VGG-CAM model with keras

## Source

Original matlab implementation and paper [here](https://github.com/metalbubble/CAM).

## Requirements

- keras with theano backend (keras version 1.0.4 or later)
- h5py
- numpy
- matplotlib
- opencv3

## External data

Download the keras [vgg16 weights](https://gist.github.com/baraldilorenzo/07d7802847aaad0a35d3).

## Usage

1. Use the `train_VGGCAM` function to fine tune the VGG16 model on your data. You should write your own code to feed the data into the network.
2. Use the `plot_classmap` function to then plot the class activation map on an image specified by its path.

## Example plot

On the Kaggle StateFarm dataset:

![Drive + Phone 1](example_VGG16CAM1.png)
![Drive + Phone 2](example_VGG16CAM2.png)

The network is focusing on the cell phone the driver is holding, regardless of driver ID or hand position.
