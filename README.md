# adaptive-xai-credit

**The Message That Didn't Land: Adaptive XAI for Indonesian Digital Finance Users**

---

## What this is

This repository contains the technical pipeline for my MSc HCI thesis. The thesis investigates whether literacy-adaptive XAI explanations improve decision confidence for Indonesian digital finance users compared to standard one-size-fits-all explanations.

The pipeline is a means to an end -- the contribution is the adaptive explanation layer (Step 8), not the model itself.

---

## Pipeline overview
* Step 1: Get the data (Home Credit Default Risk, Kaggle)
* Step 2: Inspect + clean
* Step 3: Split (80/20, stratified)
* Step 4: Configure XGBoost
* Step 5: Train
* Step 6: Evaluate (ROC-AUC)
* Step 7: Apply TreeSHAP
* Step 8: Build literacy-adaptive explanation templates

## How to run

1. Open `notebooks/home-credit.ipynb` in Google Colab
2. Run all cells in order
3. Dataset downloads automatically via kagglehub (Kaggle account required)

## Repo structure
```
adaptive-xai-credit/
├── notebooks/        ← Colab notebook
├── docs/             ← pipeline guide, navigation reference, thesis notes
├── data/             ← empty; see data/README.md for download instructions
├── templates/        ← literacy-adaptive explanation templates (Step 8)
└── README.md
```

## Status

- [x] Step 1: Data
- [x] Step 2: Clean
- [x] Step 3: Split
- [x] Step 4: Configure
- [x] Step 5: Train
- [x] Step 6: Evaluate (ROC-AUC: 0.7515)
- [ ] Step 7: TreeSHAP
- [ ] Step 8: Explanation templates
