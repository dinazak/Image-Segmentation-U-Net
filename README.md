# Image Segmentation using U-Net

This repository contains code for performing image segmentation using the U-Net architecture. The project utilizes the Oxford-IIIT PET dataset for training and evaluation.

## Problem Description

The task is to perform image segmentation using the U-Net architecture. The U-Net model is trained to classify each pixel in the image into different classes. The project focuses on the segmentation of pet images from the Oxford-IIIT PET dataset.

## Dataset

The Oxford-IIIT PET dataset is used for this project. The dataset consists of images of cats and dogs along with their corresponding segmentation masks. The dataset is loaded using the TensorFlow Datasets library (`tfds.load('oxford_iiit_pet:3.*.*', with_info=True)`) and is split into training and validation sets.

## U-Net Architecture

The U-Net architecture is a popular model for image segmentation tasks. It consists of a contracting path (downsampling) and an expansive path (upsampling) with skip connections to capture both local and global image features. The model learns to classify each pixel in the image into different classes based on the training dataset.

## Implementation
The code is implemented using TensorFlow and TensorFlow Datasets. The U-Net model is built using the Keras API. The model is trained on the training set of the Oxford-IIIT PET dataset using appropriate loss functions for image segmentation. The trained model can be used to perform image segmentation on new images.
