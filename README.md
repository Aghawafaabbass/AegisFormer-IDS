# AegisFormer-IDS: Fast FT-Transformer for Real-Time Intrusion Detection on NSL-KDD


## Citation & Publication

This project accompanies the published research paper:

**Agha, W. A.** (2025). *AegisFormer-IDS: Fast FT-Transformer for Real-Time Intrusion Detection on NSL-KDD*. Zenodo.  
🔗 https://doi.org/10.5281/zenodo.18031860

## Abstract

In the event of insecurity of network infrastructures due to cyber attacks, real-time intrusion detection systems (IDS) play a critical role in ensuring protection to these network infrastructures. This paper describes AegisFormer-IDS, a lightweight, feature-efficient Feature-Tokenized Transformer (FT-Transformer) network that is best used to perform a fast binary classification of network traffic as either normal or anomalous. Our work (based on the NSL-KDD dataset) embraces best practices such as the label encoding of categorical features, the standardization of numerical features, and binary re-labeling (normal vs. attack) to facilitate movement to a simplified Transformer encoder architecture. The architecture is very compact, with projection of features, multi-head self-attention layers, and a fully connected classification head that allows quick inference without compromising performance. AegisFormer-IDS, trained on 10 epochs with the PyTorch framework, Adam optimization, cross-entropy loss, and a learning rate scheduler, achieves validation accuracy over 99% and F1-score above 0.99 on an 80/20 train/validation split. Empirical evidence shows that it is better in speed, accuracy, and resource consumption than standard deep learning models, and can be deployed in real-time where resource constraints are present. The gap between transformer-based progress and scalable high-fidelity network security utilization is bridged in this work, leading to scalable applications of network security.

## Keywords

Intrusion Detection System (IDS), FT-Transformer, NSL-KDD Dataset, Real-Time Network Security, Deep Learning, Binary Classification, Transformer Encoder, PyTorch Implementation, Cyber Threat Detection, Feature Preprocessing

## Key Results

- Validation Accuracy: >99%
- Weighted F1-Score: >0.99
- Low inference latency suitable for real-time deployment
- Outperforms baseline models (MLP, LSTM) in both accuracy and efficiency

## Key Contributions

- Introduction of AegisFormer-IDS, a lightweight FT-Transformer optimized for real-time intrusion detection.
- A complete preprocessing pipeline tailored for the NSL-KDD dataset to enable effective use with transformer models.
- Comprehensive empirical evaluation demonstrating superior performance and lower latency compared to traditional deep learning baselines.

## Dataset

The NSL-KDD dataset (an improved version of the KDD Cup 1999 dataset) is used as the benchmark. It contains:
- 125,973 training samples
- 22,544 test samples
- 41 features (numerical and categorical)

Dataset download: https://www.unb.ca/cic/datasets/nsl.html

## Repository Files

- `AegisFormer_IDS_NSLKDD.ipynb` – Main Jupyter notebook containing the complete implementation, preprocessing, model definition, training, evaluation, and results.

## How to Run

### Option 1: Google Colab (Recommended – No local setup required)

Open directly in Colab:  
https://colab.research.google.com/drive/10bMm5RDcJ2RGGSQA4bsQBQPSzubpiv4v

Run all cells (Runtime → Run all).

### Option 2: Run Locally

**Requirements**
- Python 3.7+
- Jupyter Notebook/Lab

**Install dependencies**
```bash
pip install torch pandas numpy scikit-learn matplotlib seaborn
Run the notebook
Bashjupyter notebook AegisFormer_IDS_NSLKDD.ipynb
Author
Agha Wafa Abbas
Lecturer, School of Computing, University of Portsmouth, United Kingdom
Lecturer, School of Computing, Arden University, Coventry, United Kingdom
Lecturer, School of Computing, Pearson, London, United Kingdom
Lecturer, School of Computing, IVY College of Management Sciences, Lahore, Pakistan
License
This project is licensed under the MIT License – see the LICENSE file for details.
