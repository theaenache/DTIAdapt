# DTIAdapt

Affiliated with Sekeh Lab at San Diego State University

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](#license)
[![Python Version](https://img.shields.io/badge/python-3.8%2B-blue.svg)](#requirements)

## Overview

DTIAdapt is a domain-adaptive Drug–Target Interaction (DTI) prediction framework based on the Triple-Branch Cross-Attention Transformer (CAT) architecture. It integrates the cross-attention mechanism from the CDTrans paper [1] with domain adaptation strategies to improve transfer learning between source and target datasets.

## Features

- **Triple-Branch CAT Architecture**: Learns joint representations of drugs and proteins.
- **Cross-Attention Module**: Implements cross-attention layers to model interactions across domains.
- **Domain Adaptation**: Employs adversarial and discrepancy-based losses to align feature distributions.
- **Evaluation of Transfer Gains**: Measures performance improvement when transferring from source to target domains.

## Repository Structure

```bash
DTIAdapt/
├── datasets/              ← raw & preprocessed data
│   ├── human/
│   ├── biosnap/           
│   └── bindingdb/           
├── notebooks/             ← Jupyter notebooks
│   ├── 01_data_prep.ipynb
│   ├── 02_model_def.ipynb
│   ├── 03_training.ipynb
│   └── 04_evaluation.ipynb
├── models/                ← saved checkpoints
├── scripts/               ← standalone .py scripts (optional)
├── results/               ← plots, metrics CSVs
├── README.md
└── requirements.txt


