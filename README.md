# Hybrid Quantum-Classical EfficientNet-DVQC for Bone Fracture Classification
# Ablation Study Results

This folder contains the experimental results of the ablation study for the proposed hybrid EfficientNet-B0–DVQC framework for bone fracture classification from X-ray images.

## Purpose

The ablation study evaluates the contribution of the quantum output head by comparing the proposed DVQC-based configurations with classical alternatives using the same EfficientNet-B0 feature-extraction backbone.

## Configurations Evaluated

The following configurations were evaluated:

1. EfficientNet-B0 Baseline
2. EfficientNet-B0 + 4D Classical Head
3. EfficientNet-B0 + Nonlinear Classical MLP
4. EfficientNet-B0 + 8D Classical Head
5. EfficientNet-B0 + DVQC (8 qubits)
6. EfficientNet-B0 + 16D Classical Head
7. EfficientNet-B0 + DVQC (Final)

All results are reported as mean ± standard deviation over five independent random seeds.

## Evaluation Metrics

The following test-set metrics are reported:

* Accuracy
* Sensitivity
* Specificity
* Precision
* F1-Score
* ROC-AUC

## Key Result

The final EfficientNet-B0 + DVQC configuration achieved a mean test accuracy of 98.66 ± 0.84%, sensitivity of 98.66 ± 1.39%, specificity of 98.66 ± 0.75%, precision of 98.81 ± 0.67%, F1-score of 98.73 ± 0.81%, and ROC-AUC of 0.9949 ± 0.0039 across five seeds.

These results are used to analyze the effect of replacing the classical output head with a variational quantum circuit and to assess the contribution of the quantum component within the proposed hybrid architecture.

## Reproducibility

The repository contains the corresponding experimental outputs and code used to generate the reported ablation results. The experiments use fixed random seeds to enable reproducible comparison between configurations.
