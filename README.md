# Cancer Classification Neural Network

This repository contains a PyTorch implementation of a neural network for binary cancer classification. The model is built using the `nn.Module` class from PyTorch and includes two fully connected layers with ReLU activation and a sigmoid activation for binary classification.

## Model Architecture

The neural network architecture is defined in the `CancerClassifier` class within the `cancer_classifier.py` file. It consists of:
- Input layer: `nn.Linear(input_size, hidden_size)`
- ReLU activation: `nn.ReLU()`
- Hidden layer: `nn.Linear(hidden_size, output_size)`
- Sigmoid activation: `nn.Sigmoid()`

## Usage

1. **Dataset:**
   - Replace the placeholder value for `input_size` with the actual number of input features.
   - Ensure your dataset is properly preprocessed and split into training and testing sets.

2. **Model Instantiation:**
   - Adjust the `hidden_size` and `output_size` based on your specific problem.

3. **Loss Function and Optimizer:**
   - The model uses Binary Cross Entropy Loss (`nn.BCELoss()`) and the Adam optimizer (`optim.Adam`).

4. **Training:**
   - Implement your training script, making use of the defined model, loss function, and optimizer.
