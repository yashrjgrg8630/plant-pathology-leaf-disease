# 🍏 Plant Pathology 2020 - Apple Leaf Disease Classification

[![Python](https://img.shields.io/badge/python-3.11-blue?logo=python&logoColor=white)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/tensorflow-2.13-orange?logo=tensorflow&logoColor=white)](https://www.tensorflow.org/)
[![Kaggle](https://img.shields.io/badge/Kaggle-Dataset-blue?logo=kaggle&logoColor=white)](https://www.kaggle.com/c/plant-pathology-2020-fgvc7)

---

## 🔗 Project Overview
This project classifies apple leaves into four categories: **Healthy, Rust, Scab, and Multiple Diseases**, using a **Convolutional Neural Network (CNN)**.  

The goal is to help farmers and agronomists detect diseases early, reducing crop loss.

**Dataset:** [Plant Pathology 2020 - Kaggle](https://www.kaggle.com/c/plant-pathology-2020-fgvc7)  
**Number of Images:** 3,651 training images  

---

## 🚀 Project Workflow
1. **Data Preprocessing**  
   - Images resized to 128×128 pixels  
   - Normalization and data augmentation using `ImageDataGenerator`  
2. **CNN Model Architecture**  
   - 3 Convolutional layers (Conv2D + MaxPooling + BatchNormalization)  
   - Fully connected layer + Dropout  
   - Output layer with 4 neurons (softmax activation)  
3. **Training**  
   - Loss function: categorical cross-entropy  
   - Optimizer: Adam  
   - Trained for 15 epochs  
4. **Predictions**  
   - Generated `submission.csv` for Kaggle leaderboard  

---

## 📂 Repository Structure
plant-pathology-leaf-disease/
├── plant-pathology-cnn.ipynb # Jupyter Notebook with full code
├── submission.csv # Sample predictions
├── README.md # Project documentation
└── requirements.txt # Python dependencies (optional)

yaml
Copy code

---

## 📊 Results
- Training Accuracy: **~78%**  
- Validation Accuracy: **~77%** (best at Epoch 14)  
- Submission format compatible with Kaggle leaderboard

---

## ⚡ Future Improvements
- Apply **Transfer Learning** (EfficientNet, ResNet50) for higher accuracy  
- Use **Grad-CAM** to visualize CNN focus areas on leaves  
- Fine-tune **data augmentation** and hyperparameters to reduce overfitting  
- Explore **Ensemble methods** to improve classification performance  

---

## 🛠️ Technologies Used
- **Python 3.11**  
- **TensorFlow 2.x / Keras**  
- **NumPy, Pandas, Matplotlib, Seaborn**  
- **Jupyter Notebook**  

---

## 📌 How to Run
1. Clone the repository:  
   ```bash
   git clone https://github.com/YOUR_USERNAME/plant-pathology-leaf-disease.git
Install dependencies:

bash
Copy code
pip install -r requirements.txt
Open plant-pathology-cnn.ipynb in Jupyter Notebook or Kaggle Notebook

Run all cells to train model or generate predictions

📚 References
Kaggle Plant Pathology 2020 Challenge: Link

TensorFlow Keras Documentation: Link

Convolutional Neural Networks: Stanford CS231n Notes
