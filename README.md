# MNIST Digit Classifier from Scratch

This project implements a simple feedforward neural network from scratch using only NumPy, Pandas, and Matplotlib to classify handwritten digits from the MNIST dataset.

## 🧠 Project Overview

The neural network has the following architecture:

- **Input layer**: 784 nodes (28x28 pixel grayscale images)
- **Hidden layer**: 10 neurons with ReLU activation
- **Output layer**: 10 neurons with softmax activation (for digit classes 0–9)

The code trains the model using gradient descent and evaluates its performance on both a training set and a development (dev) set.

## 📁 Files

- `train.csv`: CSV file containing the MNIST training data (labels + flattened pixel values).
- `mnist.py` or main script: Contains all the code to load data, initialize parameters, forward and backpropagate, update weights, make predictions, and visualize results.

## 🚀 How It Works

1. **Data Loading**: The `train.csv` file is loaded using `pandas` and split into training and dev sets.
2. **Preprocessing**: Pixel values are normalized to the range [0, 1].
3. **Training**: The model is trained with a custom implementation of:
    - Forward propagation
    - ReLU and Softmax activations
    - One-hot encoding of labels
    - Backpropagation
    - Parameter updates using gradient descent
4. **Evaluation**: Accuracy is printed during training and tested with a few examples.
5. **Visualization**: Uses Matplotlib to display individual digit predictions.
