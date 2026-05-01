# 🩸 HemoClass — Blood Cell Image Classification

MATLAB project for classifying leukocyte images (healthy vs pathological) using matrix decomposition and neural-network approaches.

Developed for the **Advanced Numerical Methods** course.

## 👥 Team

- Antonio Spedito
- Gaia Montalbano
- Alessandro Picone

## 🧪 Methodology

- Image preprocessing (grayscale conversion, resizing, cleanup)
- Matrix compression / decomposition:
  - QR
  - SVD
- Classification with:
  - custom neural network
  - MATLAB neural-network workflow

## ▶️ Suggested execution flow

```matlab
run preprocc.m
run func_ourQR.m
run func_ourSVD.m
run nn_manual.m
run nn_matlab.m
```

## 📌 Notes

- SVD was more effective than QR for preserving discriminative information in this task
- Full project details are available in:
  - `Classificazione_Immagini_Sangue.pdf`

## 📄 License

See `LICENSE`.

