Neural Network From Scratch with NumPy

A compact implementation of a feed-forward neural network built from scratch using NumPy, without using high-level deep-learning frameworks such as TensorFlow, PyTorch, or Keras.

The project uses the scikit-learn Digits dataset to demonstrate the fundamental components of neural-network training, including forward propagation, backpropagation, mini-batch gradient descent, activation functions, loss computation, and model evaluation.

🎯 Objective

The goal of this project was to understand the mechanics of a neural network by implementing the core training pipeline directly with NumPy rather than relying on a deep-learning framework.

The project focuses on the question:

«Can a small neural network implemented from first principles effectively learn handwritten digit classification?»

---

🧠 Model Architecture

The network is a simple multilayer perceptron:

Input Layer
   ↓
128-neuron Hidden Layer
   ↓
ReLU Activation
   ↓
10-neuron Output Layer
   ↓
Softmax

The input consists of the 8×8 grayscale digit images from the scikit-learn Digits dataset.

Implemented from scratch

- Xavier parameter initialization
- Forward propagation
- ReLU activation
- Softmax output
- Cross-entropy loss
- Backpropagation
- Mini-batch gradient descent
- Parameter updates
- Training/validation monitoring

---

📊 Dataset

The project uses the Digits dataset provided by scikit-learn.

- 1,797 handwritten digit samples
- 8 × 8 pixel images
- 10 classes: digits 0–9
- 64 input features after flattening

The input features are standardized before training.

---

⚙️ Training

Example configuration used in the experiment:

Parameter| Value
Hidden units| 128
Epochs| 40
Learning rate| 0.01
Random seed| 42
Batch training| Yes
Output classes| 10

The implementation uses separate training, validation, and test data to monitor generalization.

---

📈 Results

The trained network achieved:

Test Accuracy: 93.89%

Validation accuracy during training reached approximately 93.61%.

Training loss decreased consistently during optimization, while validation accuracy improved throughout most of the training process.

Model performance

The project also generates:

- Confusion matrix
- Classification report
- Training/validation metrics
- Saved model parameters
- Reproducibility metadata

---

🔬 Why Build a Neural Network From Scratch?

Modern frameworks make neural-network development extremely convenient, but they can hide many of the mathematical operations involved in training.

Implementing the network directly with NumPy provided an opportunity to understand:

Input → Forward Pass → Loss → Gradients → Backpropagation → Parameter Update

This project was therefore developed primarily as a study of the computational and mathematical foundations of neural networks.

---

🧪 Reproducibility

Random seeds are explicitly controlled so that the experiment can be reproduced with the same configuration.

The project records relevant training information and model metadata as part of the output artifacts.

---

🚀 Running the Project

Clone the repository:

git clone https://github.com/showravj2-create/neural-network-from-scratch/blob/main/neural_network_from_scratch.ipynb

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1srK6Lq_pBP4Vjjh7PmjGML9aNamFS0mp?usp=sharing)

Install the dependencies:

pip install -r requirements.txt

Then open:

neural_network_from_scratch.ipynb

in Jupyter Notebook or Google Colab and run the cells sequentially.

---

🛠️ Technologies

- Python
- NumPy
- scikit-learn
- Matplotlib
- Jupyter Notebook / Google Colab

---

🔭 Future Improvements

Possible extensions include:

- Comparing the NumPy implementation with PyTorch
- Implementing additional optimizers such as Adam
- Adding regularization
- Testing different network architectures
- Hyperparameter experiments
- Learning-rate scheduling
- Comparing different activation functions
- Applying the implementation to a larger dataset

---

👤 Author

Showrav Das

Mathematics Graduate interested in:

Machine Learning • Deep Learning • Computer Vision • Natural Language Processing

GitHub: "@showravj2-create" (https://github.com/showravj2-create)
