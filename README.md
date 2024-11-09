# UNet Image Segmentation Model
 This repository contains an implementation of a UNet model for binary image segmentation using TensorFlow and Keras. The model is applied to a synthetic dataset created from a single image, where a simple 
 thresholding technique generates a binary mask. The UNet model is trained to segment this mask.
## Table of Contents

-[About the Project]_(#About the Project)
-[Model Architecture]_(#Model Architecture)
-[Requirements]_(#Requirements)
-[Dataset]_(#Dataset)
-[Usage]_(#Usage)
-[Results]_(#Results)
-[License]_(#License)
 
## About the Project 
 This project demonstrates a basic UNet architecture for image segmentation. The UNet model is a common choice for biomedical image segmentation tasks due to its encoder-decoder structure, allowing it to learn 
 spatial and contextual information. The model is trained on a single synthetic dataset to predict binary masks from input images.

## Model Architecture 
1. Encoder: Successive convolutional layers followed by max pooling to capture features.
2. Bottleneck: The deepest part of the network where feature maps are at their smallest size.
3. Decoder: Transposed convolutional layers to upsample the feature maps and combine high-level and low-level features.
