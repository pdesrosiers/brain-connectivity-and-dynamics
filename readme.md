# Graph and Dynamical Systems Approaches to Whole-Brain Neuronal Networks

This repository contains interactive Jupyter notebooks prepared for a hands-on session held as part of the **Frontiers in Neurophotonics Summer School 2025**.

## Overview

Modern network science and computational modeling offer powerful tools to analyze brain connectivity and neuronal dynamics. In this hands-on session, you will explore how to represent structural and functional brain networks as graphs, extract meaningful features, and simulate activity using biologically inspired models.

## Notebooks

### 1. Structural and Functional Network Analysis

This notebook guides you through:

- **Analyzing structural connectivity** from zebrafish brain data  
- **Computing graph-theoretical features** such as degree, clustering, and path metrics  
- **Inferring functional connectivity** from calcium imaging data  
- **Quantifying structure–function coupling** using correlation and node-level metrics

📁 [`structural_functional_connectivity_tutorial.ipynb`](https://github.com/pdesrosiers/Graph-and-dynamical-systems-approaches-to-whole-brain-neuronal-networks/blob/main/structural_functional_connectivity_tutorial.ipynb)  
▶️ [Open in Colab](https://colab.research.google.com/github/pdesrosiers/Graph-and-dynamical-systems-approaches-to-whole-brain-neuronal-networks/blob/main/structural_functional_connectivity_tutorial.ipynb)


---

### 2. Neural Dynamics Simulation

This notebook focuses on:

- **Simulating single-neuron dynamics** and generating synthetic calcium traces  
- **Modeling population-level activity** in zebrafish-inspired neural circuits  
- **Comparing simulated activity with empirical patterns** from calcium imaging

📁   
▶️ 

---
## Data


All data used in these notebooks are publicly available. In particular, we rely on the following dataset:

**Dataset**: *Structural and genetic determinants of zebrafish functional brain networks*  
**Authors**: Antoine Légaré, Mado Lemieux, Vincent Boily, Sandrine Poulin, Arthur Légaré, Patrick Desrosiers, Paul De Koninck  
**Repository**: Borealis – Sentinelle Nord, Université Laval  
**DOI**: [https://doi.org/10.5683/SP3/IIVGOB](https://doi.org/10.5683/SP3/IIVGOB)  
**Description**: Whole-brain calcium imaging data from larval zebrafish (5–7 dpf), including synchronized tail movement recordings.  
**Note**: A subset of this dataset is included in the [`/data`](./data/) folder for educational use.


---

## Getting Started

### ▶️ Run in Google Colab (Recommended)

You can run each notebook directly in your browser using **Google Colab** — no installation required. Just click the **"Open in Colab"** badge provided under each notebook title.

Make sure you're logged into a Google account and accept any permissions required to access files.

### 🖥️ Run Locally (Optional – for advanced users)

If you prefer to run the notebooks on your own machine:

1. Clone the repository 

	```bash
   git clone https://github.com/pdesrosiers/Graph-and-dynamical-systems-approaches-to-whole-brain-neuronal-networks.git
   cd Graph-and-dynamical-systems-approaches-to-whole-brain-neuronal-networks
   ```
	
2.	Install the required Python packages

	```bash
	pip install -r requirements.txt
	```
	
3. Launch Jupyter Notebook

	```bash 
	jupyter notebook
	```

---
## Acknowledgments
We thank the **organizing committee of the Frontiers in Neurophotonics Summer School 2025** for the opportunity to present this hands-on session.

We are especially grateful to **Paul De Koninck** and PhD candidate **Antoine Légaré** for generously sharing the experimental data used in this tutorial.

---

## Authors

Patrick Desrosiers and Nicolas Doyon at CERVO Brain Research Center