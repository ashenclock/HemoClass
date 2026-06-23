<div align="center">

# 🩸 HemoClass

**Blood Cell Image Classification using Matrix Decomposition & Neural Networks**

[![MATLAB](https://img.shields.io/badge/MATLAB-R2023a-orange.svg)](https://www.mathworks.com/products/matlab.html)
[![License: GPL-3.0](https://img.shields.io/badge/License-GPL--3.0-blue.svg)](LICENSE)

*Advanced Numerical Methods — University of Palermo*

</div>

---

## 📋 Overview

HemoClass is a MATLAB-based pipeline for classifying leukocyte (white blood cell) microscopy images as **healthy** or **pathological (cancerous)**. The project explores how different matrix decomposition techniques affect the quality of image compression and downstream classification accuracy.

## 🧪 Methodology

The pipeline follows a structured approach:

| Stage | Description | File |
|-------|-------------|------|
| **Preprocessing** | Grayscale conversion, resizing, noise removal | `preprocc.m` |
| **Image Loading** | Batch import of microscopy images | `func_imread.m` |
| **QR Decomposition** | Compress images via QR factorization | `func_ourQR.m` |
| **SVD Decomposition** | Compress images via Singular Value Decomposition | `func_ourSVD.m` |
| **Neural Network (Custom)** | Manually implemented feedforward NN | `nn_manual.m` |
| **Neural Network (MATLAB)** | Classification using MATLAB's NN Toolbox | `nn_matlab.m` |

### Key Finding
> SVD proved significantly more effective than QR for preserving discriminative features in compressed blood cell images, leading to higher classification accuracy.

## 🚀 Quick Start

```matlab
% 1. Prepare the image dataset
run('PreparazioneImmagini.m')

% 2. Preprocess images
run('preprocc.m')

% 3. Apply matrix decomposition
run('func_ourQR.m')   % QR approach
run('func_ourSVD.m')  % SVD approach

% 4. Train and evaluate classifiers
run('nn_manual.m')    % Custom neural network
run('nn_matlab.m')    % MATLAB toolbox neural network
```

## 👥 Authors

- **Antonio Spedito** — [@ashenclock](https://github.com/ashenclock)
- **Gaia Montalbano**
- **Alessandro Picone**

## 📄 Documentation

The full project report is available at [`Classificazione_Immagini_Sangue.pdf`](Classificazione_Immagini_Sangue.pdf).

## 📜 License

This project is licensed under the GPL-3.0 License — see the [LICENSE](LICENSE) file for details.
