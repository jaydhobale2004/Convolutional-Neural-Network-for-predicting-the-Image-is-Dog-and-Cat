[README_CNN_Dog_vs_Cat.md](https://github.com/user-attachments/files/26058804/README_CNN_Dog_vs_Cat.md)
# Convolutional Neural Network for Dog vs Cat Image Classification

A **Convolutional Neural Network (CNN)** project for classifying images as either **dog** or **cat** using TensorFlow / Keras.

## Overview

This project applies deep learning to a classic binary image classification problem. The notebook builds and trains a CNN that learns visual patterns from labeled image folders and then predicts whether a new image belongs to the dog or cat class.

The workflow includes:

- image preprocessing with augmentation
- creation of training and test image generators
- CNN model construction
- model training
- single-image prediction

## Tech Stack

- **Python**
- **TensorFlow / Keras**
- **ImageDataGenerator**
- **Jupyter Notebook / Google Colab**

## Model Architecture

The CNN is built using `tf.keras.Sequential` and includes:

- convolution layer with 32 filters
- max pooling
- second convolution layer with 32 filters
- second max pooling layer
- flatten layer
- dense hidden layer with 128 units
- sigmoid output layer for binary classification

Training configuration:

- **Input size:** 64 × 64
- **Batch size:** 32
- **Epochs:** 25
- **Loss:** Binary Crossentropy
- **Optimizer:** Adam

## Data Pipeline

The notebook expects the dataset in this structure:

```text
dataset/
├── training_set/
├── test_set/
└── single_prediction/
```

Training images are augmented using:

- rescaling
- shear transformation
- zoom
- horizontal flipping

Test images are rescaled before inference.

## Repository Contents

```text
Convolutional-Neural-Network-for-predicting-the-Image-is-Dog-and-Cat/
└── Copy_of_cnn.ipynb
```

## How to Run

1. Clone the repository.
2. Install dependencies:
   ```bash
   pip install tensorflow
   ```
3. Place the image dataset in the expected folder structure.
4. Open the notebook:
   ```bash
   jupyter notebook Copy_of_cnn.ipynb
   ```
5. Run all cells in order.

## Potential Improvements

- add dataset download instructions
- save the trained model as `.h5` or `.keras`
- include accuracy/loss plots
- add sample prediction screenshots
- compare performance with transfer learning models such as MobileNet or ResNet
- move notebook code into reusable Python scripts

## Why This Project Matters

This project demonstrates:

- practical computer vision fundamentals
- CNN-based image classification
- image preprocessing and augmentation
- TensorFlow / Keras workflow for deep learning

## Author

**Jay Dhobale**
