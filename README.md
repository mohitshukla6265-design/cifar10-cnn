# CIFAR-10 Image Classification using CNN

A Deep Learning project that classifies images into 10 different categories using a Convolutional Neural Network (CNN). The project is implemented using TensorFlow, Keras, NumPy, and Matplotlib.

---

## Team Members

| Name | Contribution |
|--------|--------|
| Mohit Shukla | Dataset preprocessing, model training, GitHub repository management |
| Prashant Pujari | CNN architecture design, hyperparameter tuning, model evaluation |
| Md Aamish | Performance analysis, testing, documentation and README preparation |

---

## About the Project

This project uses a Convolutional Neural Network (CNN) to classify color images from the CIFAR-10 dataset. The model learns image features using convolutional layers and predicts one of the ten object categories.

The project also uses:

- Batch Normalization
- ReLU Activation
- Max Pooling
- Spatial Dropout
- L2 Regularization
- Custom Cross Entropy Loss Function

to improve performance and reduce overfitting.

---

## Dataset Information

**Dataset:** CIFAR-10

The dataset contains 60,000 color images of size 32×32 pixels belonging to 10 classes.

### Classes

| Class ID | Category |
|-----------|-----------|
| 0 | Airplane |
| 1 | Automobile |
| 2 | Bird |
| 3 | Cat |
| 4 | Deer |
| 5 | Dog |
| 6 | Frog |
| 7 | Horse |
| 8 | Ship |
| 9 | Truck |

---

## Technologies Used

- Python 3.x
- TensorFlow
- Keras
- NumPy
- Matplotlib

---

## Project Structure

```text
cifar10-cnn/
│
├── cnn_model.py
├── README.md
├── requirements.txt
│
├── outputs/
│   ├── accuracy_graph.png
│   ├── loss_graph.png
│
└── sample_predictions/
```

---

## Model Architecture

```text
Input Layer (32x32x3)
        │
        ▼
Conv2D (32 Filters)
        │
Batch Normalization
        │
ReLU
        │
Conv2D (32 Filters)
        │
Batch Normalization
        │
ReLU
        │
MaxPooling2D
        │
SpatialDropout2D (0.2)
        │
        ▼
Conv2D (64 Filters)
        │
Batch Normalization
        │
ReLU
        │
Conv2D (64 Filters)
        │
Batch Normalization
        │
ReLU
        │
MaxPooling2D
        │
SpatialDropout2D (0.3)
        │
        ▼
Flatten
        │
Dense (256)
        │
Batch Normalization
        │
ReLU
        │
Dropout (0.5)
        │
Dense (10)
        │
Softmax
```

---

## Training Configuration

| Parameter | Value |
|------------|---------|
| Optimizer | Adam |
| Learning Rate | 0.001 |
| Loss Function | Custom Cross Entropy |
| Epochs | 10 |
| Batch Size | 128 |
| Validation Split | 15% |

---

## Installation

### Clone the Repository

```bash
git clone https://github.com/mohitshukla6265-design/cifar10-cnn.git
cd cifar10-cnn
```

### Install Dependencies

```bash
pip install tensorflow numpy matplotlib
```

---

## Run the Project

```bash
python cnn_model.py
```

---

## How It Works

1. Load CIFAR-10 dataset
2. Normalize image pixel values
3. Build CNN architecture
4. Train the model
5. Evaluate on test data
6. Plot accuracy and loss graphs
7. Predict a random test image

---

## Sample Output

```text
Actual Class: Ship
Predicted Class: Ship
```

---

## Performance

| Metric | Value |
|----------|----------|
| Dataset | CIFAR-10 |
| Number of Classes | 10 |
| Expected Accuracy | 70% - 80% |
| Image Size | 32 × 32 × 3 |

---

## Output Graphs

The project generates:

- Training Accuracy Graph
- Validation Accuracy Graph
- Training Loss Graph
- Validation Loss Graph

---

## Features

- Color image classification
- Deep CNN architecture
- Custom loss function
- L2 regularization
- Spatial dropout
- Batch normalization
- Automatic sample prediction
- Performance visualization

---

## Future Improvements

- Data augmentation
- Transfer learning using ResNet or VGG16
- Hyperparameter optimization
- Model deployment using Flask or Streamlit

---

## Authors

# Mohit Shukla
## Prashant Pujari
### Md Aamish

---
