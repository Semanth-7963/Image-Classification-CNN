# 🧠 Image Classification using CNN with Attention Visualization

A deep learning project that developed an image classification system using Convolutional Neural Networks (CNN) with attention-based visualization, built with TensorFlow and Keras.

---

## 📌 Project Overview

This project implements a CNN-based image classifier trained on the CIFAR-10 dataset. The model uses a convolutional stem, a residual trunk, and an attention pooling mechanism to classify images into 10 categories. A key feature of this project is the **attention map visualization** — showing which regions of an image the model focuses on when making predictions.

---

## 🚀 Results

| Metric | Score |
|---|---|
| **Top-1 Accuracy** | 71.8% |
| **Top-5 Accuracy** | 98.2% |
| **Final Loss** | 0.084 |
| **Validation Accuracy** | 72.2% |

---

## 🗂️ Dataset

- **CIFAR-10** — 60,000 images across 10 classes
- Classes: airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck
- Image size: 32×32 pixels (RGB)
- Split: 40,000 training / 10,000 validation / 10,000 test

---

## 🛠️ Tech Stack

- **Language:** Python 3.x
- **Frameworks:** TensorFlow, Keras
- **Libraries:** NumPy, Matplotlib
- **Model Components:**
  - Convolutional Stem
  - Residual Trunk with Squeeze-Excite blocks
  - Attention Pooling Layer
  - Warm-up Cosine Learning Rate Scheduler

---

## 📁 Project Structure

```
Image-Classification-CNN/
│
├── convoltuion.py        # Main model training and evaluation script
├── README.md             # Project documentation
```

---

## ⚙️ How to Run

### 1. Clone the repository
```bash
git clone https://github.com/SemanthParvataneni/Image-Classification-CNN.git
cd Image-Classification-CNN
```

### 2. Install dependencies
```bash
pip install tensorflow keras numpy matplotlib
```

### 3. Run the model
```bash
python convoltuion.py
```

> The CIFAR-10 dataset will be downloaded automatically on first run (~170MB).

---

## 🔍 Attention Visualization

The model generates attention maps that highlight which parts of an image influenced the prediction. Below is an example output:

| Original Image | Attention Map |
|---|---|
| Raw CIFAR-10 image | Heatmap overlay showing model focus areas |

This helps interpret **why** the model makes specific predictions — an important aspect of explainable AI.

---

## 📈 Training Details

| Parameter | Value |
|---|---|
| Epochs | 5 |
| Batch Size | 128 |
| Optimizer | AdamW |
| Learning Rate | 0.001 (with warm-up cosine schedule) |
| Weight Decay | 0.0001 |

---

## 👤 Author

**Semanth Parvataneni**  
Developed an image classification system using deep learning techniques as part of my ML portfolio.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
