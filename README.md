# Neural Network Regularization: Dropout & Early Stopping

A hands-on deep learning project demonstrating how **Dropout** and **Early Stopping** help reduce overfitting and improve the generalization ability of neural networks.

This repository contains two end-to-end implementations:

- Customer Churn Prediction (Regression)
- MNIST Digit Classification

Both projects were implemented using TensorFlow/Keras and focus on understanding the practical impact of regularization techniques rather than maximizing benchmark performance.

---

## Objectives

This project was built to gain hands-on understanding of:

- Neural Network training
- Overfitting
- Validation Monitoring
- Dropout Regularization
- Early Stopping
- Learning Curves
- Generalization Performance

---

# Project Structure

```
.
├── Customer_Churn_prediction.ipynb
├── MNIST_Classification_with_dropout_and_Early_Stopping.ipynb
├── README.md
└── images/
```

---

# Project 1 — Customer Churn Prediction

## Goal

Predict customer churn using a fully connected neural network.

### Techniques Used

- Data preprocessing
- Feature Scaling
- Dense Neural Network
- Dropout
- EarlyStopping Callback
- Validation Monitoring

---

## Results


| Metric | Value |
|---------|------:|
| Training Loss |0.36 |
| Validation Loss | 0.35|
| Test accuracy |0.85 |

---

## Training Curves

### Loss Curve

> Insert image here

```
images/churn_loss.png
```

---

## Observation

An interesting observation was that the validation loss became slightly lower than the training loss.

This occurs because Dropout is enabled only during training, making the optimization problem intentionally harder. During validation, all neurons participate in prediction, leading to improved performance and demonstrating the effectiveness of dropout as a regularization technique.

---

# Project 2 — MNIST Classification

## Goal

Classify handwritten digits using a feed-forward neural network.

### Techniques Used

- Dense Neural Network
- ReLU Activation
- Softmax Output
- Dropout
- EarlyStopping
- Validation Split

---

## Results

| Metric | Value |
|---------|------:|
| Training Accuracy | 0.98|
| Validation Accuracy | 0.97|
| Test Accuracy | 0.97|

---

## Accuracy Curves

> Insert image here

```
images/mnist_accuracy.png
```

---

## Loss Curves

> Insert image here

```
images/mnist_loss.png
```

---

# Key Takeaways

Through these implementations I developed practical understanding of:

- Why neural networks overfit
- How Dropout prevents co-adaptation of neurons
- Why validation performance can exceed training performance when using Dropout
- How Early Stopping prevents unnecessary training after convergence
- Monitoring learning curves to diagnose underfitting and overfitting
- Building complete TensorFlow/Keras training pipelines

---

# Tech Stack

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

---

# Future Improvements

- Batch Normalization
- L2 Regularization
- Hyperparameter Tuning
- Learning Rate Scheduling
- TensorBoard Visualization
- Model Checkpointing
- Cross Validation
- Hyperparameter Search (Optuna/KerasTuner)

---

# License

MIT License
