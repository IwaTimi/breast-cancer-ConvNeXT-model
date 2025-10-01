# 🧬 Breast Cancer Classification using ConvNeXt + SE Attention

This project applies **ConvNeXt with Squeeze-and-Excitation (SE) attention mechanisms** to classify breast cancer from histopathology images (BreakHis dataset).  
It achieves **~99% accuracy** with explainable AI through Grad-CAM heatmaps.

---

## 📂 Project Structure
- `notebooks/` → Training & evaluation Jupyter notebooks
- `models/` → Saved `.pth` model weights
- `outputs/` → Results (confusion matrix, accuracy/loss plot, Grad-CAM maps)
- `requirements.txt` → Python dependencies

---

## 🚀 Methodology
1. **Data Preprocessing** → Resize, Normalize, Train/Val/Test split  
2. **ConvNeXt Backbone** → Pre-trained on ImageNet  
3. **SE Attention Integration** → Feature recalibration for better focus  
4. **Training** → Adam optimizer, LR scheduler  
5. **Evaluation** → Accuracy, Precision, Recall, F1-score  
6. **Explainability** → Grad-CAM heatmaps  

---

## 📊 Results
- **Accuracy:** ~99%  
- **Precision:** 0.99  
- **Recall:** 0.99  
- **F1-score:** 0.99  

### Confusion Matrix
![Confusion Matrix](outputs/confusion_matrix.png)

### Accuracy & Loss Curve
![Accuracy Loss](outputs/accuracy_loss_plot.png)

### Grad-CAM Heatmaps
![Grad-CAM](outputs/gradcam_heatmap_sample1.png)

---

## 📘 Dataset
The project uses the [BreakHis dataset](https://www.kaggle.com/datasets/ambarish/breakhis).  
Due to size, the dataset is **not included** in this repository.

---

## ⚡ How to Run
Clone the repo and install dependencies:

```bash
git clone https://github.com/<your-username>/BreastCancer-ConvNeXt-SE.git
cd BreastCancer-ConvNeXt-SE
pip install -r requirements.txt
