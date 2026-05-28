# Data

This folder contains the input files required by `notebooks/subjective_bayesian_network_notebook.ipynb`.

## Files

```text
breast_treat_qol_likert.bif
```

Input Bayesian network for the breast-cancer running example. The network contains clinical variables, treatment variables, temporal QoL variables, and virtual evidence nodes.

```text
cpt_likert_csv.csv
```

SOAP-derived evidence table used for MAP-EM learning. The entries encode manually constructed evidence from the SOAP summaries, including virtual evidence values where verbal QoL statements have been translated into model-compatible form.

## Notes

Column names in the CSV must correspond to node names in the Bayesian network. Observed values must correspond to valid state labels for those nodes. Missing values are treated as unobserved variables during learning.
