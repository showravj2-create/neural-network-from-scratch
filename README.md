Neural Network From Scratch with NumPy

A from-scratch implementation of a feed-forward neural network using NumPy, without relying on high-level deep-learning frameworks such as TensorFlow, PyTorch, or Keras.

The project uses the scikit-learn Digits dataset to demonstrate the mathematical and computational foundations of neural-network training, including forward propagation, backpropagation, activation functions, cross-entropy loss, mini-batch gradient descent, parameter optimization, and model evaluation.

[![Open In 
Colab(https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1srK6Lq_pBP4Vjjh7PmjGML9aNamFS0mp?usp=sharing)

---

🎯 Objective

The primary objective of this project was to understand how a neural network learns by implementing its core computational pipeline directly with NumPy rather than using an existing deep-learning framework.

The project investigates the following question:

«Can a small neural network implemented from first principles learn handwritten digit classification effectively?»

The implementation focuses on understanding the mathematical relationship between:

Input → Forward Propagation → Loss → Gradients → Backpropagation → Parameter Update

---

🧠 Model Architecture

The model is a simple Multilayer Perceptron (MLP):

8 × 8 Input Image
       ↓
  64 Input Features
       ↓
  128 Hidden Neurons
       ↓
   ReLU Activation
       ↓
  10 Output Neurons
       ↓
      Softmax
       ↓
 Digit Prediction (0–9)

Implemented from scratch

- Xavier parameter initialization
- Forward propagation
- ReLU activation
- Softmax output layer
- Cross-entropy loss
- Backpropagation
- Mini-batch gradient descent
- Parameter updates
- Training/validation monitoring

No high-level neural-network training API was used.

---

📊 Dataset

The experiment uses the Digits dataset provided by scikit-learn.

Property| Value
Samples| 1,797
Image dimensions| 8 × 8
Input features| 64
Classes| 10
Classes| Digits 0–9

The images are flattened into 64-dimensional feature vectors and the input features are standardized before training.

---

⚙️ Training Configuration

The experiment was conducted using the following configuration:

Parameter| Value
Hidden units| 128
Epochs| 40
Learning rate| 0.01
Random seed| 42
Batch training| Mini-batch
Output classes| 10

The dataset is separated into training, validation, and test sets to evaluate both optimization progress and generalization.

---

📈 Results

The trained neural network achieved:

Test Accuracy: 93.89%

Validation accuracy reached approximately 93.61% during training.

The training process showed a consistent reduction in loss while validation accuracy improved through most of the optimization process, indicating that the network successfully learned useful representations of the handwritten digits.

Evaluation artifacts

The experiment produces:

- Training curve
- Validation metrics
- Confusion matrix
- Classification report
- Saved model parameters
- Training metadata

These artifacts are available in the ""results/"" (results/) directory.

---

🔬 Why Build a Neural Network From Scratch?

Modern deep-learning frameworks make it possible to train neural networks with only a few lines of code. However, these abstractions can hide many of the mathematical operations involved in learning.

Implementing the model directly with NumPy provides a clearer understanding of:

- Matrix multiplication
- Activation functions
- Probability distributions
- Loss functions
- Gradient computation
- Chain-rule-based backpropagation
- Parameter optimization
- Mini-batch training

This project was therefore designed primarily as an exploration of the mathematical and computational foundations of neural networks.

---

🧪 Reproducibility

Random seeds are explicitly controlled to make the experiment reproducible.

The repository also stores relevant experiment metadata and model artifacts generated during training.

---

🚀 Running the Project

Google Colab

The notebook can be opened directly in Google Colab:

""Open In Colab" (https://colab.research.google.com/assets/colab-badge.svg)" (https://colab.research.google.com/drive/1srK6Lq_pBP4Vjjh7PmjGML9aNamFS0mp?usp=sharing)

Local environment

Clone the repository:

git clone https://github.com/showravj2-create/neural-network-from-scratch.git
cd neural-network-from-scratch

Install the required dependencies:

pip install -r requirements.txt

Then open:

neural_network_from_scratch.ipynb

using Jupyter Notebook or JupyterLab.

---

📁 Repository Structure

neural-network-from-scratch/
│
├── README.md
├── neural_network_from_scratch.ipynb
├── requirements.txt
├── LICENSE
│
└── results/
    ├── training_curve.png
    ├── confusion_matrix.png
    ├── classification_report.txt
    ├── metadata.json
    └── model.npz

---

🛠️ Technologies

- Python
- NumPy
- scikit-learn
- Matplotlib
- Jupyter Notebook
- Google Colab

---

🔭 Future Improvements

Possible extensions include:

- Comparing the NumPy implementation with PyTorch
- Implementing additional optimizers such as Adam
- Adding L2 regularization
- Experimenting with different network architectures
- Performing systematic hyperparameter experiments
- Implementing learning-rate scheduling
- Comparing different activation functions
- Evaluating the model on larger datasets

---

👤 Author

Showrav Das

Mathematics graduate interested in:

Machine Learning • Deep Learning • Computer Vision • Natural Language Processing

GitHub: "@showravj2-create" (https://github.com/showravj2-create)
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
