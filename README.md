# Training ResNet on the MNIST Dataset

- 22022511 - Nguyen Viet Bac
---

This notebook implements a ResNet model to train on the MNIST dataset using PyTorch. It covers model setup, data preprocessing, and training steps for a neural network on image data.

## Contents

- **ResNet**: The ResNet architecture with configurable versions such as ResNet18, ResNet34, ResNet50, ResNet101, and ResNet152.
- **Data Preparation**: Preprocessing MNIST data from single-channel grayscale images to 3 channels and resizing from \(28 \times 28\) to \(224 \times 224\) to fit ResNet input requirements.
- **Training and Evaluation**: Using PyTorch to train the model and evaluate its accuracy on the test set.

## Requirements

- **Python 3.6+**
- **PyTorch**
- **torchvision**

Install the required libraries with:

```bash
pip install torch torchvision
```

## Usage

1. **Model Initialization**: Choose the desired ResNet model (e.g., `resnet18`, `resnet34`, `resnet50`, etc.) from the code provided.
2. **Data Preprocessing**: MNIST data is transformed to 3-channel images and resized to \(224, 224\).
3. **Training**: Run training steps over multiple epochs, tracking the loss and accuracy.
4. **Evaluation**: Evaluate the model’s accuracy on the MNIST test dataset.

## Results

After training, the model will display its accuracy on the MNIST test set.

## Example Output

After 5 epochs of ResNet18:

```
Epoch [1/5], Train Loss: 0.1126, Test Loss: 0.0599, Test Accuracy: 97.99%
Epoch [2/5], Train Loss: 0.0411, Test Loss: 0.0556, Test Accuracy: 98.26%
Epoch [3/5], Train Loss: 0.0325, Test Loss: 0.0457, Test Accuracy: 98.62%
Epoch [4/5], Train Loss: 0.0285, Test Loss: 0.0242, Test Accuracy: 99.22%
Epoch [5/5], Train Loss: 0.0239, Test Loss: 0.0230, Test Accuracy: 99.27%
```

