README
================
Patternverse
2025-11-25

# Olive Oil Authentication Using FTIR Spectroscopy  
**Chemometric Classification in R**

This project applies chemometric and machine learning techniques to classify olive oil samples based on their infrared spectra. It demonstrates how spectroscopy, data preprocessing, and supervised models can be combined to build an authenticity classifier.

---

## Project Goals

- Use mid-infrared (FTIR) spectral data to distinguish between different olive oil categories.
- Apply chemometric preprocessing (normalization, smoothing, derivatives, PCA).
- Train classification models (PLS-DA, Random Forest, SVM).
- Compare model performance and interpret results.
- Provide reproducible R code for scientific workflows.

---

## Dataset Description

This project uses the dataset **FTIR_Spectra_olive_oils.csv**, containing **120 mid-infrared spectra** collected from **60 authenticated extra virgin olive oils**.  
The samples were supplied to the **Institute of Food Research (UK)** by the **International Olive Oil Council**.

### Acquisition Details
- Spectra were obtained using **Attenuated Total Reflectance (ATR)** sampling.  
- Each sample was measured **twice**, producing duplicate spectra.  
- Acquisition order was **randomized** with respect to country of origin for both measurement sessions.  
- The dataset therefore includes **duplicate, independently acquired spectra** for all samples.

### Original Source & Citation

The dataset is described in:

> **Tapp H.S., Defernez M., Kemsley E.K.**  
> *FTIR spectroscopy and multivariate analysis can distinguish the geographic origin of extra virgin olive oils.*  
> Journal of Agricultural and Food Chemistry, **51(21)**, 6110–6115 (2003).

### Licensing & Data Sharing

The data are made available according to the **BBSRC policy on data sharing**.  
You are free to analyse and redistribute the dataset, provided you **acknowledge the original source** (via citation or link).

---

## 🔬 Methods Used

### **1. Data Preprocessing**
- Baseline correction  
- Normalization  
- Savitzky–Golay smoothing (optional)  
- Derivative spectra  
- PCA for exploratory analysis  

### **2. Exploratory Data Analysis**
- Plotting raw and processed spectra  
- PCA score/loading plots  
- Outlier inspection  

### **3. Model Training**
Models implemented:

- **PLS-DA** (Partial Least Squares Discriminant Analysis)  
- **SVM (Radial Basis Kernel)**  
- **Random Forest**

Cross-validation is used where applicable.

### **4. Model Evaluation**
- Accuracy  
- Confusion matrix  
- Sensitivity / specificity  
- Visual comparison of true vs. predicted classes  

---

## Example Visualizations

The project includes visual outputs such as:

- Raw FTIR spectra overlay  
- Preprocessed (smoothed / derivative) spectra  
- PCA score plots  
- Confusion matrices  
- Variable importance (Random Forest)

---

## Technologies Used

- **R**  
- tidyverse  
- caret or tidymodels  
- pls / mixOmics (PLS-DA)  
- e1071 (SVM)  
- randomForest  
- ggplot2 (visualization)  

---

## How to Run the Code

### **Option A — R Script**

