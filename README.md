# 🍏 Plant Pathology 2020 - Apple Leaf Disease Classification

This project classifies apple leaves into **Healthy, Rust, Scab, and Multiple Diseases** using a Convolutional Neural Network (CNN).  
Dataset: [Plant Pathology 2020 - Kaggle](https://www.kaggle.com/c/plant-pathology-2020-fgvc7)

---

## 🚀 Project Workflow
1. Data preprocessing with `ImageDataGenerator`.
2. CNN model with Conv2D, MaxPooling, Dropout.
3. Training with categorical cross-entropy.
4. Generating predictions (`submission.csv`) for Kaggle.

---

## 📂 Files in this Repo
- `plant-pathology-cnn.ipynb` → Jupyter Notebook (full code).
- `submission.csv` → Sample predictions file.
- `README.md` → Project documentation.

---

## 📊 Results
- Achieved **~78% training accuracy** and **~77% validation accuracy** (best at Epoch 14).  
- Submission file format compatible with Kaggle leaderboard.  

---

## ⚡ Future Improvements
- Use **Transfer Learning** (EfficientNet, ResNet) for higher accuracy.
- Apply **Grad-CAM** for visual explanations.
- Perform **data augmentation** and **fine-tuning** to reduce overfitting.
