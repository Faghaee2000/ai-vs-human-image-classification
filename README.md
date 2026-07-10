# ai-vs-human-image-classification
Dataset: AI vs. Human-Generated Images
https://www.kaggle.com/datasets/alessandrasala79/ai-vs-human-generated-dataset?utm_source=chatgpt.com

Source: Kaggle
Task: Binary Image Classification
Classes:
AI-Generated Images
Real (Human) Photographs
Models

The following models are implemented and compared:

Transfer Learning Models
ResNet50
EfficientNet-B0

Both models use pretrained ImageNet weights with a customized classification head.

Custom CNN

A convolutional neural network designed and trained from scratch for binary image classification.

Data Preprocessing

The preprocessing pipeline includes:
Image resizing
Normalization
Train / Validation / Test split
Data Augmentation

To improve model generalization and reduce overfitting, the following augmentation techniques are applied during training:
Random Horizontal Flip
Random Rotation
Random Resized Crop
Color Jitter (optional)
Training Configuration

Typical training settings include:
Optimizer: Adam
Loss Function: CrossEntropyLoss
Learning Rate: 1e-4
Batch Size: 32
Image Size: 224 × 224
Number of Epochs: 20 (configurable)
Evaluation

Models are evaluated using:
Accuracy
Precision
Recall
F1-score
Confusion Matrix

Additionally, training and validation curves are used to compare learning behavior.


The project compares:
Transfer Learning vs Custom CNN
Training speed
Validation performance
Generalization capability
Error analysis
Grad-CAM visualizations
