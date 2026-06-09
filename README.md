CIFAR-10 Image Classification using CNN

A deep learning project that classifies images into 10 different object categories using a Convolutional Neural Network (CNN). This project was developed using Python, TensorFlow, and Keras to demonstrate image classification on the CIFAR-10 dataset.

Team Members
Member	Work Done
Mohit Shukla	Dataset preprocessing, model training, GitHub repository management
Prashant Pujari	CNN architecture design, hyperparameter tuning, model evaluation
Md Aamish	Data analysis, performance visualization, documentation and testing

About the Project

This project uses a Convolutional Neural Network (CNN) to classify color images from the CIFAR-10 dataset. The model learns image features through convolution and pooling operations and predicts one of the ten object classes. Regularization techniques such as Batch Normalization, Dropout, Spatial Dropout, and L2 Regularization are used to improve generalization and reduce overfitting.

Classes Recognized
No.	Class
1	Airplane
2	Automobile
3	Bird
4	Cat
5	Deer
6	Dog
7	Frog
8	Horse
9	Ship
10	Truck
Tech Stack
Python 3.x
TensorFlow
Keras
NumPy
Matplotlib
CNN (Convolutional Neural Network)
Project Structure
cifar10-cnn/
│
├── cnn_model.py
├── README.md
├── requirements.txt
├── outputs/
│   ├── accuracy_graph.png
│   ├── loss_graph.png
│
└── sample_predictions/
How to Run
1. Clone the Repository
git clone https://github.com/mohitshukla6265-design/cifar10-cnn.git
cd cifar10-cnn
2. Install Dependencies
pip install tensorflow numpy matplotlib
3. Run the Project
python cnn_model.py
How the Model Works
Loads CIFAR-10 dataset from TensorFlow.
Normalizes image pixel values between 0 and 1.
Applies convolution layers for feature extraction.
Uses Batch Normalization and ReLU activation.
Applies Max Pooling to reduce dimensions.
Uses Spatial Dropout and L2 Regularization to reduce overfitting.
Flattens extracted features.
Uses Dense layers for classification.
Predicts one of the 10 CIFAR-10 classes using Softmax activation.
Model Architecture
Input Layer (32x32x3)
        │
Conv2D (32)
        │
Batch Normalization
        │
ReLU
        │
Conv2D (32)
        │
Batch Normalization
        │
ReLU
        │
MaxPooling
        │
SpatialDropout
        │
Conv2D (64)
        │
Batch Normalization
        │
ReLU
        │
Conv2D (64)
        │
Batch Normalization
        │
ReLU
        │
MaxPooling
        │
SpatialDropout
        │
Flatten
        │
Dense (256)
        │
Dropout (0.5)
        │
Dense (10, Softmax)
Training Details
Setting	Value
Optimizer	Adam
Learning Rate	0.001
Loss Function	Custom Cross Entropy
Epochs	10
Batch Size	128
Validation Split	15%
Dataset	CIFAR-10
Output Graphs

After training, the following graphs are generated:

Accuracy Graph
Training Accuracy
Validation Accuracy
Loss Graph
Training Loss
Validation Loss
Sample Prediction

The model randomly selects an image from the test dataset and predicts its class.

Example:

Actual Class: Ship
Predicted Class: Ship
Expected Performance
Metric	Value
Test Accuracy	70% - 80%
Dataset	CIFAR-10
Number of Classes	10
Conclusion

The CNN model successfully classifies CIFAR-10 images with good accuracy. The use of convolution layers, batch normalization, dropout, and regularization helps the model learn meaningful image features while reducing overfitting. This project demonstrates the practical application of deep learning techniques for image classification tasks.

Authors
Mohit Shukla
Prashant Pujari
Md Aamish
