#  Traffic Sign Detection

A deep learning project for classifying traffic signs using **Convolutional Neural Networks (CNNs)** and **Transfer Learning (MobileNetV2)**. The trained models can recognize different traffic signs from images, useful for autonomous driving and intelligent transportation systems.

---

## Features

* Preprocessing and augmentation of traffic sign dataset.
* Two models implemented:

  * **CNN (from scratch)**
  * **MobileNetV2 (transfer learning)**
* Trained models saved as `.h5` files for inference.
* Jupyter notebooks for training and evaluation.

---

## Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/sahithkasam/traffic-sign-detection.git
   cd traffic-sign-detection
   ```

2. Install dependencies:

   ```bash
   pip install tensorflow keras numpy pandas matplotlib scikit-learn
   ```


---

## ▶️ Usage

### Run CNN Model:

1. Open the notebook:

   ```bash
   jupyter notebook CNN.ipynb
   ```
2. Run all cells to train or evaluate the CNN model.

### Run MobileNetV2 Model:

1. Open the notebook:

   ```bash
   jupyter notebook MobileNetV2.ipynb
   ```
2. Run all cells to train/evaluate using transfer learning.

### Load Pretrained Models:

You can directly load pretrained models:

```python
from tensorflow.keras.models import load_model

# Load CNN model
cnn_model = load_model("traffic_sign_cnn.h5")

# Load MobileNetV2 model
mobilenet_model = load_model("traffic_sign_mobilenetv2.h5")
```

---

## 📊 Example Results

* CNN achieved \99.3% accuracy on test set.
* MobileNetV2 achieved \95% accuracy on test set (usually higher due to transfer learning).






