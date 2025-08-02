# SegmentationModelComparison

This repository contains experiments and comparisons of deep learning models for medical image segmentation, specifically using a knee phantom dataset. The primary goal is to analyze how different architectures perform on the same dataset, focusing on accuracy, robustness, and feature extraction.

## 📌 Models Implemented

### U-Net (Unet.ipynb)
A popular encoder–decoder CNN architecture designed for biomedical image segmentation.

### U-Net++ (Nested U-Net) (unetpp.ipynb)
An improved version of U-Net with nested and dense skip connections for better feature fusion.

### SegFormer (Segformer.ipynb)
A transformer-based segmentation model that leverages attention mechanisms for high-quality segmentation with fewer parameters.

## 📂 Project Structure

```
SegmentationModelComparison/
│
├── Segformer.ipynb     # Notebook with SegFormer implementation & training
├── Unet.ipynb          # Notebook with U-Net implementation & training
├── unetpp.ipynb        # Notebook with U-Net++ implementation & training
├── requirements.txt    # Python dependencies
└── README.md           # Project documentation
```

## ⚙️ Requirements

Make sure you have the following installed:

- Python 3.8+
- Jupyter Notebook / Jupyter Lab
- PyTorch (preferred) or TensorFlow
- OpenCV
- NumPy
- Matplotlib
- scikit-learn
- Albumentations (for data augmentation)

Install dependencies:
```bash
pip install -r requirements.txt
```

## 📊 Dataset

- **Dataset Used:** Knee dataset obtained from medical phantoms (synthetic anatomical models)
- **Format:** Typically grayscale medical images with segmentation masks
- **Task:** Segment knee joint regions to evaluate structural boundaries

👉 **Note:** Update dataset paths inside each notebook before running.

## 🚀 Usage

1. **Clone the repository:**
   ```bash
   git clone https://github.com//SegmentationModelComparison.git
   cd SegmentationModelComparison
   ```

2. **Launch Jupyter Notebook/Lab:**
   ```bash
   jupyter lab
   ```

3. **Open and run any of the model notebooks:**
   - `Unet.ipynb` → Train/evaluate U-Net
   - `unetpp.ipynb` → Train/evaluate U-Net++
   - `Segformer.ipynb` → Train/evaluate SegFormer

## 📈 Evaluation Metrics

Each model is evaluated using:

- **Dice Coefficient** (F1 Score for segmentation)
- **IoU** (Intersection over Union)
- **Pixel-wise Accuracy**

These metrics help compare segmentation quality across models.

## 📊 Results & Comparison

- **U-Net:** Strong baseline, fast training, effective for medical images
- **U-Net++:** Improved boundary precision, better feature reuse
- **SegFormer:** Transformer backbone shows robustness but may need more data for optimal performance


## 🔮 Future Work

- Add DeepLabV3+ and Mask R-CNN for further comparison
- Extend to real patient MRI datasets for validation beyond phantoms

## 🤝 Contributing

✨ Contributions and suggestions are welcome!
## Medium article:
https://medium.com/@workwithpoojasri/from-u-net-to-segformer-segmenting-spinal-structures-with-precision-af433be5f3ba
