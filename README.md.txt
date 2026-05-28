# QoL Bayesian Network EM

This repository contains the code and data used for the paper 'Subjective and temporal quality-of-life information in Bayesian Networks' by Kwisthout & Kimpel with subjective, ordered, and temporal quality-of-life information.

The notebook runs the MAP-EM learning procedure, learns an updated Bayesian network from SOAP-derived virtual evidence, and performs exact inference for temporal QoL statement queries under treatment settings. It also generates the tables and figures.

## Repository structure

```text
data/
  breast_treat_qol_likert.bif
  cpt_likert_csv.csv
  README.md

notebooks/
  reproduce_manuscript.ipynb

outputs/
  figures/
  learned_networks/
  learning/
  inference/
```

## Installation

The code was tested with Python 3.12.13. Install the required packages with:

```bash
pip install -r requirements.txt
```

The required package versions are listed in `requirements.txt`.

## Reproducing the paper's workflow

Run the notebook from top to bottom:

```text
notebooks/subjective_bayesian_network_notebook.ipynb
```

The notebook expects the following files to be present in `data/`:

```text
data/breast_treat_qol_likert.bif
data/cpt_likert_csv.csv
```

The notebook writes outputs to `outputs/`, including the learned Bayesian network, learning-related manuscript tables, exact-inference outputs, and generated figures.


## Notes

The data and network are constructed for methodological illustration. The learned probabilities should not be interpreted as clinically validated estimates.
