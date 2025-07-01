# Fine-tuning-Pipeline-for-YOLOv11-for-Image-Classification


This repository provides a **complete pipeline in Jupyter Notebook** to fine-tune **YOLOv11** for image classification on the [Chicken Disease Dataset](https://www.kaggle.com/datasets/allandclive/chicken-disease-1?resource=download&select=train_data.csv) from Kaggle. The model achieved an impressive **98.7% accuracy**, demonstrating its effectiveness in poultry disease recognition using deep learning.

---

## 📌 Project Summary

- ✅ **Model**: YOLOv11 (Re-purposed for classification)
- 📊 **Accuracy**: 98.7%
- 📁 **Dataset**: [Chicken Disease 1 (Kaggle)](https://www.kaggle.com/datasets/allandclive/chicken-disease-1)
- 📒 **Notebook**: End-to-end pipeline including training, evaluation, and visualizations
- 🖼️ **Outputs**: Confusion Matrix, Accuracy & Loss Curves

---

## 📂 Dataset Description

The dataset contains labeled images of chickens categorized by disease type. It is ideal for training computer vision models in the agricultural and veterinary domain.

- **Classes (4 total)**:
  - 🟩 Healthy
  - 🐛 Coccidiosis
  - 🦠 Salmonella
  - 💉 New Castle Disease

- **Files Included**:
  - `train_data.csv`: Contains image file paths and labels
  - `images/`: Folder with chicken images

📌 **Dataset Link**:  
[https://www.kaggle.com/datasets/allandclive/chicken-disease-1](https://www.kaggle.com/datasets/allandclive/chicken-disease-1)

---

## 🧠 Model Overview

YOLOv11 is originally designed for object detection. In this project, it is adapted for image classification by:

- Replacing detection layers with a classification head
- Feeding preprocessed single-object images (one chicken per image)
- Training with cross-entropy loss for multi-class classification

---

## 📒 Notebook Pipeline

The Jupyter Notebook `yolov11_chicken_disease_finetuning.ipynb` includes:

1. ✅ Importing Libraries
2. 📂 Loading and Preprocessing Dataset
3. 🔧 Configuring YOLOv11 for Classification
4. 🏋️ Training Loop
5. 📊 Evaluation using Accuracy & Confusion Matrix
6. 📈 Plotting Loss and Accuracy Curves
7. 💾 Saving the Fine-tuned Model

---

## 📈 Results

- **Final Accuracy**: 98.7%
- **Evaluation Metrics**:
  - Confusion Matrix
  - Per-Class Accuracy
  - Training vs Validation Curves

📊 **Visuals** (replace these with your image paths):

![Confusion Matrix](![WhatsApp Image 2025-07-01 at 6 26 25 PM (1)](https://github.com/user-attachments/assets/91a38c88-f7d6-41c9-af17-53f614c59c62)
)
![WhatsApp Image 2025-07-01 at 6 26 26 PM](https://github.com/user-attachments/assets/e7418246-c14f-4910-a062-a9a6d5f8c081)

![Training Curves](![WhatsApp Image 2025-07-01 at 6 26 25 PM](https://github.com/user-attachments/assets/a7a2427c-316f-4dfc-9670-64e4238e3382)
)
![WhatsApp Image 2025-07-01 at 6 26 26 PM (1)](https://github.com/user-attachments/assets/66f7a505-13c5-47a9-89f5-b6d765030115)
![WhatsApp Image 2025-07-01 at 6 26 27 PM](https://github.com/user-attachments/assets/70c42f14-0765-42fe-b29d-06a6f83a92b2)


---

## 🧪 How to Run

### 🧰 Requirements

Install the dependencies:

```bash
pip install -r requirements.txt
