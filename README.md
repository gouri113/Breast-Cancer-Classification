# Breast Cancer Classification Model
### Using Deep Learning — Neural Network & Multi-Model Comparison

![Python](https://img.shields.io/badge/Python-3.8+-blue?style=flat&logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?style=flat&logo=tensorflow)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-Latest-green?style=flat&logo=scikit-learn)
![License](https://img.shields.io/badge/License-MIT-yellow?style=flat)

---

## Overview

This project builds a **binary classification model** to detect whether a breast tumor is **Malignant (Cancerous)** or **Benign (Non-Cancerous)** using the **Wisconsin Breast Cancer Dataset**.

The primary model is a **Deep Learning Neural Network** built with TensorFlow/Keras, benchmarked against three classical machine learning models — Logistic Regression, SVM, and Random Forest — for a comprehensive performance comparison.

> ⚠️ **Disclaimer:** This is a research/educational project. It is not intended for real clinical diagnosis. Always consult a qualified medical professional.

---

## Problem Statement

Given **30 numerical features** extracted from a breast mass biopsy (cell radius, texture, perimeter, area, concavity, etc.), predict:

| Label | Meaning |
|-------|---------|
| `0` | Malignant — Cancerous |
| `1` | Benign — Non-Cancerous |

The key clinical priority is **maximizing recall for Malignant cases** — ensuring cancerous tumors are never missed.

---

## Dataset

| Property | Details |
|----------|---------|
| **Source** | `sklearn.datasets.load_breast_cancer()` |
| **Samples** | 569 |
| **Features** | 30 numerical features |
| **Missing Values** | None |
| **Classes** | 2 (Malignant: 212, Benign: 357) |

### Feature Groups
All 30 features are derived from **10 base measurements**, each computed as mean, standard error, and worst value:

> Radius · Texture · Perimeter · Area · Smoothness · Compactness · Concavity · Concave Points · Symmetry · Fractal Dimension

---

## Neural Network Architecture
