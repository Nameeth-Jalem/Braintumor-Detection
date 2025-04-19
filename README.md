<div align="center">
  <h1>🧠 Brain Tumor Detection Using CNN</h1>
  <p><strong>Deep learning approach to detect brain tumors from MRI scans.</strong></p>

  <p>
    <a href="https://github.com/Nameeth-Jalem/Braintumor-Detection/stargazers"><img src="https://img.shields.io/github/stars/Nameeth-Jalem/Braintumor-Detection?style=social" /></a>
    <a href="https://github.com/Nameeth-Jalem/Braintumor-Detection/network/members"><img src="https://img.shields.io/github/forks/Nameeth-Jalem/Braintumor-Detection?style=social" /></a>
    <a href="https://github.com/Nameeth-Jalem/Braintumor-Detection/issues"><img src="https://img.shields.io/github/issues/Nameeth-Jalem/Braintumor-Detection" /></a>
  </p>
</div>

---

## 🧠 Project Overview

This project uses **Convolutional Neural Networks (CNN)** to classify MRI scans as either showing a **brain tumor** or **no tumor**.

---

## ⚙️ Model Configuration (YAML)

```yaml
model:
  name: CNN
  input_shape: 150x150x3
  epochs: 15
  optimizer: adam
  loss_function: categorical_crossentropy
  metrics:
    - accuracy
    - precision
    - recall
  dataset:
    classes: [yes, no]
    prediction_folder: pred
