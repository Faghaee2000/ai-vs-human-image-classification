# ai-vs-human-image-classification
Dataset

Dataset: AI vs. Human-Generated Images

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

Model Interpretation

To better understand model predictions, Grad-CAM is used to visualize the image regions that contribute most to each classification decision.

Repository Structure
.
├── data/
├── notebooks/
├── models/
├── src/
│   ├── dataset.py
│   ├── train.py
│   ├── evaluate.py
│   ├── models.py
│   └── utils.py
├── results/
│   ├── figures/
│   ├── confusion_matrix/
│   └── gradcam/
├── requirements.txt
└── README.md
Results

The project compares:

Transfer Learning vs Custom CNN
Training speed
Validation performance
Generalization capability
Error analysis
Grad-CAM visualizations

A detailed comparison of all models will be included after training.

Technologies
Python
PyTorch
Torchvision
NumPy
Pandas
Matplotlib
Scikit-learn
OpenCV
Future Work

Possible improvements include:

Vision Transformers (ViT)
ConvNeXt
EfficientNetV2
More advanced data augmentation
Ensemble learning
Cross-dataset evaluation
Authors
