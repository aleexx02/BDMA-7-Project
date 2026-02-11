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
```text
.
├── BDMA7_project_files/
│   ├── train_images/              # Training images (one folder per class)
│   ├── val_images/                # Validation images (one folder per class)
│   └── test_images/
│       └── mistery_cat/           # Unlabeled test images
│
├── ConvNext_3Heads_Layers.ipynb   # Model 1: ConvNeXt-Small with 3 classifier heads
├── ConvNext_3Layers/              # Model 2: ConvNeXt-Small with 1 head (fixed 3-layer architecture)
├── ConvNext_Layers/               # Model 3: ConvNeXt-Small with 1 head (1–3 trainable layers)
├── README.md                      # Project documentation
├── Report.pdf                     # Project report
└── sample_submission.csv          # Example CSV submission file
```


## Setup

Clone this repository
```bash
git clone https://github.com/aleexx02/BDMA-7-Project.git
cd BDMA-7-Project
```
