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



Each notebook corresponds to a different model or input feature combination.  
The focus is on predicting the 5880gpm geopotential height line, which approximates the boundary of the North Pacific High.

## 🧪 Models

- **ConvLSTM**:  
  - `ConvLSTM_all_features+feature_important.ipynb`  
  - `ConvLSTM_only_z.ipynb`  
  - `ConvLSTM_5var_unadjusted.ipynb`  
  - `ConvLSTM_5var_adjusted.ipynb`
- **Conv3D**:  
  - `Conv3D_5var_unadjusted.ipynb`
- **UNet-GRU**:  
  - `UNet-GRU_5var_unadjusted.ipynb`

## 📂 Dataset Access

Due to file size limitations on GitHub, the full dataset is hosted on Google Drive:

🔗 [Download the dataset from Google Drive](https://drive.google.com/drive/u/0/folders/10oi15WS6di_tycivWf58LBTeFuGfWwdW)

### Download includes:

data/
├── data_stream-oper_stepType-instant.nc

├── X_full_z.npy

├── y_full_z.npy

├── valid_times_full_z.npy

├── X_full_(z,t,u,v,q).npy

├── y_full_(z,t,u,v,q).npy

├── valid_times__full_(z,t,u,v,q).npy

├── X_part1.npy ~ X_part4.npy

├── y_part1.npy ~ y_part4.npy

└── valid_times_part1.npy ~ valid_times_part4.npy


These files contain ERA5-derived geopotential height fields and multivariate predictors over East Asia, sampled from 2022 to 2024 (May–October, 6-hourly intervals).

## 🔧 To Do

- [ ] Upload `results/` with prediction maps and evaluation metrics
- [ ] Add sample `.npy` data (under 100MB) for minimal testing
- [ ] Add `.gitignore` and `requirements.txt` for reproducibility

---

Feel free to fork or clone this repository and experiment with different model architectures and input features.

