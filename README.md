# Handwritten Digits Classification with MLP

## Objective
Implement a multi-layer perceptron (MLP) to classify handwritten digits from the scikit-learn Digits dataset and evaluate how different activation functions affect convergence and test performance. 

## Structure
- 'notebooks/digit_classification_mlp.ipynb' - Full implementation with experiments and results.
- 'requirements.txt' - Python dependencies

## Key Results
- Best activation function: Tanh
- Test set accuracy:
  - Tanh: 96%
  - ReLU: 95%
  - Sigmoid: 63% (underperforms due to vanishing gradients)

## How to Run
pip install -r requirements.txt
jupyter notebook notebooks/digit_classification_mlp.ipynb

## Summary
A simple MLP achieves strong performance on the Digits dataset, and activation choice noticeably affects optimisation and final test accuracy. Tanh and ReLU significantly outperform Sigmoid on this task.
