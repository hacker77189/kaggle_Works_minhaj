# 🌍 NDVI-based Land Cover Classification

This project was developed for a hackathon focused on **multiclass land cover classification** using **NDVI (Normalized Difference Vegetation Index)** time series data. The task involves building a logistic regression model to classify various land types based on temporal NDVI patterns.

---

## 🧠 Problem Statement

Use NDVI time-series data to classify land cover into one of the following classes:

- **Water**
- **Impervious**
- **Farm**
- **Forest**
- **Grass**
- **Orchard**

The model must be robust to noise and missing data and capable of generalizing well to clean test data.

---

## 📊 Key Concept: NDVI

NDVI is a widely used vegetation index calculated from satellite data:

```
NDVI = (NIR - RED) / (NIR + RED)
```

- **NIR** = Near-Infrared reflectance  
- **RED** = Red reflectance  

NDVI values help detect vegetation health and type by analyzing light absorption/reflection patterns.

---

## 📁 Dataset Description

Each row represents a unique sample and contains:

- **ID**: Unique identifier
- **class**: Ground truth label (target)
- **27 NDVI time points**: Columns like `20150720_N`, `20150602_N`, etc. Each column represents NDVI for a specific date, forming a **temporal series**.

---

## ⚠️ Challenges in Data

- **Noise**: Cloud cover affects satellite imagery; polygon labels may be imprecise.
- **Missing Values**: Cloud obstruction leads to missing NDVI values.
- **Seasonal Trends**: Vegetation patterns change over time, requiring careful feature extraction.

---

## 🛠️ Allowed Techniques

- ✅ Denoising
- ✅ Missing value imputation
- ✅ Feature engineering on NDVI time series
- ❌ No models other than **Logistic Regression** are allowed.

---

## 🏆 Leaderboard Setup

- **Public Leaderboard (89% of test data)**: Immediate feedback.
- **Private Leaderboard (11% of test data)**: Final evaluation. This subset is **clean** and **noise-free**, testing true generalization.

---

## 📌 Goal

Build a logistic regression classifier that:

- Handles **noisy** and **missing** data effectively.
- Learns **seasonal trends** in vegetation via NDVI sequences.
- Generalizes well from noisy training data to clean test data.

---

## 🤖 Model Constraints

Only **multiclass logistic regression** is allowed.

You are free to apply:

- Temporal smoothing
- Time-series feature engineering (e.g., seasonal trends, derivatives, peaks)
- Statistical imputation for missing values

---

## 📬 Contact

For collaboration, questions, or suggestions:

**Minhaj Alam**  
[GitHub](https://github.com/hacker77189) | [Email](mailto:your-email@example.com)

---
