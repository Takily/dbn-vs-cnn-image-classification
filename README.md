# DBN vs CNN: Image Classification Model Comparison

This project is a personal comparison between two deep learning models for image classification: a Deep Belief Network (DBN) and a Convolutional Neural Network (CNN). My goal was to explore how each architecture learns from image data, how their internal representations differ, and how well they classify items of clothing.

## 📚 Overview

- **DBN**: A generative model made of stacked Restricted Boltzmann Machines (RBMs), trained layer by layer and fine-tuned with a separate linear classifier.
- **CNN**: A standard convolutional neural network built with Keras and trained end-to-end using supervised learning.
- **Dataset**: FashionMNIST — grayscale images of clothing items (e.g., shirts, shoes, bags), 28x28 pixels.
- **Evaluation**: Accuracy, confusion matrix, and visual exploration of class predictions.

## 🧠 Models

### Deep Belief Network (DBN)
- I used a third-party PyTorch-based library to implement the DBN.
- I trained it layer by layer in an unsupervised way, then added a linear classifier on top.
- I used Optuna to find good hyperparameters and improved accuracy.
- I also extracted the hidden representations after each RBM layer to see how the features changed.

### Convolutional Neural Network (CNN)
- I built the CNN using Keras and TensorFlow.
- It includes Conv2D, MaxPooling, BatchNormalization, and Dense layers.
- It was trained in a fully supervised way with categorical crossentropy loss.

## 🔬 What I Explored

- I printed the mean and standard deviation of hidden representations in the DBN after each layer to get a sense of how the model transforms data.
- I visualized images from the dataset and checked their predicted labels to better understand model performance.
- I used confusion matrices to see which classes were most often confused with each other.


