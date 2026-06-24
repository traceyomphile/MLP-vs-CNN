# MLP vs CNN for Image Classification

## Project Overview

This project investigates the performance of two neural network architectures for image classification tasks:

- Multi-Layer Perceptron (MLP)
- Convolutional Neural Network (CNN)

The work compares these models on two benchmark datasets:

- MNIST
- CIFAR-10

The study is structured around two main experimental components:

1. A complexity ladder comparison, where both architectures are evaluated on both datasets.
2. A parameter-budget challenge, where both models are constrained to a similar number of trainable parameters and compared under equal resource limits.

The objective is to evaluate not only predictive accuracy, but also the efficiency and suitability of each architecture for different types of image data.

---

## Assignment Context

This repository contains the implementation and analysis completed for CSC3042F Assignment 1.

The assignment focuses on the following questions:

- How do MLPs and CNNs differ in their ability to learn from image data?
- Which architecture performs better on grayscale versus colour image datasets?
- How does model complexity affect both accuracy and training efficiency?
- How do parameter constraints influence the effectiveness of each architecture?

---

## Repository Contents

The repository contains the following key files and folders:

- A1.ipynb — the main Jupyter Notebook containing the implementation, experiments, plots, and analysis.
- A1.html — an HTML export of the notebook.
- A1.pdf — a PDF version of the assignment work.
- CSC3042F_Assignment1_MLPvsCNNs.pdf — the submitted or reference assignment document.
- data/ — dataset-related files and supporting materials.
- logs/ — training logs and experiment outputs.

---

## Experimental Scope

### Part A: Complexity Ladder

In this section, the following experiments were conducted:

- MLP trained on MNIST
- CNN trained on MNIST
- MLP trained on CIFAR-10
- CNN trained on CIFAR-10

The models were evaluated using:

- training loss
- validation loss
- training accuracy
- validation accuracy
- test accuracy
- training time

This part of the project highlights how CNNs are generally more effective for image data because they exploit spatial structure, while MLPs flatten input images and do not naturally model local pixel relationships.

### Part B: Parameter Budget Challenge

In this section, both architectures were designed to use a similar parameter count within a target budget range.

The models were then trained on CIFAR-10 for a longer number of epochs, and the following were reported:

- test accuracy
- total training time
- seconds per epoch
- parameter counts
- hyperparameter tuning results

This part explores whether CNNs remain more efficient under strict parameter constraints.

---

## Technologies Used

The implementation is built using the following Python libraries:

- PyTorch
- TorchVision
- NumPy
- Pandas
- Matplotlib

These tools were used for model construction, training, evaluation, visualization, and reporting.

---

## Requirements

To run the notebook locally, the following dependencies are recommended:

- Python 3.9 or newer
- PyTorch
- TorchVision
- NumPy
- Pandas
- Matplotlib

A GPU is optional but can significantly accelerate training.

---

## Setup and Execution

1. Clone or download this repository.
2. Open the project directory in a Python environment with the required dependencies installed.
3. Launch the notebook using Jupyter Notebook or JupyterLab.
4. Run the cells in sequence in A1.ipynb.

If the datasets are not already available, the notebook will attempt to download them through the relevant PyTorch data loaders.

---

## Expected Outputs

Running the notebook produces:

- trained MLP and CNN models
- evaluation metrics for each experiment
- training and validation curves
- result tables summarizing test performance
- a written analysis of model behaviour and efficiency

---

## Key Findings

The project demonstrates that:

- CNNs generally outperform MLPs on image classification tasks, especially for more complex datasets such as CIFAR-10.
- MLPs can perform reasonably well on simpler datasets such as MNIST, but they are less suited to capturing spatial patterns in images.
- CNNs make more efficient use of parameters for visual tasks because they exploit local connectivity and shared convolutional filters.

---

## Notes

This repository is intended for academic purposes as part of an assignment submission. It provides a practical comparison of traditional fully connected networks and convolutional networks for image recognition.

---

## Author

Student: Tracey Letlape

Student Number: LTLTRA001

Course: CSC3042F
