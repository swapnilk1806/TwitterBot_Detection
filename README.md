# 🤖 Twitter Bot Detection

A machine learning project aimed at detecting Twitter bots based on content and graph features extracted from public tweet data. This system uses **Relevance Vector Machine (RVM)** with a linear kernel for classification, achieving a testing accuracy of **81.25%**.

---

## 📘 Introduction

Social media platforms, especially Twitter, have seen a surge in automated accounts (bots) that are often used for misinformation, spam, or malicious influence. This project builds a bot detection model by combining user metadata, content features, and graph-based features extracted from Twitter's public APIs and datasets.

This system helps in identifying suspicious Twitter accounts using machine learning—specifically **RVM (Relevance Vector Machines)**—trained on real datasets.  

---

## 🎯 Objectives

- Extract and merge **user metadata**, **tweet-level content**, and **graph features** from Twitter.
- Train a classifier to differentiate between bots and human accounts.
- Use publicly available bot detection datasets for model training and evaluation.

---

## ✨ Features

- 🔍 **Tweet and User Metadata Extraction** using Twitter API endpoints.
- 🧠 **Machine Learning Classification** using RVM with a linear kernel.
- 📊 **Feature Merging and Preprocessing** from various sources (`Content_Data.csv`, `Graph_Data.csv`).
- ✅ **Model Accuracy: 81.25%** on the test set.
- 📁 Lightweight, easy-to-extend architecture for new models (SVM, RF, etc.).

---

## 🧾 Dataset Files

| File Name             | Description                                  |
|-----------------------|----------------------------------------------|
| `Content_Data.csv`    | Content-based features (e.g., tweet stats)   |
| `Graph_Data.csv`      | Graph-based features (follower/following)    |
| `Training_Data.csv`   | Final merged dataset used for ML training    |
| `MergingTrainingData.py` | Script to merge content and graph features |
| `RVMTrainingModel.py` | Main script to train the model using RVM     |

> Datasets sourced from:  
[Bot Repository Datasets](https://botometer.iuni.iu.edu/bot-repository/datasets.html)

---

## ⚙️ Setup Instructions

### 📦 Prerequisites

Install required Python packages:
```bash
pip install numpy pandas scikit-learn matplotlib
pip install getoldtweets3
