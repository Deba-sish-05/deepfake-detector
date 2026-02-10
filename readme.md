# DeepFake Face Detection using CNN (From Scratch)

## 📌 Project Overview
This project builds a Convolutional Neural Network (CNN) from scratch to detect whether a face image is **Real** or **AI-generated (DeepFake)**.

## 🧠 Dataset
Dataset used: **140k Real and Fake Faces** from Kaggle  
- Training images: 100,000  
- Validation images: 20,000  

## 🏗 Model Architecture
Custom CNN with:
- 3 Convolution layers
- ReLU activations
- MaxPooling
- Fully connected layers

## ⚙️ Training Setup
| Parameter | Value |
|----------|-------|
| Image size | 224×224 |
| Batch size | 32 |
| Epochs | 5 |
| Optimizer | Adam |
| Loss | CrossEntropyLoss |

## 📊 Results

| Epoch | Training Loss | Validation Accuracy |
|------|---------------|---------------------|
| 1 | 0.4772 | 86.65% |
| 2 | 0.2338 | 91.59% |
| 3 | 0.1349 | 94.53% |
| 4 | 0.0895 | **95.33%** |
| 5 | 0.0664 | 95.22% |

Best model saved at **Epoch 4**

## 🚀 Features
✔ Deep learning model built from scratch  
✔ Trained on 120k+ face images  
✔ Achieved 95%+ accuracy  
✔ Model prediction visualized on sample images  

## 💾 Model File
`best_deepfake_model.pth`

## 🔮 Future Work
- Add dropout layers
- Try transfer learning (ResNet/EfficientNet)
- Test on real-world DeepFake videos
