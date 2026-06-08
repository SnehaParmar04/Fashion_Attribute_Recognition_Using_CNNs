#  Fashion Attribute Recognition Using CNN and Transfer Learning

##  Project Overview

This project focuses on classifying fashion product images into different categories using deep learning techniques. The goal is to automatically identify the type of fashion item based on image data.

Two models were implemented and compared:

- Custom Convolutional Neural Network (CNN)
- MobileNetV2 Transfer Learning Model

The performance of both models was evaluated to analyze the effectiveness of transfer learning in image classification tasks.

---

##  Dataset Information

**Dataset:** Fashion Product Images Dataset  
**Dataset Link:** https://www.kaggle.com/datasets/paramaggarwal/fashion-product-images-dataset  

###  Dataset Statistics

- Total Dataset Size: 44,424 images  
- Final Balanced Dataset: ~4,103 images  

---

##  Selected Classes (7 Classes)

- Shirts  
- Tshirts  
- Jeans  
- Track Pants  
- Casual Shoes  
- Watches  
- Tops  

### Class Distribution (Balanced Dataset)

- Shirts: 700  
- Tshirts: 700  
- Jeans: 603  
- Track Pants: 700  
- Casual Shoes: 700  
- Watches: 700  
- Tops: 700  

---

##  Image Information

- Image Format: JPG  
- Input Image Size: 128 × 128 pixels  
- Number of Classes: 7  
- Task Type: Multi-Class Image Classification  

---

##  Methodology

The project follows a structured deep learning pipeline:

- Dataset Loading (CSV + Images)
- Data Filtering (7 classes selection)
- Image Preprocessing
- Image Resizing and Normalization
- Data Augmentation
- Train / Validation / Test Split
- Custom CNN Model Development
- CNN Training and Evaluation
- Transfer Learning using MobileNetV2
- Model Comparison

---

##  Models Used

###  Custom CNN

Architecture:

- Conv2D (32 filters)
- MaxPooling2D
- Conv2D (64 filters)
- MaxPooling2D
- Conv2D (128 filters)
- MaxPooling2D
- Flatten Layer
- Dense Layer (256 neurons)
- Dropout (0.5)
- Softmax Output Layer (7 classes)

---

###  MobileNetV2 (Transfer Learning)

Architecture:

- MobileNetV2 (ImageNet Pretrained)
- Frozen Base Layers
- Global Average Pooling Layer
- Dense Layer (128 neurons)
- Dropout (0.4)
- Softmax Output Layer (7 classes)

---

##  Evaluation Metrics

The models were evaluated using:

- Accuracy
- Loss
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Classification Report

---

##  Results

| Model | Test Accuracy | Test Loss |
|------|--------------|----------|
| Custom CNN | 77.27% | 0.677 |
| MobileNetV2 | **93.66%** | **0.190** |

 MobileNetV2 significantly outperformed the CNN model by achieving better accuracy and lower loss.

---

##  Repository Structure
fashion-attribute-recognition/
│
├── Fashion_Attribute_Recognition.ipynb
├── README.md
├── dataset_link.txt
└── figures/


---

##  How to Run the Project

```bash
# Open notebook in Kaggle or Colab

# Ensure dataset path is correct

# Run all cells sequentially

---
## ** AUTHOR**

**Sneha Maheshbhai Parmar**  
**MSc. Data Science**  
**University of Europe**
