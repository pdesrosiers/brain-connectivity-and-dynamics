# Graph and Dynamical Systems Approaches to Whole-Brain Neuronal Networks

This repository contains interactive Jupyter notebooks prepared for a hands-on session held as part of the **Frontiers in Neurophotonics Summer School 2026**.

---
## Overview

Modern network science and computational modeling offer powerful tools to analyze brain connectivity and neuronal dynamics. In this hands-on session, you will explore how to represent structural and functional brain networks as graphs, extract meaningful features, and simulate activity using biologically inspired models.

---
## Notebooks

### 1. Structural and Functional Network Analysis

The first hands-on session is divided into two comprehensive parts:

#### Session 1: Calcium Imaging Signal Extraction & Spatial Network Constraints

This notebook focuses on the essential upstream data-engineering steps required to transform raw whole-brain optical recordings into pristine functional trace matrices.

- **Interactive Spatial Masking:** Developing custom HTML5 canvas envelopes to isolate valid parenchymal brain tissue from peripheral agarose and ring artifacts.
- **Cell Segmentation:** Extracting unique cellular centroids across the larval zebrafish brain using spatial Gaussian filtering and local neighborhood maximum features.
- **Geometric Constraint Testing:** Evaluating how physical space limits network coupling by fitting distance-binned absolute correlations ($|R|$) to a truncated non-linear exponential decay model ($|R(d)| \propto e^{-d/\lambda}$) to extract the circuit's characteristic length ($\lambda$).

📁 [`functional_data_tutorial_2026.ipynb`](https://github.com/pdesrosiers/brain-connectivity-and-dynamics/blob/main/notebooks/functional_data_tutorial_2026.ipynb)
  
<a target="_blank" href="https://colab.research.google.com/github/pdesrosiers/brain-connectivity-and-dynamics/blob/main/notebooks/functional_data_tutorial_2026.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

#### Part 2: Graph Theory and Zebrafish Brain Network

This notebook transitions into network neuroscience, exploring how structural parameters shape collective functional networks and behavioral outputs.

- **Functional Network Inference:** Constructing whole-brain functional connectivity (FC) matrices via pairwise Pearson correlations and using row-wise Z-score scaling and symmetrical hierarchical clustering to reveal synchronized neural assemblies.
- **Graph-Theoretical Characterization:** Mapping the functional and structural brain graphs to calculate core topological features such as degree, strength, clustering coefficients, path lengths, and centrality metrics.
-**Structure–Function Coupling:** Quantifying the alignment between anatomical wiring (SC) and statistical dependencies (FC) using matrix correlation and node-level metrics.

📁 [`structural_functional_connectivity_tutorial_2026.ipynb`](https://github.com/pdesrosiers/brain-connectivity-and-dynamics/blob/main/notebooks/structural_functional_connectivity_tutorial_2026.ipynb)
  
<a target="_blank" href="https://colab.research.google.com/github/pdesrosiers/brain-connectivity-and-dynamics/blob/main/notebooks/structural_functional_connectivity_tutorial_2026.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>


### Session 2: Neural Dynamics and Circuit Simulation

This notebook transitions from static data processing to mechanistic computational modeling, focusing on how network connectivity rules shape population dynamics and drive behavior.

- **Spiking Networks & Fluorescence Convolutions:** Simulating fundamental single-neuron dynamics, generating random networks of spiking Leaky Integrate-and-Fire (LIF) units, and modeling the resulting calcium fluorescence response through mathematical convolutions (Deneux et al. 2016).
- **Hindbrain Circuit Motif Interrogation:** Replicating and analyzing the sensory-processing and decision-making model from Koyama et al. (2016) to study how manipulating connectivity parameters alters two-alternative behavioral choices.
- **Brain-Wide Sensorimotor Modeling:** Implementing the population-level neural mass model from Haesemeyer et al. (2018) to simulate heat-evoked swimming behaviors, track firing rates across different cell populations, and evaluate how structural changes modify motor output.

📁  [`ModelsOfNeuralActivityNeurohotonics2026.ipynb`](https://github.com/pdesrosiers/brain-connectivity-and-dynamics/blob/main/notebooks/ModelsOfNeuralActivityNeurohotonics2026.ipynb)
 
<a target="_blank" href="https://colab.research.google.com/github/pdesrosiers/brain-connectivity-and-dynamics/blob/main/notebooks/ModelsOfNeuralActivityNeurohotonics2026.ipynb">  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>


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

💾 To save your changes, go to

```File → Save a copy in Drive```

This creates a private, editable version of the notebook in your own Google Drive.

### 🖥️ Run Locally (Optional – for advanced users)

If you prefer to run the notebooks on your own machine:

1. Clone the repository 

	```bash
   git clone https://github.com/pdesrosiers/brain-connectivity-and-dynamics
   cd brain-connectivity-and-dynamics
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
