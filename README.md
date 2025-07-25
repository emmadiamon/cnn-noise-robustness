# Noise-Robust Image Classification with CNNs

This project investigates the robustness of Convolutional Neural Networks (CNNs), specifically VGG16 and ResNet50, for image classification under Gaussian noise using the Rice Image Dataset. It includes baseline models, noise injection, and enhancements through a custom U-Net denoising autoencoder and noise-aware training.

## Project Overview

- Fine-tuned VGG16 and ResNet50 using transfer learning on clean and noise-augmented images
- Implemented Gaussian noise injection at varying levels to evaluate model degradation
- Built and trained a U-Net autoencoder to denoise corrupted images prior to classification
- Improved classification accuracy and generalization under noisy conditions

## Techniques Used

- Transfer learning (VGG16, ResNet50)
- Data preprocessing and augmentation
- Gaussian noise modeling
- Denoising autoencoder (U-Net architecture)
- Model evaluation with confusion matrices and performance plots

## Project Structure
├── CV_Project_Implementation.ipynb # Baseline training and noise evaluation
├── Modification_of_CV_Project.ipynb # Denoising autoencoder and enhanced training
├── figures/ # Visualizations (e.g., accuracy/loss plots, confusion matrices)
└── README.md
## Dataset

- [Rice Image Dataset](https://www.kaggle.com/datasets/rashikrahmanpritom/rice-image-dataset)
- 75,000 high-resolution images across five rice varieties
- 2,000-image subset used for training and evaluation due to compute limitations

## Results

- VGG16 showed stronger robustness to noise than ResNet50 across all tested standard deviations
- Denoising and data augmentation significantly improved accuracy and reduced validation loss
- Demonstrated performance resilience on noisy inputs using a combined training strategy

## Contributors

- Emma Diamon – Data preprocessing, visualization, VGG16 training, autoencoder, evaluation, documentation
- Nishitha Tanukunuri – ResNet50 training, batch testing, metrics analysis, documentation
