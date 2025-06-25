# Transformer Network Implementation from Scratch 🔄🧠

This repository contains my implementation of the Transformer Network programming assignment, the final project of the **DeepLearning.AI Deep Learning Specialization**.

## 📘 Project Overview

This project provides a deep, hands-on dive into the groundbreaking Transformer architecture introduced in the paper ["Attention Is All You Need"](https://arxiv.org/abs/1706.03762). The goal is to build a complete Transformer model from scratch using TensorFlow and Keras, implementing all core components that enable state-of-the-art sequence-to-sequence modeling in Natural Language Processing.

Unlike traditional recurrent models (RNNs, LSTMs), the Transformer relies entirely on attention mechanisms, enabling significant parallelization and achieving superior performance in tasks like machine translation and text summarization.

## 🧠 Key Architectural Components

- **Positional Encoding:**  
  Incorporates sequence order by adding sinusoidal positional encodings to input embeddings, compensating for the lack of recurrence.

- **Masking:**  
  - *Padding Mask* to ignore zero-padding tokens in input sequences.  
  - *Look-ahead Mask* in the decoder to prevent attending to future tokens during training.

- **Self-Attention Mechanism:**  
  Implements Scaled Dot-Product Attention using Query (Q), Key (K), and Value (V) matrices to weigh word importance contextually.

- **Multi-Head Attention:**  
  Runs multiple attention heads in parallel to capture diverse representation subspaces.

- **Encoder Block:**  
  Comprises Multi-Head Attention and Feed-Forward sub-layers with residual connections and Layer Normalization.

- **Decoder Block:**  
  Includes Masked Multi-Head Attention, Encoder-Decoder Attention, and Feed-Forward sub-layers, all with residual connections and Layer Normalization.

- **Full Transformer Model:**  
  Combines stacked encoder and decoder blocks with a final linear layer and softmax to generate output probabilities.

## 🎓 Source & Acknowledgements

This project is the final programming assignment from **Course 5: Sequence Models** in the  
[DeepLearning.AI Deep Learning Specialization](https://www.coursera.org/specializations/deep-learning) on Coursera.

All credit for the original problem, instructional design, and conceptual framework goes to DeepLearning.AI and the course instructors.

### Reference  
Vaswani, A., Shazeer, N., Parmar, N., Uszkoreit, J., Jones, L., Gomez, A. N., ... & Polosukhin, I. (2017). [Attention is all you need](https://arxiv.org/abs/1706.03762).

---

> ✨ A foundational project demonstrating how attention mechanisms revolutionized NLP by enabling efficient and effective sequence modeling.
