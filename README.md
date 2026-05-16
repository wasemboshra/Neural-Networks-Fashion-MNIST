# Fashion-MNIST Image Classification using MLP
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1AlGowtevBHg7Wl200lCkvC2yVot3mhln?usp=sharing)

## 1. Problem Description
This project aims to classify clothing images from the official Fashion-MNIST dataset into 10 distinct categories. The model is designed using a Multilayer Perceptron (MLP) architecture built via TensorFlow and Keras to satisfy the course project requirements.

## 2. Dataset Link
The dataset is loaded directly from Keras datasets, but the formal source and documentation can be accessed here:
* [Fashion-MNIST on GitHub](https://github.com/zalandoresearch/fashion-mnist)

## 3. Results & Experiments Comparison

| Metric | Experiment 1 (Base Model) | Experiment 2 (Modified Parameters) |
| :--- | :---: | :---: |
| **Hidden Layer Neurons** | 128 Neurons | 256 Neurons |
| **Activation Function** | ReLU | ReLU |
| **Learning Rate (LR)** | 0.001 | 0.01 |
| **Final Test Loss** | 0.3368 | 0.4323 |
| **Final Test Accuracy** | 88.20% | 86.20% |

### Analysis:
* **Experiment 1** achieved a higher accuracy (88.20%) and lower loss because a learning rate of 0.001 is well-optimized for the Adam optimizer on this task.
* **Experiment 2** had more capacity (256 neurons) but expanding the learning rate to 0.01 caused the model to overshoot optimal weights slightly, leading to a minor drop in accuracy (86.20%).

## 4. Project Structure & Requirements Checklist
- [x] **Data Preprocessing:** Images normalized and labels encoded using One-Hot encoding.
- [x] **Model Architecture:** MLP structure initialized using standard Sequential.
- [x] **Loss & Performance Monitoring:** Categorical Crossentropy applied.
- [x] **Visualization:** Training vs Validation loss and accuracy curves plotted.

## 5. Instructions for Running the Project
1. Clone this repository to your machine.
2. Install the necessary dependencies:
   ```bash
   pip install tensorflow numpy matplotlib
