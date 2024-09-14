Fashion MNIST Image Classification with CNN in R
Project Description
This project demonstrates the implementation of a Convolutional Neural Network (CNN) using Keras and TensorFlow in R to classify images from the Fashion MNIST dataset. The dataset consists of 70,000 grayscale images of 10 different fashion categories, with 60,000 images for training and 10,000 for testing.

Tasks:
Implement a CNN with 6 layers to classify the Fashion MNIST dataset.
Train the model for 10 epochs.
Make predictions for test images.
Visualize the predictions and model performance.
Project Structure
fashion_mnist_classification.R: Main R script containing the code for data loading, CNN model definition, training, prediction, and evaluation.
README.md: This file, explaining the project and how to run the code.
requirements.txt: List of R packages and dependencies needed for this project.
How to Run the Code
Install R and RStudio (if not already installed).

Install Required Packages: Before running the script, install the necessary R packages.
install.packages(c("keras", "tensorflow", "ggplot2", "dplyr"))
library(keras)
library(tensorflow)
install_keras()  # Installs TensorFlow backend

Run the Script:

Open fashion_mnist_classification.R in RStudio.
Ensure that all libraries are loaded successfully.
Execute the script to load the Fashion MNIST dataset, define the CNN model, train it, and make predictions.
View Predictions: The script will make predictions on a few test images and print the predicted classes along with actual labels. You can also visualize a sample image with its predicted and actual class using ggplot2.
Model Overview
The CNN model is structured as follows:

Input Layer: 28x28 grayscale images (1 channel).
2 Convolutional Layers with ReLU activation and max pooling.
Flatten Layer to reshape the data for the dense layers.
Dense Layer with 128 units and ReLU activation.
Output Layer with 10 units and softmax activation for classification into one of 10 fashion categories.
Performance:
The model is trained for 10 epochs and evaluates its accuracy and loss using test data after training.

Dependencies
R version: >= 4.0
TensorFlow
Keras
ggplot2
dplyr
Additional Notes
Ensure that the tensorflow and keras packages are installed correctly and TensorFlow backend is working in R.
If you encounter errors related to TensorFlow or Keras installation, restart your R session or consult the TensorFlow for R documentation.
