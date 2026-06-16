# MNIST Handwritten Digit Classification using TensorFlow

## Overview

This project implements a Multi-Layer Perceptron (MLP) using TensorFlow and Keras to classify handwritten digits from the MNIST dataset. The model is trained on 60,000 images and evaluated on 10,000 test images.

## Dataset

The MNIST dataset contains grayscale images of handwritten digits (0–9).

* Training samples: 60,000
* Test samples: 10,000
* Image size: 28 × 28 pixels
* Number of classes: 10

## Data Preprocessing

* Loaded the MNIST dataset using TensorFlow.
* Normalized pixel values from the range [0, 255] to [0, 1].

## Model Architecture

| Layer           | Output Shape |
| --------------- | ------------ |
| Flatten         | 784          |
| Dense (ReLU)    | 128          |
| Dense (ReLU)    | 64           |
| Dense (Softmax) | 10           |

### Model Summary

* Total Parameters: 109,386
* Trainable Parameters: 109,386

## Training Configuration

* Optimizer: Adam
* Loss Function: Sparse Categorical Crossentropy
* Metrics: Accuracy
* Epochs: 5
* Batch Size: 32
* Validation Split: 20%

## Results

### Training Performance

| Epoch | Validation Accuracy |
| ----- | ------------------- |
| 1     | 95.84%              |
| 2     | 96.67%              |
| 3     | 96.69%              |
| 4     | 97.01%              |
| 5     | 97.47%              |

### Test Performance

* Test Accuracy: 97.42%
* Test Loss: 0.0812

## Prediction Visualization

The model predicts the digit class for unseen test images and displays:

* Actual label
* Predicted label
* Corresponding handwritten digit image

## Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Matplotlib

## Key Learning Outcomes

* Image preprocessing and normalization
* Building neural networks using Keras Sequential API
* Understanding Flatten and Dense layers
* Multi-class classification with Softmax
* Model training, validation, and evaluation
* Visualizing predictions

## Run the Project

```bash
pip install tensorflow matplotlib numpy
```

```bash
python mnist_classification.py
```

## Author

Deep Learning experiments and implementations using TensorFlow and Keras.

