# Assignment 12 - Neural Network and Deep Learning Basics

## Student

**Name: OBAJE PAUL**

## Project Overview

This project focuses on applying neural networks and deep learning concepts to image classification. The CIFAR-10 dataset is used to train and evaluate feedforward neural network models that classify images into ten different object categories.

The project demonstrates the complete machine learning workflow, including dataset preparation, image preprocessing, neural network development, model training, evaluation, experimentation, and analysis.

## Dataset

The project uses the **CIFAR-10** image classification dataset.

CIFAR-10 contains 60,000 colour images divided into 10 classes:

- Airplane
- Automobile
- Bird
- Cat
- Deer
- Dog
- Frog
- Horse
- Ship
- Truck

The dataset contains 50,000 training images and 10,000 test images. Each image has a size of 32 × 32 pixels with three colour channels.

## Objectives

The main objectives of this project are to:

1. Load and explore the CIFAR-10 dataset.
2. Visualize sample images from the different classes.
3. Normalize image pixel values.
4. Build a simple feedforward neural network.
5. Train the model using the Adam optimizer.
6. Evaluate the model using accuracy, precision, recall, and F1-score.
7. Generate a classification report and confusion matrix.
8. Experiment with different neural network architectures.
9. Investigate the effect of data augmentation.
10. Discuss practical applications and limitations of neural networks for image classification.

## Technologies Used

- Python
- Google Colab
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Methodology

### 1. Data Preparation

The CIFAR-10 dataset is loaded using TensorFlow/Keras. Sample images are visualized to understand the different categories represented in the dataset.

### 2. Image Preprocessing

The image pixel values are converted from the original 0-255 range to values between 0 and 1.

The class labels are also converted into categorical form so that categorical crossentropy can be used as the loss function.

### 3. Baseline Neural Network

A simple feedforward neural network is created using:

- Flatten layer
- Dense hidden layer
- ReLU activation
- Softmax output layer
- Adam optimizer
- Categorical crossentropy loss
- Accuracy metric

### 4. Improved Neural Network

A second model is developed with additional hidden layers and a larger number of neurons. Dropout layers are also introduced to help reduce overfitting.

### 5. Data Augmentation

Data augmentation is applied using:

- Rotation
- Width shifting
- Height shifting
- Horizontal flipping

The augmented model is then compared with the other models.

## Model Evaluation

The models are evaluated using:

- Test accuracy
- Precision
- Recall
- F1-score
- Classification report
- Confusion matrix

Training and validation accuracy and loss are also visualized using graphs.

## Model Comparison

Three models are evaluated:

| Model | Description |
|---|---|
| Baseline Model | Simple feedforward neural network |
| Improved Model | Additional layers, larger hidden layers and dropout |
| Augmented Model | Improved architecture trained with augmented images |

The final accuracy values are recorded in the notebook after training.

## Results

The final results obtained from the experiments will be reported here after completing the model training.

### Baseline Accuracy

_To be added from the Google Colab results._

### Improved Model Accuracy

_To be added from the Google Colab results._

### Augmented Model Accuracy

_To be added from the Google Colab results._

### Best Model

_To be added after comparing the three models._

## Classification and Confusion Matrix

The final model is evaluated using a classification report containing precision, recall, and F1-score for each CIFAR-10 class.

A confusion matrix is also generated to identify classes that the model classifies correctly and classes that are frequently confused with one another.

## Practical Application

A neural network image classification system could be used in digital media platforms to automatically categorize uploaded images.

For example, an image management system could identify whether an uploaded image contains an airplane, vehicle, animal, or another object. This could reduce the amount of manual image organization required.

The system could be scaled to process large numbers of images and could be integrated into a web or mobile application through an API.

## Challenges and Limitations

The CIFAR-10 images are relatively small, which makes some classes difficult to distinguish.

Some categories have visually similar characteristics. For example, the model may confuse cats and dogs or automobiles and trucks.

Another limitation is that a simple feedforward neural network does not specifically learn spatial image features in the same way that a convolutional neural network does.

## Future Work

Future work could investigate convolutional neural networks (CNNs), which are specifically designed for image-related tasks.

Additional experiments could also investigate:

- More neural network architectures
- Different optimizers
- More training epochs
- Additional augmentation techniques
- Hyperparameter tuning
- Transfer learning

## Files

The repository will contain:

- `Assignment12_Neural_Network.ipynb` - Google Colab/Jupyter notebook containing the complete implementation.
- `README.md` - Project documentation.
- `cifar10_neural_network.keras` - Saved trained neural network model.
- `classification_report.txt` - Classification results.
- `model_results.txt` - Comparison of model performance.

## Conclusion

This project demonstrates the process of developing and evaluating neural network models for image classification using the CIFAR-10 dataset.

The experiments compare a baseline feedforward neural network with an improved architecture and an augmented model. The results demonstrate how changes to model architecture and training data can affect classification performance.

The project also provides practical experience with preprocessing, model training, performance evaluation, visualization, and the use of neural networks for real-world image classification applications.
