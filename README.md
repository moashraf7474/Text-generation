# 🔥 LSTM Text Generator (Shakespearean Style)

An end-to-end deep learning project that builds, trains, and deploys a character-level Language Model using a **Long Short-Term Memory (LSTM)** network in PyTorch. The model is trained on the classic Project Gutenberg Shakespeare dataset to capture and mimic stylistic early modern English syntax, patterns, and vocabulary.

An interactive **Gradio Web UI** is integrated directly into the project, allowing you to generate custom text sequences with adjustable generation length and sampling creativity (temperature).

---

## 🚀 Features

* **Character-Level Modeling:** Learns patterns text-by-text, allowing it to generate entirely unique words, punctuation structures, and character alignments.
* **Robust PyTorch Pipeline:** Built utilizing `TensorDataset` and `DataLoader` with optimization techniques like memory pinning for accelerated GPU training.
* **Interactive Web Interface:** Deploys instantly via Gradio with an accessible public URL link, allowing users to tweak parameters seamlessly without rewriting code.
* **Sampling Flexibility:** Implements temperature-scaled softmax distribution sampling to control the balance between predictable text and creative randomness.

---

## 📊 Model Architecture & Hyperparameters

The network utilizes an embedding layer followed by stacked recurrent layers to process the sequential nature of characters.

### Architecture Overview
1. **Embedding Layer:** Maps character indices into a continuous dense vector space.
2. **LSTM Network:** A deep 2-layer Recurrent Neural Network tracking sequential historical context across a sliding window of characters.
3. **Linear Layer:** Fully connected layer mapping hidden states back to the vocabulary dimension for next-character predictions.

### Hyperparameters Summary

| Parameter | Value | Description |
| :--- | :--- | :--- |
| **Vocabulary Size** | 91 | Total unique characters found in the dataset |
| **Sequence Length** | 50 | Number of historical characters given to predict the next |
| **Embedding Size** | 128 | Dimensionality of the character embeddings |
| **Hidden Size** | 256 | Number of features in the LSTM hidden state |
| **LSTM Layers** | 2 | Number of stacked LSTM layers |
| **Batch Size** | 256 | Number of sequence chunks processed concurrently |
| **Optimizer** | Adam (`lr=0.001`) | Optimization algorithm used during training |

---

## 🛠️ Installation & Setup
