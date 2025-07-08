# 🧠 ResUNet++ for Breast Tumor Segmentation (BUS-UC Dataset)

This project implements the **ResUNet++** architecture for breast tumor segmentation using the **BUS-UC Breast Ultrasound Dataset**. The work was carried out under the research guidance of **Prof. Ram Sarkar**, Jadavpur University, as part of a research internship evaluation.

---

## 📂 Dataset
- **Source**: [Kaggle - BUS-UC](https://www.kaggle.com/datasets/orvile/bus-uc-breast-ultrasound)
- **Classes**: Benign and Malignant
- **Annotations**: Binary tumor segmentation masks
- **Preprocessing**:
  - Grayscale image conversion
  - Resized to **128×128**
  - Normalized to [0, 1]

---

## 🧱 Model: ResUNet++

An enhanced U-Net that integrates:
- ✅ Residual Blocks
- ✅ ASPP (Atrous Spatial Pyramid Pooling)
- ✅ Squeeze-and-Excitation (SE) Modules

---

## 📊 Training Configuration

- **Epochs**: 30  
- **Batch Size**: 4  
- **Optimizer**: Adam  
- **Loss**: Binary Crossentropy  
- **Validation Split**: 15%  
- **Train/Val/Test Ratio**: 70/15/15  

---

## 📈 Results

| Metric            | Value         |
|-------------------|---------------|
| Training Accuracy | 98.92%        |
| Validation Acc.   | 97.21%        |
| Test Accuracy     | **97.86%**    |
| Test Loss         | 0.0670        |

---

## 📘 Comparison with DAU-Net Paper

| Metric          | ResUNet++ (Ours) | DAU-Net Paper (ResUNet++) |
|-----------------|------------------|----------------------------|
| Test Accuracy   | **97.86%**       | ~**96.5%**                 |
| Visual Results  | Sharp boundaries | Moderate smoothness        |
| Model Params    | 6M+              | Similar                    |

> ✅ Our model shows improved accuracy while retaining architectural depth, confirming reproducibility and robustness.

---


