# brain-decoding-ica-pca

# 🧠 Brain Decoding with ICA vs PCA

This project compares **Independent Component Analysis (ICA)** and **Principal Component Analysis (PCA)** for decoding cognitive states from fMRI data using the Haxby dataset. We extract brain activation patterns, classify them with SVMs, and visualize the components as brain maps.

---

## 📚 Project Highlights

- 🎯 **Goal**: Classify cognitive states (e.g., face, house, cat, etc.) from brain activity
- 🧠 **Data**: [Haxby fMRI Dataset](https://nilearn.github.io/stable/auto_examples/02_decoding/plot_haxby_simple.html)
- 🧮 **Techniques**: PCA, ICA, SVM
- 🔬 **Tools**: Nilearn, Scikit-learn, Matplotlib, Seaborn
- 🧾 **Outputs**:
  - Classification accuracy
  - Brain component visualizations
  - Confusion matrices for ICA vs PCA

---

## 🧪 Methodology

1. **Preprocessing**: Extract time-series data from fMRI volumes using a ventral temporal mask
2. **Feature Extraction**:
   - PCA: Reduce to 100 principal components
   - ICA: Extract 100 independent components
3. **Classification**:
   - Linear SVM to predict stimulus categories
   - Evaluate and compare performance
4. **Visualization**:
   - Confusion matrix for both methods
   - Brain maps of top components (via `nilearn.plotting`)

---

## 📊 Results Snapshot

- PCA Accuracy: ~💯%
- ICA Accuracy: ~💯%
- Component maps show distinct spatial patterns per method

> ICA tends to find **more interpretable components**, while PCA excels at **capturing variance**.

---

## 🧰 Requirements

```bash
pip install nilearn nibabel scikit-learn matplotlib seaborn
