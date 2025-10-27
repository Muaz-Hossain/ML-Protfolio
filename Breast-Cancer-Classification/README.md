# 🎗️ Breast Cancer Classification - Logistic Regression from Scratch

A complete implementation of Logistic Regression from scratch to classify breast cancer tumors as malignant or benign using the Wisconsin Breast Cancer dataset.

## 📊 Project Overview

- **Algorithm**: Logistic Regression implemented from scratch
- **Dataset**: Wisconsin Breast Cancer Dataset (569 samples, 30 features)
- **Accuracy**: **93.57%** on test data
- **Goal**: Binary classification (Malignant vs Benign tumors)

## 🛠️ Implementation Details

### Model Architecture
- **Forward Propagation**: Linear transformation + Sigmoid activation
- **Cost Function**: Binary Cross-Entropy with numerical stability (1e-8)
- **Backward Propagation**: Gradient computation using chain rule
- **Optimization**: Gradient Descent with learning rate = 0.01

### Key Features
✅ Pure NumPy implementation (No ML libraries for core algorithm)  
✅ Feature standardization  
✅ Train-test split (70-30)  
✅ Comprehensive evaluation metrics  

## 📈 Code Structure

```python
# 1. Data Loading & Preprocessing
data = load_breast_cancer()
x = (x - np.mean(x, axis=0)) / np.std(x, axis=0)

# 2. Model Components
def sigmoid(z):                    # Activation function
def fw_propagation(x, w, b):       # Forward pass
def cost_function(y, y_pred):      # Loss calculation
def backward_propagation(x, y, y_pred):  # Gradient computation
def update(w, b, dw, db, alpha):   # Parameter update

# 3. Training & Evaluation
def train(x, y, epochs, alpha):    # Training loop
def predict(x, w, b):              # Prediction function
def accuracy(y_true, y_pred):      # Accuracy calculation

