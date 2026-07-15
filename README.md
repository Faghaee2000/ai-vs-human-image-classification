# AI vs. Human Image Classification

## Project Description

This project investigates whether convolutional neural networks (CNNs) can distinguish between real photographs and AI-generated images.

Three different models were implemented and compared:

- Custom CNN
- ResNet50 (Transfer Learning)
- EfficientNet-B0 (Transfer Learning)

The models were evaluated using Accuracy, Precision, Recall, F1-score, Confusion Matrix, and GradCAM visualization.



## Dataset

Dataset: AI vs. Human-Generated Images

Source:
https://www.kaggle.com/datasets/alessandrasala79/ai-vs-human-generated-dataset



## Project Structure


Assignment2/
│
├── AI_vs_Human_Image_Classification.ipynb
├── GradCAM.ipynb
├── resnet50_model.pth
├── requirements.txt
├── README.md
└── data/




## Requirements

Install the required packages using:

```bash
pip install -r requirements.txt
```



## Models

- Custom CNN
- ResNet50
- EfficientNet-B0



## Results

The pretrained models achieved better performance than the custom CNN.

ResNet50 obtained the best overall results, followed by EfficientNet-B0.

GradCAM was used to visualize the regions that influenced the predictions of the best-performing model.



## Author

Fatemeh Aghaei
