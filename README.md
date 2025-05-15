# ❄️ Antarctic Glacier Analysis

To develop a deep learning model that predicts future Antarctic glacier distributions by learning from historical satellite time series images.

---

## 🔍 Overview

This project builds and evaluates a deep learning-based forecasting system to predict monthly Antarctic glacier coverage using historical satellite image time series.
It explores various temporal models including ConvLSTM2D, Transformer, AutoEncoder, and GAN-based architectures. The pipeline also integrates visualization tools and a lightweight web application for result interaction.

🗓️ Project Period: April 28, 2025 – May 16, 2025

---

## 📂 Project Structure
```
.
├── data/                                    # Raw and processed datasets
├── docs/                                    # Supporting documents and presentations
├── code/                                    # Codes
└── README.md
```

---

## 🚀 Features

- Grayscale transformation and 256×256 resizing of satellite image data (1978.11–2025.04)
- Moving average, extent distribution, and seasonal decomposition for EDA
- Forecasts 60 months ahead using autoregressive ConvLSTM2D-based sequence generation
- Flask-based web app to input future dates and return predicted glacier imagery
- Modular structure for testing different deep learning models

---

## 🧪 Models Used
- AutoEncoder-based model
- GRU-based model

---

## 👥 Contributors

- [Choi Hwankyu]()
- [Park Junho]()
- [Kim Sihwan]()
- [Kimm Soo Min](https://github.com/somnio-kimm)
