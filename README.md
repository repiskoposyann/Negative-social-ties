# Bullying-Withdrawal Longitudinal Analysis

This repository contains a reproducible **observed-variable longitudinal path-analysis workflow** for a study on bullying victimization, social withdrawal, family support, and later internalizing symptoms.

## What this repository is

This repository provides a complete computational companion for a **summary-variable dataset** with 17 columns. The analysis estimates:

- longitudinal path models based on observed variables,
- mediation through social withdrawal,
- moderation by family support,
- bootstrap confidence intervals for indirect effects,
- a Wald-style comparison of cyberbullying and offline bullying effects on withdrawal,
- sensitivity models separating strong-tie and neutral-tie withdrawal,
- multicollinearity diagnostics,
- residual diagnostics,
- publication-ready tables and figures.

## What this repository is not

This repository **does not** reproduce a full item-level latent-variable SEM with:

- latent measurement models,
- longitudinal measurement invariance testing,
- latent moderated structural equations,
- global SEM fit indices such as CFI, TLI, or RMSEA.

The reason is straightforward: the available dataset is a **summary-level dataset**, not a raw item-level dataset.

## Repository structure

```
bullying-withdrawal-analysis/
├── data/
│   └── longitudinal_bullying_withdrawal_data.csv
├── output.data/
│   ├── tables/
│   ├── figures/
│   └── logs/
├── SRC/
│   └── run_observed_variable_analysis.py
├── README.md
├── requirements.txt

```

## Dataset structure

The dataset includes 17 variables:

- id
- age
- gender
- parent_edu
- low_income
- recruit_source
- offline_bullying_T1
- cyberbullying_T1
- family_support_T1
- strong_tie_withdrawal_T2
- neutral_tie_withdrawal_T2
- depression_T1
- anxiety_T1
- stress_T1
- depression_T3
- anxiety_T3
- stress_T3

## Installation

```
pip install -r requirements.txt
```

## Run

```
python src/run_observed_variable_analysis.py
```

## Outputs

Tables → `output/tables/`  
Figures → `output/figures/`  
Logs → `output/logs/`

## Citation

Reproducible observed-variable longitudinal path-analysis code and outputs for the bullying–withdrawal study.

## License

MIT License
