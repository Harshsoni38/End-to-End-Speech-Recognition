# 🎙️ End-to-End Speech Recognition using RNN-Transducer

**Course:** EE5171 – Deep Learning Based Speech Processing  
**Institute:** IIT Madras  
**Toolkit:** [ESPnet](https://github.com/espnet/espnet) | **Framework:** PyTorch  
**Dataset:** [LibriSpeech-100h](https://www.openslr.org/12)   

---

## 🧠 Project Overview

This project focuses on building an **end-to-end Automatic Speech Recognition (ASR)** system using the **RNN-Transducer (RNN-T)** architecture with a **Conformer encoder**, implemented through the **ESPnet** toolkit.  
The model is trained and evaluated on the **LibriSpeech 100-hour subset**, a standard benchmark dataset for ASR research.

The goal was to explore how **Conformer-based encoders** improve contextual modeling, convergence speed, and recognition accuracy compared to standard RNN or Transformer architectures.

---

## 🚀 Objectives

- Implement a complete ASR pipeline using **ESPnet**.  
- Train an **RNN-Transducer model with a Conformer encoder** for speech-to-text transcription.  
- Analyze **training dynamics** through loss and WER (Word Error Rate) curves.  
- Tune hyperparameters to **improve model accuracy** and **training efficiency**.  
- Evaluate and compare architectural trade-offs and performance metrics.

---

## 🧩 Architecture

### **Model Components**
- **Encoder:** Conformer (combining convolution + self-attention for local and global context)  
- **Prediction Network:** RNN-based sequence predictor  
- **Joint Network:** Feed-forward layer combining encoder and prediction outputs  
- **Loss Function:** Transducer loss for alignment-free sequence training  

### **Key Advantages**
- Better handling of long-range dependencies via **self-attention**.  
- Enhanced local feature extraction through **convolutional modules**.  
- Faster convergence and improved WER performance.

---
