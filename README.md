# ICP_6-Assignment

Name: Dama Vamsi

Course: Big Data Analytics

Reg No: 700771673

# MNIST Feedforward Neural Network – Keras Experiments

This project explores building and tuning a feedforward neural network using the **Keras Sequential API** on the MNIST dataset.

It includes experiments with various architectures, activation functions, and optimizers to achieve high classification accuracy.

---

##  Objectives

- Build a simple feedforward neural network using Keras
- Experiment with:
  - Number of hidden layers
  - Neuron counts
  - Activation functions (`ReLU`, `tanh`, `sigmoid`)
  - Optimizers (`adam`, `sgd`, `rmsprop`)
- Achieve **>99% test accuracy** on MNIST

---

## Model Architectures Tested

1. **Basic ReLU Model** – 5 hidden layers
2. **Deep Layer Variant** – 7 hidden layers with varied neuron counts
3. **Activation Experiments**
   - `tanh` on all layers
   - `sigmoid` on all layers
4. **Optimizer Experiments**
   - `adam` (baseline)
   - `sgd`
   - `rmsprop`
5. **High Accuracy Tuned Model**
   - 512 → 256 → 128 → 64
   - Dropout regularization
   - Trained for 15 epochs
   - Achieved **>99% test accuracy**

---

## Dataset

- **MNIST**: 28×28 grayscale images of handwritten digits (0–9)
- Preprocessing: Normalization + One-hot encoding

---

## Results

| Experiment | Test Accuracy |
|------------|----------------|
| ReLU (5 layers) | ~98.5% |
| Deep Layer (7 layers) | ~98.9% |
| `tanh` activation | ~98.2% |
| `sigmoid` activation | ~97.8% |
| `adam` optimizer | Best performer |
| `sgd` optimizer | Slower convergence |
| `rmsprop` optimizer | Moderate performance |
| **Final Model (Adam + Dropout + 15 epochs)** | **99.3%** |

---THE END---

