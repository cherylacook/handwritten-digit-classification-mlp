# Handwritten Digit Classification with MLP

**Note**: This project was completed as part of the AIML232 course at Te Herenga Waka — Victoria University of Wellington.

## Objective
Implement a multi-layer perceptron (MLP) to classify handwritten digits from the scikit-learn Digits dataset. Evaluate how different activation functions affect early learning speed, convergence, and final test accuracy.

## Dataset
This project uses the built-in scikit-learn Digits dataset: 1,797 grayscale images of handwritten digits (8x8 pixels) relatively evenly distributed across the classes 0-9.

## Structure
- `digit_classification_mlp.ipynb` - Full implementation with activation function experiments and results.
- `requirements.txt` - Python dependencies.

## Key Results
- Test set accuracy:
  - Tanh: 96%
  - ReLU: 95%
  - Sigmoid: 63%
- Observations:
  - Sigmoid converged very slowly (<15% accuracy in the first 5 epochs) due to vanishing gradients, resulting in poor test accuracy.
  - Tanh and ReLU converge quickly and reliably, with Tanh slightly outperforming ReLU.
  - Activation choice strongly impacts both early learning and final performance.
  
## How to Run
Python version: 3.10+ 
```
pip install -r requirements.txt
jupyter notebook
# then run digit_classification_mlp.ipynb in the browser, and run all cells in order
```

## Summary
A simple three-layer MLP can effectively classify handwritten digits, with activation choice having a strong impact: Tanh and ReLU converge quickly and achieve high test accuracy, while Sigmoid converges slowly and performs poorly due to vanishing gradients.

## Reproducibility / Notes
- Random seeds are fixed where applicable to ensure consistent results.
- All code is fully contained in the provided notebook and can be run end-to-end.
