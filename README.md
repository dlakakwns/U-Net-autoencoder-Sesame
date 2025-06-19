## Overview
Hyperspectral imaging (HSI) integrates spectroscopy and imaging, providing detailed spectral-spatial information, and the selection of task-relevant wavelengths can streamline data acquisition and processing for field deployment. Anomaly detection aims to identify observations that deviate from normal patterns, typically in a one-class classification framework. In this study, we extend this framework to binary classification by employing a U-Net based deterministic autoencoder augmented with attention blocks to analyze HSI data of sesame plants inoculated with Pseudomonas syringae pv. sesami. Single-band grayscale images across the full spectral range were used to train the model on healthy samples, while the presence of disease was classified by assessing the reconstruction error, which we refer to as the anomaly score. The average classification accuracy in the visible region spectrum (430–689 nm) exceeded 80%, with peaks at 641 nm and 689 nm. In comparison, the near-infrared region (> 700 nm) attained an accuracy of approximately 60%. Several visible bands demonstrated potential for early disease detection. Some lesion samples showed a gradual increase in anomaly scores over time, and notably, Band 23 (689 nm) exhibited exceeded anomaly scores even at early stages before visible symptoms appeared. This supports the potential of this wavelength for the early stage detection of bacterial leaf spot in sesame.

## Data
The original contributions presented in this study are included in the article. Further inquiries can be directed to the corresponding authors.

## Python Versions 
### For ROI
opencv-python             4.10.0.82

spectral                  0.23.1

### For Modeling
pandas: 2.2.2

numpy: 1.26.4

torch: 2.6.0

cv2: 4.10.0

tqdm: 4.66.4

torch.nn: 2.6.0

torch.nn.functional: 2.6.0

torch.optim: 2.6.0

torch.optim.AdamW: 2.6.0

torch.utils.data: 2.6.0

PIL: 10.3.0

torchvision: 0.21.0

matplotlib: 3.8.4

plotly: 5.22.0

optuna: 4.1.0

sklearn: 1.4.2

## Files Describtion
- Classification : Main Code file
- Result_txt : Hyperparameters and results from the best trial.
- Best_model : Model files from the best trial.
