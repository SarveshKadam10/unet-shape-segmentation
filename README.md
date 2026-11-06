# U-Net Shape Segmentation

Binary image segmentation of synthetic geometric shapes using a compact U-Net.

## Overview

This project trains a U-Net to classify each pixel of a 128×128 grayscale image as either object or background. The synthetic dataset contains circles, squares, and triangles with corresponding binary segmentation masks.

## Dataset

- 1,000 training images
- 200 test images
- Image size: 128×128 grayscale
- Shapes: circles, squares, and triangles
- Binary masks: object = 1, background = 0

## Model

The compact U-Net consists of:

- Two encoder blocks with 16 and 32 filters
- 64-filter bottleneck
- Two decoder blocks with 32 and 16 filters
- Skip connections between encoder and decoder
- Sigmoid output for binary segmentation

## Training

- Optimizer: Adam
- Learning rate: 0.001
- Loss: Binary Cross-Entropy
- Batch size: 16
- Epochs: 15

## Results

- Test Accuracy: 1.000
- Test IoU: 1.000
- TP: 214,160
- TN: 3,062,640
- FP: 0
- FN: 0

## Implementation

The complete implementation, training procedure, evaluation metrics, architecture visualization, learning curve, and segmentation examples are included in the Jupyter notebook.
