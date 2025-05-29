
# 🎭 Deepfake Detection using EfficientViT and Temporal Modeling

A lightweight and highly accurate deepfake video detection system using **EfficientViT** for frame-level embeddings and **Temporal Convolutional Networks (TCN)** for sequence modeling. GPU used : T4 GPU

---

## 🔍 Overview

This project focuses on detecting deepfake videos by leveraging spatial and temporal features:

- **Spatial Features**: Extracted using `EfficientViT`, a vision transformer designed for fast and efficient image encoding.
- **Temporal Features**: Modeled using a 1D convolutional layer to capture inter-frame inconsistencies.
- Achieved **100% accuracy** and **1.0000 AUC** on the test set.

---

## 📌 Key Features

- ✅ Frame-wise feature extraction using a pretrained `EfficientViT`
- ✅ Temporal convolution over time sequences of frames
- ✅ Binary classification (real vs fake)
- ✅ ROC-AUC and confusion matrix evaluation
- ✅ Visual performance tracking (Accuracy, AUC)

---


## 📂 Dataset Structure

```
deepfake_dataset/
├── train/
│   ├── real/
│   └── fake/
└── test/
    ├── real/
    └── fake/
```

Each video is preprocessed by extracting **10 uniformly spaced frames** resized to `224x224`.


### Evaluated metrics:
```
✅ Accuracy: 1.0000
✅ AUC Score: 1.0000
✅ Confusion Matrix:
[[20  0]
 [ 0 20]]
```

---

---

## 🔮 Future Work

- 🎙️ Add audio-visual fusion for enhanced detection
- 🧠 Extend to classify types of manipulations
- 📱 Deploy using ONNX or TensorRT for real-time usage
- 🔍 Introduce model explainability (e.g., Grad-CAM)

---

## 📌 Author

<b>**Anugya Saxena**</b>  
🎓 B.Tech CSE @ DTU  
🏅 NTSE Scholar | AI-ML Enthusiast | AIMS DTU | GDSC DTU

---

## 📜 License

This project is licensed under the MIT License.

---

## 🤝 Acknowledgments

- AIMS-DTU 
