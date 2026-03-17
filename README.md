# Plant Disease Recognition with AlexNet
## Overview

This project focuses on plant leaf disease classification using a convolutional neural network inspired by AlexNet. The objective is to classify leaf images into three categories: Healthy, Powdery, and Rust. Beyond building a baseline CNN, the project also explores performance improvements through augmentation, weight initialization, and activation-function tuning.

## My Contribution

Although this was submitted as a group course project, I led and completed the majority of the work end to end, including:

literature review

experiment design and iteration planning

model development and training

evaluation of alternative configurations

report writing and presentation preparation

## Dataset

The model was trained on the Plant Disease Recognition Dataset from Kaggle, which contains plant leaf images labeled under three classes:

Healthy

Powdery

Rust

The dataset includes approximately 1,530 images and is split into training, validation, and test sets. This project uses the dataset for supervised image classification and applies preprocessing and augmentation to improve generalization on a relatively small image corpus.

Dataset source:
Plant Disease Recognition Dataset on Kaggle, Link: https://www.kaggle.com/datasets/rashikrahmanpritom/plant-disease-recognition-dataset

## Methodology,

The project followed this workflow:

Load and preprocess images using ImageDataGenerator

Apply augmentation techniques such as rotation, zoom, shear, and shifting

Train an AlexNet-style CNN on RGB leaf images

Compare different epoch and batch-size settings

Test He initialization

Analyze the impact of dead neurons in ReLU-based networks

Compare ReLU, LeakyReLU, and PReLU activation functions

The implementation was built with TensorFlow/Keras and includes a deep CNN architecture with convolutional layers, pooling, dense layers, and dropout. The notebook also documents training and validation behavior across multiple experiments.

## Key Findings

Data augmentation helped improve robustness on a relatively limited dataset.

He initialization improved convergence behavior for ReLU-based layers.

The project explicitly investigated the dead-neuron problem in ReLU networks.

Among the tested configurations, He initialization + LeakyReLU produced the best results according to the final report.

## Tech Stack

Python

TensorFlow / Keras

NumPy

Matplotlib

## Repository Contents

main.ipynb — notebook containing preprocessing, training, and evaluation

PlantDiseaseRecognition.pdf — final project report

## Notes

This project was completed before I started consistently using GitHub for version control, so some earlier experimental iterations and intermediate notebooks were not preserved.
