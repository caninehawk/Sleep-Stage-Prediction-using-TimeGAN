# 💤 Sleep Stage Prediction using TimeGAN and GRU  
_Reproducible Colab implementation combining actigraphy and PSG data from the MESA Sleep Study_

---

![Python](https://img.shields.io/badge/Python-3.10-blue.svg)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.13-orange.svg)
![Google Colab](https://img.shields.io/badge/Google%20Colab-Notebook-yellow.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

---

## 📘 Overview

This repository provides a **Google Colab notebook** implementing the research work:

> **“Daytime Activity Context Improves Nighttime Sleep Stage Prediction using TimeGAN-Augmented Sequences”**  
> *Sandeep Shandilya Katna, San José State University (2025)*

The notebook delivers an **end-to-end reproducible pipeline** that:
- Processes **MESA Sleep Study** actigraphy and PSG data  
- Extracts statistical and circadian activity features  
- Balances minority sleep stages (N1, N3, REM) using **TimeGAN**  
- Trains **LSTM**, **GRU**, **CNN**, and **MLP** models  
- Evaluates using **subject-wise Group K-Fold (K=5)** cross-validation  

---

## 📓 Open in Colab

👉 [**Run on Google Colab**](https://colab.research.google.com/github/sandeepshandilya/sleep-stage-timegan/blob/main/SleepStage_TimeGAN.ipynb)

---

## 🧠 Dataset

The notebook uses data from the **MESA Sleep Ancillary Study (2010–2013)** — a subset of the **Multi-Ethnic Study of Atherosclerosis (MESA)**.

📦 Dataset link: [https://sleepdata.org/datasets/mesa](https://sleepdata.org/datasets/mesa)

Each participant includes:
- **Actigraphy:** 7 days of wrist-worn accelerometer data  
- **Polysomnography (PSG):** Overnight sleep stage scoring  
- **Validated sleep questionnaires**

Upload your extracted files to your Colab runtime or mount Google Drive.


---

## ⚙️ Setup

Run the following cell in your Colab notebook to install dependencies:

```python
!pip install tensorflow==2.13.0 torch==2.1.0 scikit-learn==1.4.0 sdv matplotlib seaborn
```
