
# Image Captioning with Encoder-Decoder Networks

A comprehensive Deep Learning framework designed for automated image caption generation. This repository benchmarks two distinct paradigms: a classical **CNN-LSTM** architecture and a modern **Vision Transformer (ViT) + GPT-2** transformer pipeline.

---

## 📌 Project Overview

Image captioning operates at the intersection of Computer Vision and Natural Language Processing (NLP). The objective is to translate spatial visual signals into syntactically correct, context-aware descriptive captions. This repository implements and evaluates both recurrent and attention-driven approaches to understand visual scenes and generate natural language descriptions.

---

## 🏗️ Architecture & Methodologies

### 1. CNN (Encoder) + LSTM (Decoder)
* **Visual Feature Extraction (CNN Encoder):** Utilizes pre-trained convolutional backbones (e.g., ResNet) to process raw pixel data into dense latent feature representations.
* **Sequential Language Modeling (LSTM Decoder):** A recurrent LSTM decoder conditions on the visual embeddings, autoregressively decoding text captions token-by-token.

### 2. Vision Transformer (ViT Encoder) + GPT-2 (Decoder)
* **Patch-Based Visual Processing (ViT Encoder):** Splits images into structured patch sequences and processes them using multi-head self-attention mechanisms to capture global scene context.
* **Transformer Decoder (GPT-2):** Leverages a pre-trained autoregressive GPT-2 model to generate sentences based on encoded visual representations.
* **Custom Tokenization:** Implements custom vocabulary mapping with specialized sequence boundary tokens (`<startoftext>` / `<endoftext>`) to manage sequence boundaries cleanly.

---

## ⚡ Quick Start Guide

### Prerequisites
* Python 3.8 or higher
* CUDA-compatible GPU (recommended for training and inference)

### 1. Clone the Repository
```bash
git clone [https://github.com/laxmanr-wq/image-captioning-encoder-decoder.git](https://github.com/laxmanr-wq/image-captioning-encoder-decoder.git)
cd image-captioning-encoder-decoder






├── CNN(Encoder)+LSTM(Decoder).ipynb                 # CNN feature extractor with recurrent LSTM decoder pipeline
├── ViT(Encoder)+GPT2(Decoder)_Image_Captioning_Model.ipynb # Vision Transformer with GPT-2 generation model
├── README.md                                        # Project documentation and specifications
