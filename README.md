# CNN on Tom and Jerry Dataset

**Course:** CVPR | **Student ID:** 23-51626-2 | **Assignment:** CNN Development on Custom Dataset

## Overview
A custom CNN trained from scratch in PyTorch to classify Tom & Jerry cartoon frames into 4 classes: jerry, tom, tom_jerry_0 (neither), tom_jerry_1 (both).

## Dataset
Tom and Jerry Image Classification (Kaggle: balabaskar/tom-and-jerry-image-classification), 5,478 frames. Split 70/15/15 into train/validation/test.

## Model and Training
- Architecture: 2 Conv blocks (64, 128 filters) + 2 fully connected layers (6.5M parameters)
- Input size: 64x64, batch size 32
- Optimizer: Adam (lr = 1e-3), Loss: CrossEntropyLoss
- Epochs: 10, Augmentation: flip, rotation, color jitter

## Results
- Test accuracy: 76.67%
- Macro F1: 0.7454

## Files
- `CNN_23-51626-2.ipynb`: full implementation with outputs and plots
- Model weights (`CNN_23_51626_2.pth`, 26 MB) are kept locally because of the 20 MB limit.
