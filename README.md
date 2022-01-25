# Multiomics-BMI  

This repository includes the code used in our multiomics BMI study.  

> Preprint version:  
> **Multiomic investigations of Body Mass Index reveal heterogeneous trajectories in response to a lifestyle intervention.**  
> Kengo Watanabe, Tomasz Wilmanski, Christian Diener, Anat Zimmer, Briana Lincoln, Jennifer J. Hadlock, Jennifer C. Lovejoy, Sean Gibbons, Andrew T. Magis, Leroy Hood, Nathan D. Price, and Noa Rappaport.  
> *medRxiv*, DOI: https://doi.org/10.1101/2022.01.20.22269601  

Correspondence to Noa Rappaport (noa.rappaport@isbscience.org).  

## Code overview  
> The below figure numbers correspond to the current preprint version.  

### 1. 220121_Multiomics-BMI-paper_code-01_baseline-LASSO.ipynb  
This Jupyter Notebook generated the LASSO models predicting BMI from the baseline Arivale datasets.  
Output:  
* Figure 1a, 1b  
* Supplementary Figure 3  
* Intermediate tables for other notebook (BMI predictions, beta-coefficients)  

### 2. 220121_Multiomics-BMI-paper_code-02_LASSO-bcoef.ipynb  
This Jupyter Notebook visualized the variables of the omics-based BMI models and assessed them using BMI regression.  
Output:  
* Figure 2  
* Supplementary Figure 2  
* Supplementary Figure 4  
* Intermediate tables for other notebook (regression summary)  

### 3. 220121_Multiomics-BMI-paper_code-03_misclassification.ipynb  
This Jupyter Notebook assessed misclassification and further addressed the underlying molecular differences with hierarchical clustering.  
Output:  
* Figure 3a, 3b  
* Figure 3d, 3e  
* Supplementary Figure 5b, 5c  
* Intermediate table for other notebook (misclassification label)  

### 4. 220121_Multiomics-BMI-paper_code-04_OLS-regression_numeric-features.ipynb  
This Jupyter Notebook assessed baseline numeric features independently using baseline measured and omics-based BMIs regression. Also, each numeric feature was assessed in point of misclassification.  
Output:  
* Figure 1c  
* Figure 3c  

### 5. 220121_Multiomics-BMI-paper_code-05_OLS-regression_clinical-labs.ipynb  
This Jupyter Notebook assessed baseline clinical lab tests in point of misclassification.  
Output:  
* Supplementary Figure 5a  

### 6. 220121_Multiomics-BMI-paper_code-06_longitudinal-LASSO.ipynb  
This Jupyter Notebook generated the LASSO models predicting BMI from the time-series Arivale datasets.  
Output:  
* Intermediate tables for other notebook (BMI predictions)  

### 7. 220121_Multiomics-BMI-paper_code-07_longitudinal-LMM.ipynb  
This Jupyter Notebook assessed longitudinal changes of measured and omics-based BMIs using linear mixed model (LMM).  
Output:  
* Figure 5  

### 8. 220121_Multiomics-BMI-paper_code-08_longitudinal-network-analysis_all-omics.ipynb  
This Jupyter Notebook assessed (1) the baseline analyte–analyte interactions with baseline metabolomics-based BMI using generalized linear model (GLM) and (2) the siginificant analyte–analyte interactions with days in program using generalized estimating equations (GEE).  
Output:  
* Figure 6b, 6c  
* Intermediate table for other notebook (GLM/GEE summary)  

### 9. 220121_Multiomics-BMI-paper_code-09_network-analysis-visualization.ipynb  
This Jupyter Notebook visualized the network analyses of analyte interactions.  
Output:  
* Figure 6a  

### 10. xxx.ipynb  
> Not finished yet (Jan 24, 2022)  
> This Jupyter Notebook generated the random forest classifier...  

Output:  
* Figure 4  

## Requirements  
The following package/library versions were used and hence confirmed at least.  
* Python (version 3.7.6 or 3.9.6)  
* numpy (version 1.18.1 or 1.21.1)  
* pandas (version 1.0.3 or 1.3.1)  
* scipy (version 1.4.1 or 1.7.1)  
* matplotlib (version 3.2.1 or 3.4.2)  
* seaborn (version 0.10.1 or 0.11.1)  
* scikit-learn (version 0.22.1 or 0.24.2)  
* statsmodels (version 0.11.1 or 0.12.2)  
* R (version 4.0.3)  
* tidyverse (version 1.3.0)  
* circlize (version 0.4.11)  

## Log  
Last update on Jan 24, 2022  
* 2022-01-20 The repository was generated.  
* 2022-01-24 The Jupyter Notebooks (from 01 to 09) were uploaded.  
