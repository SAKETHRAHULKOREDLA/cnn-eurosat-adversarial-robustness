# cnn-eurosat-adversarial-robustness
CNN-based land use classification on EuroSAT with adversarial robustness using DeepFool attack (PyTorch)
# CNN-based Land Use Classification with Adversarial Robustness (EuroSAT)

This project implements a Convolutional Neural Network (CNN) for land use classification using the EuroSAT dataset, along with adversarial robustness analysis using the DeepFool attack.

---

## 🚀 Features
- Custom CNN architecture with:
  - Residual connections
  - Global Average Pooling (GAP)
  - 1x1 convolutions
- Data augmentation:
  - Random flips
  - Rotations
  - Random crop + resize
- Model evaluation:
  - Precision & Recall
  - Confusion Matrix
- Adversarial attack:
  - Custom implementation of DeepFool
  - Comparison with `torchattack` library

---

## 📂 Dataset
- EuroSAT Dataset (from Torchvision)
- 10 land use classes

---

## 🧠 Model Architecture
- Fully Convolutional Neural Network
- Residual connections for better gradient flow
- GAP layer to reduce parameters
- Final 1x1 convolution for classification

---

## ⚙️ Training Details
- Optimizer: Adam
- Loss Function: Cross-Entropy Loss
- Train/Val/Test Split: 70/15/15

---

## 📊 Results
- Achieved strong classification performance on EuroSAT dataset
- Evaluated using:
  - Precision
  - Recall
  - Confusion Matrix

---

## ⚔️ Adversarial Robustness
- Implemented DeepFool attack to generate adversarial samples
- Measured attack success rate
- Compared custom implementation with `torchattack`

---

## 🛠️ Tech Stack
- Python
- PyTorch
- Torchvision
- NumPy
- Matplotlib

---

## 📸 Visualizations
- Training vs Validation loss curves
- Confusion matrix
- Adversarial examples before/after attack

---

## ▶️ How to Run

```bash
git clone https://github.com/yourusername/cnn-eurosat-adversarial-robustness
cd cnn-eurosat-adversarial-robustness
pip install -r requirements.txt
python train.py
