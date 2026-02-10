# DeepFake Face Detection using CNN (From Scratch)

## 📌 Project Overview
This project builds a Convolutional Neural Network (CNN) from scratch to detect whether a face image is **Real** or **AI-generated (DeepFake)**.

## 🧠 Dataset
Dataset used: **140k Real and Fake Faces** from Kaggle  
- Training images: 100,000  
- Validation images: 20,000  
- Classes: `real`, `fake`

## 🏗 Model Architecture
Custom CNN architecture with:
- 3 Convolution layers
- ReLU activations
- MaxPooling layers
- Fully connected layers

## ⚙️ Training Setup

| Parameter | Value |
|----------|-------|
| Image size | 224×224 |
| Batch size | 32 |
| Epochs | 5 |
| Optimizer | Adam |
| Loss function | CrossEntropyLoss |

## 📊 Results

| Epoch | Training Loss | Validation Accuracy |
|-------|---------------|---------------------|
| 1 | 0.4772 | 86.65% |
| 2 | 0.2338 | 91.59% |
| 3 | 0.1349 | 94.53% |
| 4 | 0.0895 | **95.33%** |
| 5 | 0.0664 | 95.22% |

Best model was saved at **Epoch 4** with **95.33% validation accuracy**.

## 🧾 Trained Model Weights

The trained model is too large to be stored directly on GitHub. You can download it from Kaggle here:

👉 https://www.kaggle.com/datasets/mondaldebasish05/deepfake-detector-model-weights-cnn-from-scratch

---

## 🧠 How to Use the Model

You can load the saved model weights into your PyTorch model using:

```python
model.load_state_dict(torch.load("best_deepfake_model.pth"))
model.eval()
