# Multi-Domain Sentiment Classification Using BERT Mini

## Project Overview

This project explores sentiment classification of product reviews across four domains: Books, DVD, Electronics, and Kitchen & Housewares.

The aim is to compare different approaches for adapting BERT Mini to classify reviews as positive or negative.

## Models Compared

Three approaches were investigated:

1. **Frozen Encoder Baseline** – Uses pretrained BERT Mini representations while training the classification layer.
2. **Full Fine-Tuning (FFT)** – Updates the model parameters for sentiment classification.
3. **Low-Rank Adaptation (LoRA)** – Fine-tunes a smaller set of parameters to reduce training requirements.

## Dataset and Evaluation

- **Dataset:** Multi-Domain Sentiment Dataset
- **Reviews:** 7,853 cleaned reviews
- **Evaluation metrics:** Accuracy, F1-score, training time, and trainable parameters
- **Environment:** Google Colab with GPU support

## Key Findings

Full Fine-Tuning achieved the highest test accuracy at approximately **85.37%**.

LoRA reduced the number of trainable parameters by more than **99%** compared with Full Fine-Tuning, demonstrating a trade-off between predictive performance and parameter efficiency.

## Technologies Used

Python · PyTorch · Hugging Face Transformers · PEFT/LoRA · scikit-learn · Google Colab

## Project Files

The Jupyter Notebook contains the implementation, experiments, evaluation results, and visualisations.

## Acknowledgement

Developed as part of academic coursework at Coventry University. ChatGPT was used to support technical understanding, debugging, and parts of the implementation and documentation. The suggestions were reviewed and tested.
