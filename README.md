# Fake News Detection Using Transformer-Based Deep Learning Models

## Overview
This project compares traditional machine learning, basic neural networks, and transformer-based deep learning models for binary fake-news detection.

## Dataset
Dataset: `davanstrien/WELFake` from Hugging Face.  
Task: classify news articles as fake or real.

## Models
1. TF-IDF + Logistic Regression
2. Embedding MLP
3. BiLSTM
4. DistilBERT fine-tuning

## Evaluation
Primary metric: macro F1-score.  
Additional metrics: accuracy, precision, recall, ROC-AUC, confusion matrix.

## Controlled comparison / ablation
The notebook compares body-only input against title+body input using the same TF-IDF Logistic Regression setup.

## How to run
1. Open the notebook in Google Colab.
2. Select GPU runtime.
3. Run all cells from top to bottom.
4. Adjust `MAX_ROWS`, `EPOCHS_NN`, and `EPOCHS_TRANSFORMER` for final experiments.

## Reproducibility
Random seed: 42.  

## Repository structure
```text
.
├── COMP_690_AH2_Final_Draft.ipynb
├── README.md
├── requirements.txt
```

## Responsible use
This model should be used only as a decision-support or triage tool. It should not be treated as an automatic truth authority.