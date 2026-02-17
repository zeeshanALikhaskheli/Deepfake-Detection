# 🧠 DeepFake Detector  
### Explainable Detection of AI-Generated Face Manipulations Using CNN and Grad-CAM

---

## 📌 Overview

DeepFake technology uses Artificial Intelligence to generate highly realistic fake human face images. These images are often so convincing that it becomes difficult for humans to distinguish them from real images.

Deepfakes are increasingly misused for:

- Spreading misinformation  
- Identity theft  
- Social media manipulation  
- Cybercrimes  
- Reputation damage  

This project presents an **Explainable DeepFake Detection System** that not only classifies an image as **Real or Fake**, but also highlights manipulated regions using **Grad-CAM heatmaps**, improving transparency and user trust.

---

## 🎯 Problem Statement

Most deepfake detection systems only provide a binary output (Real/Fake) without explaining the reason behind the prediction.  

This lack of explainability reduces:

- User trust  
- Transparency  
- Reliability  

Therefore, we developed a system that:

- Accurately detects AI-generated facial images  
- Visually highlights manipulated regions  
- Provides explainable and trustworthy results  

---

## 🎯 Aims & Objectives

- Develop a CNN-based deepfake detection model  
- Integrate Grad-CAM for visual explanation  
- Build a user-friendly web application  
- Improve transparency in AI-based detection systems  

---

## 🏗️ Proposed Methodology

### 1️⃣ Data Collection & Preparation

- Collected real and AI-generated facial images from public datasets  
- Included various types of face manipulations  

**Preprocessing Steps:**
- Resize images to 224 × 224  
- Normalize pixel values  
- Label images as Real or Fake  
- Apply data augmentation to reduce overfitting  

---

### 2️⃣ Model Architecture & Training

We used **Transfer Learning** with EfficientNetB2 as a feature extractor.

**Training Configuration:**

- Optimizer: Adam  
- Learning Rate: 0.0005  
- Loss Function: Binary Cross-Entropy  
- Batch Size: 32  
- Early Stopping applied  

This approach improved training stability and generalization performance.

---

### 3️⃣ Grad-CAM Integration (Explainable AI)

Grad-CAM (Gradient-weighted Class Activation Mapping) was integrated to generate visual explanations.

**Process:**
- Compute gradients of predicted class  
- Calculate importance weights  
- Generate localization heatmap  
- Overlay heatmap on original image  

**Heatmap Interpretation:**
- 🔴 Red/Yellow → High manipulation focus  
- 🔵 Blue → Low importance  

---

### 4️⃣ Web Application

A user-friendly web application was developed.

**Backend:**
- Python Flask  
- Handles image upload, model inference, Grad-CAM generation  

**Frontend:**
- React.js  
- Clean and intuitive user interface  

---

## 🌐 Web Application Workflow

1. User uploads facial image  
2. Clicks “Analyze Image”  
3. Backend processes image  
4. Model predicts Real/Fake  
5. Grad-CAM heatmap generated  
6. Final output displays:
   - Prediction result  
   - Visual explanation  
   - Heatmap overlay  

---

## 📊 Results

### 🔹 Model Performance

(Add your actual values here)

- Accuracy: XX%  
- Precision: XX%  
- Recall: XX%  
- F1-Score: XX%  

---

### 🔹 Performance Graphs

```markdown
![Training Accuracy](images/accuracy.png)
![Loss Graph](images/loss.png)
![Confusion Matrix](images/confusion_matrix.png)
