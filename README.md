# Fashion MNIST Neural Network with TensorFlow and Keras

This project demonstrates how to build, train, and evaluate a fully connected neural network (FCN) for image classification using the Fashion MNIST dataset. The project uses TensorFlow and Keras for deep learning tasks and Matplotlib for visualization.

## Dataset

The dataset used in this project is the **Fashion MNIST** dataset, which consists of 60,000 training images and 10,000 testing images of 28x28 grayscale images across 10 different categories. Each image corresponds to a clothing item.

## Project Structure

1. **Load Data**: 
   - The Fashion MNIST dataset is loaded directly from TensorFlow's built-in datasets.
   - The dataset is split into training and test sets.

2. **Data Preprocessing**:
   - The images are reshaped from 28x28 matrices into 1D vectors (flattened to 784 pixels).
   - Pixel values are normalized to be in the range of 0 to 1.
   - Labels are converted to one-hot encoding for classification.

3. **Neural Network Architecture**:
   - Input layer: 784 nodes (one for each pixel).
   - Hidden layer 1: 200 neurons, ReLU activation.
   - Hidden layer 2: 100 neurons, ReLU activation.
   - Output layer: 10 neurons, softmax activation (for 10 clothing categories).

4. **Model Compilation**:
   - Loss function: Categorical Cross-Entropy.
   - Optimizer: Stochastic Gradient Descent (SGD).
   - Metric: Accuracy.

5. **Training**:
   - The model is trained for 10 epochs with a batch size of 5.
   - Training time is recorded.

6. **Evaluation**:
   - Test accuracy is calculated.
   - Random samples from the test dataset are visualized with their predicted labels.

## Requirements

To run this project, you need the following dependencies:

- TensorFlow
- NumPy
- Matplotlib
- Scikit-learn

You can install the required dependencies using pip:

```bash
pip install tensorflow numpy matplotlib scikit-learn
