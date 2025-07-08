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

## 📘 Comparison with DAU-Net Paper

| **Metric**         | **ResUNet++ (Ours – BUS-UC)** | **ResUNet++ (Paper – BUSI)** |
|--------------------|-------------------------------|-------------------------------|
| **Test Accuracy**  | 97.86%                        | Not Reported                 |
| **Dice Score (F1)**| 92.29%                        | 73.85%                        |
| **Precision**      | 91.68%                        | 80.10%                        |
| **Recall**         | 92.91%                        | 71.43%                        |
| **IoU (Jaccard)**  | 85.68%                        | 60.02%                        |
| **Test Loss**      | 0.0670                        | Not Reported                 |

📌 **Note**: This comparison is **cross-dataset** — our model was trained and evaluated on the **BUS-UC** dataset, while the paper reports results on the **BUSI** dataset. Thus, the comparison reflects architectural and training strengths but does **not imply absolute superiority** without same-dataset evaluation.

> ✅ Our model shows improved accuracy while retaining architectural depth, confirming reproducibility and robustness.

---


