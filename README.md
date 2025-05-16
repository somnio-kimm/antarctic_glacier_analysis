# ❄️ Antarctic Glacier Analysis

To develop a deep learning model that predicts future Antarctic glacier distributions by learning from historical satellite time series images.

---

## 🔍 Overview

This project builds and evaluates a deep learning-based forecasting system to predict monthly Antarctic glacier coverage using historical satellite image time series.
It explores various temporal models including ConvLSTM2D, Transformer, AutoEncoder, and GAN-based architectures. The pipeline also integrates visualization tools and a lightweight web application for result interaction.

🗓️ Project Period: April 28, 2025 – May 16, 2025

📊 Data Source: 
- National Snow and Ice Data Center: https://nsidc.org/data/seaice_index/data-and-image-archive

---

## 📂 Project Structure
```
.
├── code/      # Codes
├── data/      # Raw and processed datasets
├── docs/      # Supporting documents and presentations
└── README.md
```

---

## 🚀 Features

- Grayscale transformation and 256×256 resizing of satellite image data (1978.11–2025.04)
- Moving average, extent distribution, and seasonal decomposition for EDA
- Use 60-months images to forecast 1-month image using autoregressive sequence generation
- Flask-based web app to input future dates and return predicted glacier imagery

---

## 🧪 Models Used
- SARIMAX
- CNN
- LSTM
- Transformer
- ConvLSTM2D-based model
- AutoEncoder+GRU-based model
- U-Net+GAN-based model

---

## 👥 Contributors

- [Choi Hwankyu]()
- [Park Junho](https://github.com/Moulru)
- [Kim Sihwan]()
- [Kimm Soo Min](https://github.com/somnio-kimm)
