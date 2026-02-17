🧠 DeepFake Detector
Explainable Detection of AI-Generated Face Manipulations Using CNN and Grad-CAM

📅 Dated: 12-02-2026
🏫 Quaid-e-Awam University of Engineering, Science & Technology

👨‍💻 Authors

Zeeshan Ali

Muhammad Mudasir

Amanat Ali

Muhammad Hammad Khan

Ms. Aisha Chandio

📌 Introduction

Artificial Intelligence has advanced to a level where it can generate highly realistic human face images, known as DeepFakes, using deep learning techniques.

These fake images look so real that it becomes very difficult for the human eye to distinguish them from real images.

Deepfakes are increasingly misused in:

Fake news

Social media manipulation

Identity theft

Cybercrimes

Reputation damage

Manual detection is unreliable and time-consuming.
Therefore, there is a strong need for an automatic and intelligent deepfake detection system.

❗ Problem Statement

Artificial Intelligence can generate fake human face images that look almost real.

Although some AI tools can detect deepfakes, most systems only provide a “Real” or “Fake” result without explaining the reason.

This reduces:

User trust

Transparency

Interpretability

👉 Therefore, we need a system that:

Detects fake images accurately

Highlights manipulated regions

Provides understandable visual explanations

🎯 Aims & Objectives

The main aim of this project is:

To develop a CNN-based deepfake detection system that accurately identifies AI-generated facial images and highlights manipulated regions using visual explanations.

Objectives:

Develop a CNN-based model for deepfake detection.

Integrate Grad-CAM to visually explain model decisions.

Build an easy-to-use web application for users.

🏗️ Proposed Methodology
1️⃣ Data Collection & Preparation

Collected real and AI-generated images from public datasets.

Included different types of deepfake manipulations.

Preprocessing Steps:

Resize images to 224 × 224

Normalize pixel values

Label images as Real / Fake

Apply data augmentation to reduce overfitting

2️⃣ Model Architecture & Training

We used:

🔹 Transfer Learning with EfficientNetB2

Pre-trained EfficientNetB2 as feature extractor

CNN-based architecture

Training Parameters:

Optimizer: Adam

Learning Rate: 0.0005

Loss Function: Binary Cross-Entropy

Batch Size: 32

Early Stopping to prevent overfitting

This improved generalization and training stability.

3️⃣ Grad-CAM Integration (Explainable AI)

To improve transparency, we integrated Grad-CAM (Gradient-weighted Class Activation Mapping).

How it works:

Compute gradients of predicted class

Calculate neuron importance weights

Generate localization map

Overlay heatmap on original image

Heatmap Meaning:

🔴 Red/Yellow → High manipulation relevance

🔵 Blue → Low importance

This makes the system explainable and trustworthy.

4️⃣ Web Application Development
🔹 Backend:

Python Flask

Handles:

Image upload

Model inference

Grad-CAM generation

🔹 Frontend:

React.js

User-friendly interface

Simple image upload and result display

🌐 Web Application Workflow

1️⃣ User uploads an image
2️⃣ User clicks “Analyze Image”
3️⃣ Backend processes the image
4️⃣ Model predicts Real/Fake
5️⃣ Grad-CAM heatmap is generated
6️⃣ Final output shows:

Prediction

Visual heatmap

Transparent explanation

📊 Results
1️⃣ Model Performance Evaluation

(Add your performance metrics here)

Example format:

Accuracy: XX%

Precision: XX%

Recall: XX%

F1-Score: XX%

![Accuracy Graph](images/accuracy.png)
![Loss Graph](images/loss.png)
![Confusion Matrix](images/confusion_matrix.png)

2️⃣ Grad-CAM Explainability Results

The system successfully highlights:

Eyes

Mouth

Skin blending areas

Facial boundaries

![GradCAM Result](images/gradcam_output.png)

📌 Result Summary

✅ Accurate Deepfake Detection
Correctly identifies real and fake images with high reliability.

✅ Explainable Visual Results
Grad-CAM heatmaps clearly show manipulated areas.

✅ Easy-to-Use Web Application
Simple upload and instant result.

✅ Reduced Misinformation
Helps prevent the spread of fake content.

✅ Support for Trustworthy AI
Improves transparency in AI-based systems.

⚠️ Limitations

Image-based analysis only

Sensitive to dataset variations

🚀 Future Work

Video deepfake detection

Hybrid deep learning models

Cross-dataset evaluation

Real-time deployment

📚 References

Arshed et al., Multiclass AI-generated deepfake face detection, 2024

Irfan et al., Deepfake generation and detection survey, 2025

Kapoor et al., CNN-based deepfake detection, 2025

Kolagati et al., CNN-MLP model, 2022

Mansoor & Iliev, Explainable AI for deepfake detection, 2025

Devi & Simon, DeepGuardNet, 2025

Yardımcı et al., ResNeXt–LSTM video detection, 2025

🏁 Conclusion

This project presents an explainable deepfake detection system using CNN and Grad-CAM.

Unlike traditional black-box models, our system:

Detects fake images

Explains the reason

Highlights manipulated regions

Improves user trust

This work contributes toward building more transparent and trustworthy AI systems.
