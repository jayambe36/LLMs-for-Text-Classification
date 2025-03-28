# Finetuning Large Language Models (LLMs) for Text Classification 

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jayambe36/LLMs-for-Text-Classification/blob/master/h2o_danube_classifier.ipynb)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jayambe36/LLMs-for-Text-Classification/blob/master/phi3_classifier.ipynb)


## Overview

This repository contains code and information related to fine-tuning lightweight language models for the text classification task. The models used in this project are Phi-3 and H2O-Danube. These models are chosen for their efficiency, fast training times, and competitive performance. They are designed to deliver good performance without requiring significant computational resources.


## Results
| Model           | Parameters | Trainable Token Position | Trainable Layers | Context Length          | Hardware         | Training Time | Training Accuracy | Validation Accuracy | Test Accuracy |
|-----------------|------------|-----------------|------------------|-------------------------|------------------|----------------|-------------------|---------------------|---------------|
| Phi-3 (3.8B)    | Instruct   | Last            | Classification Head | Dynamic Padding (Batch-wise) | T4 (Colab free) | 0.63 min       | 99.51%            | 99.32%              | 96.66%        |
| H2O-Danube (1.8B) | Instruct  | Last            | All-LoRA         | Dynamic Padding (Batch-wise) | T4 (Colab free) | 2.76 min       | 99.71%            | 99.32%              | 97.33%        |
