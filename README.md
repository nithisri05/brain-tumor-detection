# Brain Tumor Detection from MRI Images using Vision Transformer (ViT)

This project implements a **4-class brain tumor classification system** using MRI images and a **Vision Transformer (ViT)** model. It also incorporates **model explainability** through heatmap generation using the **BraTS-2020 dataset**, enabling visualization of regions that influence model predictions.

---

## Problem Statement

Manual analysis of MRI scans for brain tumor detection is time-consuming and subject to human variability. This project aims to assist medical diagnosis by applying **transformer-based deep learning** to automatically classify MRI images and provide **visual explanations** of predictions.

---

## Classes

The model classifies MRI images into the following four categories:

1. No Tumor  
2. Glioma Tumor  
3. Meningioma Tumor  
4. Pituitary Tumor  

---

## 📥 Datasets

### Brain Tumor MRI Dataset (4 Classes)
- Source: Kaggle  
- Link: https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset  
- Usage: Training and evaluation of the ViT classification model  

### BraTS-2020 Dataset
- Source: Brain Tumor Segmentation Challenge  
- Usage: Heatmap and explainability generation (Grad-CAM / attention visualization)  

---

## Architecture Flow

```text
MRI Images
     ↓
Image Preprocessing & Augmentation
     ↓
Patch Embedding
     ↓
Vision Transformer (ViT)
     ↓
4-Class Classification
     ↓
Performance Evaluation
     ↓
Heatmap Generation (BraTS-2020)
