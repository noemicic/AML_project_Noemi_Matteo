# ResNet18 with Three Classification Models

This repository contains the **`code_FINAL.ipynb`** notebook, which implements three different versions of the ResNet18 model, each with a distinct classification approach:

1. **Standard Softmax Classification**: Uses a classical softmax activation function for multi-class classification.
2. **Soft-margin SVM Classification**: Employs a support vector machine with a soft-margin loss function for classification.
3. **RBF SVM via Random Fourier Features (RFF)**: Approximates the behavior of an RBF kernel SVM using Random Fourier Features.

## Hyperparameter Exploration

Various hyperparameters were experimented with for each architecture, including:

- **Dropout**: Used across all models to regularize the ResNet18 backbone and classification layers.
- **SVM Penalization Term (C)**: Applied to the soft-margin SVM and RBF SVM models.
- **Kernel Width ($\gamma$)**: Specific to the RBF SVM model, determining the smoothness of the kernel.
- **Dimensionality of RFF (D)**: Determines the number of random Fourier features used in the RBF SVM approximation.

## Results

The outcomes of the experiments, including performance metrics for each architecture and hyperparameter configuration, are stored in the **`Results`** folder. You can review these results to compare the effectiveness of the three classification approaches under varying conditions.

## Required Libraries
1. Torch:
torch: The core library for deep learning with PyTorch.
torch.nn, torch.nn.functional, torch.optim: Modules within PyTorch for building and training models.
2. Torchvision:
A library for common datasets (like CIFAR10), pretrained models, and image transformations.
3. Matplotlib:
Used for visualizing graphs and images.
4. NumPy:
A library for mathematical operations on arrays and matrices.
5. Random:
A standard Python module for generating random numbers (pre-installed with Python).

Run the following command in your terminal or Python environment:
```python
pip install torch torchvision matplotlib numpy
```
ATTENTION: Ensure the versions of torch and torchvision are compatible with each other. You can check the compatible versions in the [PyTorch documentation](https://pytorch.org/get-started/locally/).
