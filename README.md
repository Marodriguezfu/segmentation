# Image Segmentation Lab

This repository contains practical exercises on **image segmentation**, developed as part of the course *IMA201 – Image Processing*.  
It covers edge detection, classification-based segmentation, thresholding (Otsu), and region growing methods.

---

## 📖 Project Overview

The lab introduces and compares different **segmentation techniques** in digital image processing.  
The exercises are implemented in Python and explore how each method performs under various conditions such as noise, image type, and parameter choices.

---

## 🛠️ Topics Covered

1. **Edge Detection**
   - Gradient filters (Sobel vs. simple difference).
   - Thresholding gradient magnitude for contour extraction.
   - Zero-crossing of the Laplacian.
   - Analysis of noise robustness, continuity, and contour accuracy.

2. **Segmentation by Classification (K-means)**
   - Gray-level image segmentation (e.g., `cell.tif`, `muscle.tif`).
   - Color image segmentation (`fleur.tif`) with different numbers of clusters.
   - Effect of initialization, stability of results, and pre/post-filtering.

3. **Automatic Thresholding (Otsu Method)**
   - Minimizing intra-class variance to determine thresholds.
   - Application to binary and multi-class problems.
   - Extension to three-class segmentation.

4. **Region Growing**
   - Segmentation based on local statistics (mean, variance).
   - Application to brain images (`cerveau.tif`) for white and gray matter detection.
   - Effect of threshold and neighborhood radius parameters.

---

## ⚙️ Requirements

- **Python 3.x**
- **NumPy**
- **Matplotlib**
- (Optional) Spyder IDE with Anaconda

Install dependencies with:

```bash
pip install numpy matplotlib
```

##  🚀 How to Run

1. Clone or download the repository.

2. Place the provided images in the images/ folder.

3. Run the scripts step by step.

4. Adjust parameters (thresholds, number of clusters, seed point) to observe different segmentation results.

## 📊 Results

- Edge detection methods differ in robustness to noise and contour accuracy.

- K-means classification benefits from image filtering for better segmentation.

- Otsu’s method provides an automated threshold but may fail on gradient images.

- Region growing enables tissue segmentation (white/gray matter) but is sensitive to parameters.