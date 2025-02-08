# ISIC 2024 - Skin Cancer Detection with 3D-TBP

## Overview
The **ISIC 2024 Skin Cancer Detection Challenge** focuses on developing AI-driven solutions to detect malignant skin lesions from images resembling cellphone photos. While dermoscopy-based AI algorithms have shown promising results in clinical settings, the challenge is to create models that work effectively in primary care or non-clinical environments, where image quality is lower. 

This competition introduces a novel dataset containing lesion images from thousands of patients across three continents, enabling the development of AI algorithms to differentiate histologically confirmed malignant skin lesions from benign ones. Our work aims to improve early diagnosis and disease prognosis by making automated skin cancer detection accessible to broader populations and settings.

## Approach
Our approach leveraged both image and tabular data to develop robust classification models. Key techniques included:
- **Deep Learning Models:** Benchmarked CNN architectures such as **EfficientNet** and **ResNet** on lesion images.
- **Gradient Boosted Trees:** Trained models like **XGBoost, LightGBM, and CatBoost** on patient metadata.
- **Data Balancing Techniques:** Addressed class imbalance using **focal loss, stratified sampling, and undersampling with Faiss**.
- **Feature Engineering:** Combined **CNN embeddings with tabular metadata** to enhance predictive performance.
- **Ensemble Learning:** Integrated predictions from multiple models to improve overall accuracy.

## Repository Structure
### Notebooks
- **Faiss Data Creation**
  - Created an **undersampled dataset** to handle class imbalance using **Faiss**, ensuring better model generalization.
  
- **Tabular Data**
  - Trained **Gradient Boosted Tree models**, including **XGBoost and LightGBM**, on patient metadata to leverage tabular features for classification.

- **Training Notebook**
  - Combined **image data with metadata** for a more comprehensive training approach. Used **CNN models for feature extraction** and integrated them with tabular classifiers.

- **EDA_ISIC**
  - Performed basic **Exploratory Data Analysis (EDA)** to understand the dataset structure, distribution of classes, and key statistical insights.

## Competition Results
- **Rank:** 🏆 **485th out of 2,739 teams (Top 18%)**
- **Submissions:** 📈 **80+ model submissions**
- **Impact:** 🚀 **Demonstrated the potential of combining deep learning and gradient boosted trees for robust skin cancer detection.**

## Acknowledgments
This project was developed as part of the **ISIC 2024 competition on Kaggle**, aiming to advance AI-driven early detection of skin cancer in non-clinical settings.
