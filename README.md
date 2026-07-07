# 🎥 Temporal Sentence Grounding in Videos using Multi-Modal Learning

![Python](https://img.shields.io/badge/Python-3.10-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-red)
![Computer Vision](https://img.shields.io/badge/Computer%20Vision-Project-green)
![NLP](https://img.shields.io/badge/NLP-BERT%20%2B%20BLIP-orange)
![University Project](https://img.shields.io/badge/Final%20Year-MSc%20Artificial%20Intelligence-success)

## 📌 Overview

This repository showcases my MSc Artificial Intelligence final-year dissertation project on **Temporal Sentence Grounding in Untrimmed Videos**.

The objective is to identify the temporal segment within a video that best matches a natural language query. This problem lies at the intersection of **Computer Vision**, **Natural Language Processing**, and **Multi-modal Learning**.

The project explores the fusion of visual and textual representations to localize events described in natural language.

---

## 🎯 Problem Statement

Given:

* An untrimmed video
* A natural language sentence describing an event

The model predicts:

* The most relevant temporal segment within the video where the described event occurs.

---

## 🏗️ Model Architecture

The proposed pipeline consists of:

1. **Visual Feature Extraction**

   * ResNet-18
   * Frame-level feature extraction

2. **Text Feature Extraction**

   * BLIP generated captions
   * BERT embeddings
   * BiLSTM encoding

3. **Feature Fusion**

   * L2 Normalization
   * Concatenation of visual and textual embeddings
   * Multi-Layer Perceptron (MLP)

4. **Prediction**

   * Temporal segment classification
   * Cross-Entropy Loss

---

## 📂 Dataset

**ActivityNet Captions**

Subset used for experimentation:

* Training Videos: **1000**
* Test Videos: **200**
* Approximately **2300** training sentence annotations
* Approximately **700** testing queries

---

## ⚙️ Methodology

The workflow followed these stages:

* Video preprocessing
* Feature extraction using ResNet-18
* Caption generation
* Text encoding with BERT + BiLSTM
* Multi-modal feature fusion
* MLP-based prediction
* Evaluation using Recall@1 and Mean tIoU

---

## 📊 Results

| Metric               |      Score |
| -------------------- | ---------: |
| Recall@1 (IoU = 0.3) | **19.90%** |
| Recall@1 (IoU = 0.5) |  **9.54%** |
| Mean tIoU            | **14.32%** |

---

## 🔬 Key Contributions

* Combined visual and textual representations for temporal localization.
* Investigated L2-normalized feature fusion.
* Evaluated multiple feature extraction strategies.
* Demonstrated an end-to-end pipeline for video-language grounding.

---

## 🚀 Future Improvements

Possible directions include:

* Finer temporal window generation
* IoU-aware loss functions
* Transformer-based temporal reasoning
* Larger-scale ActivityNet training
* Context-aware multi-modal fusion
* End-to-end temporal proposal generation

---

## 🎥 Demo Video

A demonstration of the project can be viewed here:

**Google Drive**

**https://drive.google.com/drive/folders/1yJI3x4IOwmwJKFrxJmXwb9NoWy0AHS6w?usp=drive_link**

---

## ⚠️ Source Code

The implementation was developed as part of my MSc dissertation project.

Due to university intellectual property and submission policies, I am **unable to publicly release the source code**.

This repository is intended to document the research, methodology, experimental setup, and project demonstration.

---

## 🎓 Dissertation

**Degree:** MSc Artificial Intelligence

**Project Area:** Computer Vision • Natural Language Processing • Multi-modal Learning

---

## 👨‍💻 Author

**Mayank Mishra**

Data Scientist | Artificial Intelligence | Machine Learning | Computer Vision | NLP



---

## ⭐ Acknowledgements

I would like to thank my dissertation supervisor and the School of Computer Science for their guidance and support throughout this research project.
