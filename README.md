# UNet Image Segmentation Model

This repository contains an implementation of a UNet model for binary image segmentation using TensorFlow and Keras. The model is applied to a synthetic dataset created from a single image, where a simple thresholding technique is used to generate a binary mask. The UNet model is trained to segment this mask.

## Table of Contents

- [About the Project](#about-the-project)
- [Model Architecture](#model-architecture)
- [Requirements](#requirements)
- [Dataset](#dataset)
- [Usage](#usage)
- [Results](#results)
- [License](#license)

## About the Project

This project demonstrates a basic UNet architecture for image segmentation. The UNet model is a common choice for biomedical image segmentation tasks due to its encoder-decoder structure, allowing it to learn both spatial and contextual information. Here, the model is trained on a single synthetic dataset to predict binary masks from input images.

## Model Architecture

The UNet architecture includes:
1. **Encoder**: Successive convolutional layers followed by max pooling to capture features.
2. **Bottleneck**: The deepest part of the network where feature maps are at their smallest size.
3. **Decoder**: Transposed convolutional layers to upsample the feature maps and combine high-level and low-level features.

## Requirements

- Python 3.x
- TensorFlow 2.x
- NumPy
- PIL (Pillow)
- Matplotlib

You can install the required packages using:
```bash
pip install tensorflow numpy pillow matplotlib
