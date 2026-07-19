# 👕 Fashion MNIST Image Classification using Deep Learning (ANN)

This project implements an **Artificial Neural Network (ANN)** using **TensorFlow/Keras** to classify images from the **Fashion MNIST** dataset. The model is trained to recognize different types of clothing items such as T-shirts, Shoes, Dresses, Bags, and more.

---

## 📌 Project Overview

The objective of this project is to build a Deep Learning model that can automatically classify grayscale clothing images into one of the **10 Fashion MNIST categories**.

The project includes:

- Data Loading
- Data Preprocessing
- Feature Normalization
- One-Hot Encoding
- ANN Model Building
- Model Training
- Model Evaluation
- Confusion Matrix
- Accuracy & Loss Graphs
- Model Saving
- Inference on Test Images

---

## 🛠️ Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-Learn
- TensorFlow
- Keras

---

## 📂 Dataset

Dataset Used:

Fashion MNIST Dataset

Files:

- fashion-mnist_train.csv
- fashion-mnist_test.csv

Image Size:

28 × 28 pixels

Number of Classes:

10

---

## 👕 Classes

| Label | Class Name |
|--------|------------|
| 0 | T-shirt/top |
| 1 | Trouser |
| 2 | Pullover |
| 3 | Dress |
| 4 | Coat |
| 5 | Sandal |
| 6 | Shirt |
| 7 | Sneaker |
| 8 | Bag |
| 9 | Ankle Boot |

---

# 📌 Project Workflow

```
Load Dataset
      │
      ▼
Separate Features & Labels
      │
      ▼
Normalize Pixel Values
      │
      ▼
One-Hot Encoding
      │
      ▼
Visualize Images
      │
      ▼
Build ANN Model
      │
      ▼
Compile Model
      │
      ▼
Train Model
      │
      ▼
Evaluate Accuracy
      │
      ▼
Confusion Matrix
      │
      ▼
Save Model
      │
      ▼
Inference (Prediction)
```

---

# 📖 Step-by-Step Explanation

## 1. Import Libraries

Import all required Python libraries for data processing, visualization, machine learning, and deep learning.

Libraries used:

- NumPy
- Pandas
- Matplotlib
- TensorFlow
- Keras
- Scikit-Learn

---

## 2. Load Dataset

The Fashion MNIST CSV files are loaded into Pandas DataFrames.

Training dataset is used to train the model.

Testing dataset is used for evaluation.

---

## 3. Separate Features and Labels

The dataset contains:

- Label column (target)
- 784 pixel columns (features)

Features:

```
X_train
X_test
```

Labels:

```
y_train
y_test
```

---

## 4. Normalize Pixel Values

Pixel values range between:

```
0 → 255
```

They are normalized into

```
0 → 1
```

using:

```
Pixel / 255
```

Normalization helps the neural network learn faster and improves accuracy.

---

## 5. One-Hot Encoding

Class labels are converted into categorical vectors.

Example:

```
Label = 2

↓

[0 0 1 0 0 0 0 0 0 0]
```

This format is required for multi-class classification.

---

## 6. Visualize Sample Image

A sample Fashion MNIST image is displayed using Matplotlib.

This helps verify that the dataset is loaded correctly.

---

## 7. Build ANN Model

A Sequential Neural Network is created.

Architecture:

Input Layer

↓

Hidden Layer (Dense + ReLU)

↓

Hidden Layer (Dense + ReLU)

↓

Output Layer (10 Neurons + Softmax)

Softmax returns probabilities for all clothing classes.

---

## 8. Compile Model

Optimizer:

Adam

Loss Function:

Categorical Crossentropy

Metric:

Accuracy

---

## 9. Train Model

The ANN learns from the training images.

Training includes:

- Forward Propagation
- Loss Calculation
- Backpropagation
- Weight Updates

Training history stores:

- Accuracy
- Loss

---

## 10. Evaluate Model

The trained model is tested using unseen images.

Metrics:

- Test Accuracy
- Test Loss

These indicate the model's performance.

---

## 11. Generate Predictions

The model predicts probabilities for every test image.

The class with the highest probability is selected as the predicted label.

---

## 12. Confusion Matrix

A confusion matrix compares:

Actual Labels

vs

Predicted Labels

It helps identify which classes are classified correctly or incorrectly.

---

## 13. Classification Report

Evaluation metrics include:

- Precision
- Recall
- F1-Score
- Accuracy

These provide a detailed performance analysis for each class.

---

## 14. Plot Accuracy Graph

Training accuracy is plotted over epochs.

This graph shows how the model improves during training.

---

## 15. Plot Loss Graph

Training loss is plotted over epochs.

A decreasing loss indicates that the model is learning effectively.

---

## 16. Save Model

The trained ANN model is saved as:

```
fashion_mnist_dl_model.h5
```

The saved model can later be loaded without retraining.

---

## 17. Inference

Inference means using the trained model to predict the class of a new image.

Steps:

1. Load test image
2. Normalize image
3. Predict probabilities
4. Find highest probability
5. Display predicted label
6. Compare with actual label
7. Visualize image

Example Output:

```
Predicted Class : Sneaker

Actual Class : Sneaker
```

---

# 📊 Model Evaluation

The notebook evaluates the model using:

- Test Accuracy
- Test Loss
- Confusion Matrix
- Classification Report
- Accuracy Curve
- Loss Curve

---

# 📁 Project Structure

```
Fashion-MNIST-Deep-Learning/
│
├── DEEP_LEARNING.ipynb
├── fashion-mnist_train.csv
├── fashion-mnist_test.csv
├── fashion_mnist_dl_model.h5
├── README.md
└── requirements.txt
```

---

# ▶️ How to Run

Clone the repository:

```bash
git clone https://github.com/yourusername/Fashion-MNIST-Deep-Learning.git
```

Install dependencies:

```bash
pip install numpy pandas matplotlib scikit-learn tensorflow
```

Run:

```bash
jupyter notebook
```

Open:

```
DEEP_LEARNING.ipynb
```

Run all cells sequentially.

---

# 🎯 Learning Outcomes

After completing this project, you will understand:

- Image Classification
- Artificial Neural Networks (ANN)
- Data Preprocessing
- One-Hot Encoding
- Model Training
- Model Evaluation
- Confusion Matrix
- Classification Report
- Deep Learning Inference
- TensorFlow & Keras Workflow

---

# 🚀 Future Improvements

- Implement Convolutional Neural Networks (CNN)
- Add Data Augmentation
- Hyperparameter Tuning
- Early Stopping
- Dropout Regularization
- Batch Normalization
- Deploy using Streamlit or Flask
- Convert model to TensorFlow Lite for mobile deployment

---

# 👨‍💻 Author

**Rahul**

B.Tech CSE (AI & ML)

Deep Learning Project using TensorFlow/Keras.
