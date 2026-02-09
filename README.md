# BDMA 7 Project: Image Classification Kaggle Competition
A deep learning project focused on fine‑grained bird species classification using a 20‑class subset of the Caltech‑UCSD Birds‑200‑2011 dataset.
The project explores three ConvNeXt-Small–based models, combined with transfer learning, data augmentation, stratified cross‑validation, and test‑time augmentation (TTA) to achieve strong accuracy on a small dataset.

## Features
**ConvNext-Small Backbone**: Modern CNN architecture inspired by Vision Transformers.
**Stratified 8‑Fold Cross‑Validation**: Reliable evaluation on a small dataset.
**Data Augmentation**: Color jitter, flips, rotations, and more.
**Test-Time Augmentation (TTA)**: Improves prediction reliability.
**Ensemble Option**: Combine predictions across folds for improved accuracy.

## Results (summary)
Across the 8‑fold evaluation and three tested models:
- Overall validation accuracy range: ~91.6% – 92.3%
- Performance differences are small but correlate with classifier head complexity.
- All ConvNeXt‑based models outperform the ResNet‑50 baseline, confirming the benefits of the modernized architecture.

## Project Structure
.
├── BDMA7_project_files/         # Folder with dataset
    ├── train_images/            # Training images per class (one class = one folder)
│   ├── val_images/              # Validation images per class (one class = one folder)
│   ├── test_images/                          
        |── mistery_cat/         # Test images
│  
├── ConvNext_3Heads_Layers.ipynb/         # Model 1: ConvNext-Small with 3 classifier heads.
├── ConvNext_3Layers/                     # Model 2 ConvNext-Small with 1 head (fixed 3-layer architecture).
├── ConvNext_Layers/                      # Model 3 ConvNext-Small with 1 head (1, 2, or 3 trainable layers).
├── README.md                             # Project documentation (this file)
└── sample_submission.csv                 # Example .csv submission file


## Setup
1. Clone this repository
```bash
git clone https://github.com/aleexx02/BDMA-7-Project.git`
`cd BDMA-7-Project
```
