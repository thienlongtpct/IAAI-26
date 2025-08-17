# Meta-Learning Framework for Intrusion Detection

This repository contains the implementation of the meta-learning framework for cross-protocol intrusion detection, supporting both balanced and imbalanced datasets. The framework is designed to detect novel attacks while preserving generalization across protocols (UDP ↔ TCP).

## Dataset

- `5g_nidd.csv`: The dataset used for all experiments, containing source and target attack samples along with benign traffic.

## Notebooks

- `anomaly_all_meta_learning_udp_tcp_balanced.ipynb`: Balanced dataset experiments for UDP → TCP adaptation.
- `anomaly_all_meta_learning_udp_tcp.ipynb`: Imbalanced dataset experiments for UDP → TCP adaptation.
- `anomaly_all_meta_learning_tcp_udp_balanced.ipynb`: Balanced dataset experiments for TCP → UDP adaptation.
- `anomaly_all_meta_learning_tcp_udp.ipynb`: Imbalanced dataset experiments for TCP → UDP adaptation.
- `anomaly_meta_learning.ipynb`: Core meta-learning framework implementation for single/multi-stage experiments.

## Usage

1. Open the appropriate Jupyter notebook for your scenario (balanced or imbalanced, UDP → TCP or TCP → UDP).  
2. Make sure `5g_nidd.csv` is in the same folder or update the path in the notebook.  
3. Run the cells sequentially to reproduce experiments, including training, testing, and plotting results.  

## Features

- **Balanced and Imbalanced Dataset Support**  
- **Dependency Control** via alpha parameter  
- **Single-Stage and Multi-Stage Meta-Learning**  
- **Cross-Protocol Transfer** (UDP ↔ TCP)  

## Requirements

- Python 3.8+  
- Jupyter Notebook  
- Packages: `numpy`, `pandas`, `scikit-learn`, `torch`, `matplotlib`, `seaborn`  