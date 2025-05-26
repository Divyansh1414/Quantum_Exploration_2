# Quantum-Classical Hybrid Fraud Detection

[![Python](https://img.shields.io/badge/python-3.8-blue)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/tensorflow-2.4.0-orange)](https://www.tensorflow.org/)
[![PennyLane](https://img.shields.io/badge/pennylane-0.17.0-lightgrey)](https://pennylane.ai/)
[![Strawberry Fields](https://img.shields.io/badge/strawberryfields-0.18.0-purple)](https://strawberryfields.ai/)

A proof-of-concept hybrid quantum-classical neural network to detect credit card fraud, combining classical feed-forward layers with continuous-variable quantum layers (Strawberry Fields via PennyLane), all orchestrated in a Keras/TensorFlow pipeline.

---

## Features

- **Classical Preprocessing**  
  Standard scaling, train-test split, and one-hot encoding of binary labels.  

- **Classical Layers**  
  Two dense ELU-activated layers for initial feature extraction.

- **Quantum Layers**  
  Four parameterized continuous-variable layers:  
  1. Interferometer (beamsplitter + rotations)  
  2. Squeezing  
  3. Interferometer  
  4. Displacement + Kerr nonlinearity  

- **Hybrid Keras Model**  
  Wrapped as a `tf.keras.Sequential`, trained end-to-end with Adam and MSE loss.

- **Visualization**  
  Real-time loss and accuracy curves plotted via Matplotlib.

---


