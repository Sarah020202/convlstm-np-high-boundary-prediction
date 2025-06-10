# ConvLSTM-Based Prediction of the North Pacific High Boundary

This repository contains deep learning models to predict the 5880gpm contour of the North Pacific High using ERA5 reanalysis data. The models focus on capturing spatiotemporal dynamics using ConvLSTM, Conv3D, and UNet-GRU architectures.

## 📁 Structure
notebooks/
├── ConvLSTM_all_features+feature_important.ipynb
├── ConvLSTM_only_z.ipynb
├── ConvLSTM_5var_unadjusted.ipynb
├── ConvLSTM_5var_adjusted.ipynb
├── Conv3D_5var_unadjusted.ipynb
└── UNet-GRU_5var_unadjusted.ipynb


## 🧪 Models
- **ConvLSTM**: with full features, z-only, and 5 variable (before/after adjustment)
- **Conv3D**: spatiotemporal convolution baseline
- **UNet-GRU**: hybrid architecture for sequence prediction

## 🔧 To Do
- [ ] Upload `results/` with prediction maps
- [ ] Add sample `.npy` data (under 100MB)
- [ ] Add `.gitignore` and `requirements.txt`

