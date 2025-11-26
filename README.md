# CIFAR-10 Image Classification Project

This project contains three implementations of Convolutional Neural Networks (CNNs) for classifying images from the CIFAR-10 dataset using different frameworks and approaches.

## 📁 Project Structure

- **Part1_CIFAR.ipynb**: PyTorch implementation with data augmentation, validation set, and comprehensive evaluation
- **Part2.ipynb**: PyTorch implementation with hyperparameter tuning experiments
- **Part3_Keras.ipynb**: TensorFlow/Keras implementation comparing simple and advanced CNN architectures

## 🎯 Dataset

**CIFAR-10** is a dataset of 60,000 32x32 color images in 10 classes:
- Airplane, Automobile, Bird, Cat, Deer, Dog, Frog, Horse, Ship, Truck
- Training set: 50,000 images
- Test set: 10,000 images

## 📊 Results Summary

### Part 1 (PyTorch - Basic CNN)
- **Test Accuracy**: ~60%
- Architecture: 3 convolutional layers + 3 fully connected layers
- Features: Data augmentation, validation set, model checkpointing

### Part 2 (PyTorch - Simplified CNN)
- **Test Accuracy**: ~64-65%
- Architecture: 2 convolutional layers + 3 fully connected layers
- Features: Hyperparameter tuning (learning rate and epoch combinations)

### Part 3 (Keras/TensorFlow)
- **Model 1 (Basic)**: ~64% test accuracy
- **Model 5 (Advanced)**: ~86.6% test accuracy
  - Features: Batch Normalization, Dropout, deeper architecture

## 🛠️ Technologies Used

- **PyTorch**: Deep learning framework for Parts 1 & 2
- **TensorFlow/Keras**: Deep learning framework for Part 3
- **NumPy**: Numerical computations
- **Matplotlib**: Data visualization

## 📝 Requirements

```
torch
torchvision
tensorflow
keras
numpy
matplotlib
pandas
```

## 🚀 Usage

1. Open any of the Jupyter notebooks
2. Run the cells sequentially
3. The notebooks will automatically download the CIFAR-10 dataset on first run
4. Models will be trained and evaluated automatically

## 📌 Notes

- All notebooks include data preprocessing, model training, and evaluation
- Part 1 includes validation set splitting and model checkpointing
- Part 2 includes hyperparameter search experiments
- Part 3 compares different CNN architectures with regularization techniques

## 📄 License

This project is for educational purposes (INT305 Assignment 2).

