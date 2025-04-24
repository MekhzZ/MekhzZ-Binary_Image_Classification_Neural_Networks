# Binary Image Classification Using Neural Networks

This repository contains a project focused on binary image classification using neural networks. The implementation leverages Jupyter Notebooks to provide a detailed walkthrough of the classification process, from data preprocessing to model evaluation. The project is designed to be modular and easy to adapt for different binary classification tasks.

---

## Overview

Binary image classification is a fundamental problem in computer vision. It involves categorizing images into one of two classes. This project showcases how Shallow Neural Network can be used for this purpose. The repository provides all necessary code and documentation, enabling users to replicate the results or adapt the solution for their datasets.

---

## Features

- Neural network-based binary image classification.
- Fully documented Jupyter Notebooks for ease of understanding.
- Modular codebase for flexibility and reusability.
- Visualization of training and evaluation metrics.
- Compatibility with custom datasets.

---

## Installation

To set up the project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/MekhzZ/MekhzZ-Binary_Image_Classification_Neural_Networks.git
   cd MekhzZ-Binary_Image_Classification_Neural_Networks

2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate

3. Install the required dependencies
   ```bash
   pip install -r requirements.txt

## Dataset

The dataset used for this project should be organized as follows:
  ```code
  dataset/
  ├── train/
  │   ├── blank/
  │   ├── hog/
  ├── test/
  ```
---

## Model Architecture

The model takes each values of rgb pixels 224,224 and further more executes these values on the basis of below layers.
  ```code
  Sequential(
    (0): Flatten(start_dim=1, end_dim=-1)
    (1): Linear(in_features=150528, out_features=512, bias=True)
    (2): ReLU()
    (3): Linear(in_features=512, out_features=128, bias=True)
    (4): ReLU()
    (5): Linear(in_features=128, out_features=2, bias=True)
  )
  ```

The specific architecture details are documented in the Jupyter Notebook, along with explanations of each layer.
