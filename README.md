# KAN_UNet-BrainTumor-Segmentation

This notebook implements a Kolmogorov–Arnold Network (KAN)-enhanced U-Net architecture for brain tumor segmentation using 3D MRI data.


Key Components:
Environment Setup: Installs required libraries like MONAI, NiBabel, and Weights & Biases (W&B).

Data Preparation:

Loads NIfTI files (e.g., BraTS dataset).

Applies preprocessing such as spacing normalization, orientation alignment, intensity scaling, and conversion to PyTorch tensors.

Model Definition:

Builds a 3D U-Net for segmentation.

Integrates a SimpleKAN block to enhance feature representation in deeper layers.

Training Loop:

Uses Dice Loss to train the model.

Optimizes using the Adam optimizer across multiple epochs.

Evaluation:

Computes Dice coefficient and Hausdorff Distance (HD95) to evaluate segmentation quality.

W&B Integration:

Logs quantitative metrics to Weights & Biases for experiment tracking and visualization.

This notebook provides a full deep learning pipeline from scratch to performance evaluation for KAN-enhanced U-Net models in medical image segmentation.
