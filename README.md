# Handwritten Digits Classification with MLP

## Objective
Implement a multi-layer perceptron (MLP) to classify handwritten digits from the scikit-learn Digits dataset and evaluate how different activation functions affect convergence and test performance. 

## Structure
- `notebooks/digit_classification_mlp.ipynb` - Full implementation with experiments and results.
- `requirements.txt` - Python dependencies.

## Key Results
- Best activation function: Tanh
- Test set accuracy:
  - Tanh: 96%
  - ReLU: 95%
  - Sigmoid: 63%
- Sigmoid performs substantially worse because its activations saturate, causing vanishing gradients that hinder optimisation. By contrast, Tanh (zero-centred with stronger gradients) and ReLU (non-saturating for positive inputs) support more stable and efficient training.
  
## How to Run
Python version: 3.10+ 
```bash
pip install -r requirements.txt
jupyter notebook notebooks/digit_classification_mlp.ipynb
```

## Summary
A simple three-layer MLP achieves strong performance on the Digits dataset, and activation choice noticeably affects optimisation: Tanh and ReLU converge reliably, while Sigmoid suffers from gradient saturation and converges poorly.

## Reproducibility / Notes
- Random seeds are fixed where applicable to ensure consistent results.
- All code is fully contained in the provided notebook and can be run end-to-end.
