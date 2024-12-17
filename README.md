# Brain Tumor Detection

# Brain Tumor Detection using Vision Transformer  

## Authors  
- **Dr. Hong Cheng** (hcheng@saumag.edu)  
- **Rupesh Konduru** (RKonduru4501@muleriders.saumag.edu)  

## Overview  
This project utilizes **Vision Transformer (ViT)** to predict brain tumor labels and generate bounding boxes around detected tumors. The model is trained on a brain tumor dataset to classify tumors into four categories:  
1. Glioma  
2. Meningioma  
3. Pituitary  
4. No Tumor  

The project compares different bounding box regression techniques such as **CIOU**, **GIOU**, **DIOU**, and **Mean Square Error (MSE)**, highlighting the effectiveness of CIOU.  

## Key Features  
- **High Accuracy:** Achieved 90.5% label prediction accuracy and 71.5% bounding box IoU using CIOU.  
- **Visualization:** Outputs include bounding boxes with IoU values and predicted labels overlaid on images.  
- **Transformer-based Approach:** Demonstrates the effectiveness of Vision Transformers in medical imaging tasks.  
- **Comparison of Loss Functions:** CIOU outperforms other loss functions in bounding box regression for this dataset.  

## Results  
- **Label Accuracy:**  
  - CIOU: 90.5%  
  - GIOU: 87.0%  
  - DIOU: 88.2%  
  - MSE: 85.4%  

- **Bounding Box IoU:**  
  - CIOU: 71.5%  
  - GIOU: 65.8%  
  - DIOU: 68.2%  
  - MSE: 62.3%  

## Dataset  
The brain tumor dataset contains labeled images categorized into four classes. Each image includes:  
- Ground truth bounding boxes  
- Tumor labels  

## Model Architecture  
The model leverages a **Vision Transformer (ViT)** for feature extraction and prediction. The architecture consists of:  
- Patch embedding layers to process image inputs.  
- Transformer encoders for feature extraction.  
- Fully connected layers for tumor classification and bounding box regression.  


