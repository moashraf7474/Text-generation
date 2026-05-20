# 🔥 Character-Level Text Generation using LSTM

This project is a simple Natural Language Processing (NLP) model built using PyTorch LSTM that learns character-level patterns from text data and generates new text based on a given input seed.

---

## 🚀 Project Overview

- Build a character-level language model
- Train an LSTM network on text data
- Generate new text character-by-character
- Interactive interface using Gradio

---

## 🧠 How It Works

The model learns to predict the next character in a sequence:

Input: "to be or"  
Output: "to be or not to be..."

Pipeline:
1. Data preprocessing (character tokenization)
2. Convert text → numerical encoding
3. Create sequences (X → Y pairs)
4. Train LSTM model
5. Generate text using sampling

---

## 🏗️ Model Architecture

- Embedding Layer
- LSTM Layer
- Fully Connected Layer (Linear)
- Softmax for probability distribution

---

## 📦 Tech Stack

- Python
- PyTorch
- NumPy
- Gradio
- Jupyter Notebook / VS Code

---

## ⚙️ Training Details

- Model: LSTM (Character-level)
- Loss Function: CrossEntropyLoss
- Optimizer: Adam
- Sequence Length: 20–50
- Batch Size: 64–256
- Temperature Sampling used in generation

---

## 🎯 Features

- Character-level language modeling
- Text generation from seed input
- Temperature control for creativity
- Interactive web UI using Gradio

---

## 🖥️ How to Run

### Install dependencies
```bash
pip install torch gradio
