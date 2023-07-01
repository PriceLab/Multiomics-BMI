# Multiomics-BMI  

This repository includes the code used in our multiomics BMI study.  

**Multiomic signatures of body mass index identify heterogeneous health phenotypes and responses to a lifestyle intervention.**  
Kengo Watanabe, Tomasz Wilmanski, Christian Diener, John C. Earls, Anat Zimmer, Briana Lincoln, Jennifer J. Hadlock, Jennifer C. Lovejoy, Sean M. Gibbons, Andrew T. Magis, Leroy Hood, Nathan D. Price, and Noa Rappaport.  
*Nat. Med.* 29, 996–1008 (2023), DOI: https://doi.org/10.1038/s41591-023-02248-0
> Preprint version:  
> **Multiomic Body Mass Index signatures in blood reveal clinically relevant population heterogeneity and variable responses to a healthy lifestyle intervention.**  
> Kengo Watanabe, Tomasz Wilmanski, Christian Diener, John C. Earls, Anat Zimmer, Briana Lincoln, Jennifer J. Hadlock, Jennifer C. Lovejoy, Sean M. Gibbons, Andrew T. Magis, Leroy Hood, Nathan D. Price, and Noa Rappaport.  
> *medRxiv* 2022.01.20.22269601 (2022), DOI: https://doi.org/10.1101/2022.01.20.22269601  

Correspondence to Noa Rappaport (noa.rappaport@isbscience.org).  

## Code overview  
> The below figure numbers correspond to the latest preprint version, which are basically same with the paper version (i.e., please regard Supplementary Figure as Extended Data Figure).  

### 1. Code01_BMI-LASSO_Arivale-baseline.ipynb  
This Jupyter Notebook (with Python 3 kernel) generated the LASSO linear regression models for predicting BMI (biological BMI) from each of the Arivale baseline blood omic datasets, and calculated the testing (hold-out) set-derived BMI predictions for the Arivale cohort.  
Output figures and tables:  
* Figure 1b, 1c  
* Supplementary Figure 2d–h  
* Tables for Supplementary Data 1, 3, 10  
* Intermediate tables for other notebooks (BMI predictions)  

### 2. Code02_BMI-LASSO_Arivale-fitted_TwinsUK.ipynb  
This Jupyter Notebook (with Python 3 kernel) generated the LASSO linear regression models for predicting BMI (biological BMI) from the restricted Arivale metabolomics panel, and calculated BMI predictions for the TwinsUK cohort.  
Output figures and tables:  
* Figure 1d  
* Supplementary Figure 3  
* Tables for Supplementary Data 3, 10  
* Intermediate tables for other notebooks (BMI predictions)  

### 3. Code03_BMI-LASSO-bcoef.ipynb  
This Jupyter Notebook (with Python 3 kernel) visualized beta-coefficients of the blood omics-based BMI LASSO models, and assessed relationships between BMI and the retained variables using regression analysis (in the Arivale cohort).  
Output figures and tables:  
* Figure 2  
* Supplementary Figure 2a–c, 5  
* Tables for Supplementary Data 5  

### 4. Code04_BMI-ElasticNet_Arivale-baseline.ipynb  
This Jupyter Notebook (with Python 3 kernel) generated the elastic net linear regression models for predicting BMI (biological BMI) from each of the Arivale baseline blood omic datasets, and calculated the testing (hold-out) set-derived BMI predictions for the Arivale cohort.  
Output figures and tables:  
* Intermediate tables for other notebooks (BMI predictions, beta-coefficients)  

### 5. Code05_BMI-Ridge_Arivale-baseline.ipynb  
This Jupyter Notebook (with Python 3 kernel) generated the ridge linear regression models for predicting BMI (biological BMI) from each of the Arivale baseline blood omic datasets, and calculated the testing (hold-out) set-derived BMI predictions for the Arivale cohort.  
Output figures and tables:  
* Intermediate tables for other notebooks (BMI predictions, beta-coefficients)  

### 6. Code06_BMI-RandomForest_Arivale-baseline.ipynb  
This Jupyter Notebook (with Python 3 kernel) generated the non-linear random forest regression models for predicting BMI (biological BMI) from each of the Arivale baseline blood omic datasets, and calculated the testing (hold-out) set-derived BMI predictions for the Arivale cohort.  
Output figures and tables:  
* Intermediate tables for other notebooks (BMI predictions, feature importance)  

### 7. Code07_BMI-LASSO-vs-others.ipynb  
This Jupyter Notebook (with Python 3 kernel) compared the blood omics-based BMI models (model performance, BMI predictions, and predictor variables) between LASSO and the other methods (elastic net, ridge, and random forest).  
Output figures and tables:  
* Supplementary Figure 4  
* Tables for Supplementary Data 10  

### 8. Code08_DeltaBMI-misclassification_clustering.ipynb  
This Jupyter Notebook (with Python 3 kernel) visualized ∆BMI correlations across omics categories and ∆BMI-based misclassification (in the baseline Arivale cohort). Also, this notebook performed hierarchical clustering to reveal the underlying differences in ∆BMI misclassification, which was removed from the final paper but included in the original preprint.  
Output figures and tables:  
* Figure 3a, 3c  
* Tables for Supplementary Data 10  
* Intermediate table for other notebooks (biological BMI summary)  
* (Figure 3d, 3e and Supplementary Figure 5b, 5c in the original preprint)  

### 9. Code09_BMI-regression_numeric-features.ipynb  
This Jupyter Notebook (with Python 3 kernel) regressed the measured and omics-inferred BMIs independently on each of the available numeric physiological features (in the baseline Arivale cohort).  
Output figures and tables:  
* Figure 1e  
* Table for Supplementary Data 4  

### 10. Code10_DeltaBMI-misclassification_obesity.ipynb  
This Jupyter Notebook (with Python 3 kernel) assessed the relationships between ∆BMI-based misclassification (i.e., BMI class vs. biological BMI class) and obesity-related features (BMI-associated physiological measures, obesity-related health markers) using regression analysis (in the baseline Arivale cohort).  
Output figures and tables:  
* Figure 3d, 3e  
* Tables for Supplementary Data 6  

### 11. Code11_DeltaBMI_clinical-misclassification.ipynb  
This Jupyter Notebook (with Python 3 kernel) assessed differences in ∆BMI (1) between metabolically healthy normal-weight (MHNW) and metabolically unhealthy normal-weight (MUNW) and (2) between metabolically healthy obese (MHO) and metabolically unhealthy obese (MUO), based on a clinical definition (in the baseline Arivale cohort).  
Output figures and tables:  
* Figure 3b  
* Table for Supplementary Data 10  

### 12. Code12_DeltaBMI-misclassification_TwinsUK.ipynb  
This Jupyter Notebook (with Python 3 kernel) validated the findings about ∆BMI-based misclassification (i.e., BMI class vs. biological BMI class) with the TwinsUK cohort.  
Output figures and tables:  
* Supplementary Figure 6  
* Tables for Supplementary Data 6, 10  

### 13. Code13_DeltaBMI-misclassification_gut-microbiome.ipynb  
This Jupyter Notebook (with Python 3 kernel) assessed the relationships between ∆BMI-based misclassification (i.e., BMI class vs. biological BMI class) and gut microbiome alpha-diversity metrics using regression analysis (in the baseline Arivale cohort).  
Output figures and tables:  
* Figure 4b  
* Table for Supplementary Data 6  

### 14. Code14_Obesity-classifier_Arivale-gut-microbiome.ipynb  
This Jupyter Notebook (with Python 3 kernel) generated the random forest models for classifying participants into normal vs. obese class (based on either BMI or MetBMI) from the Arivale baseline gut microbiome dataset, and calculated the testing (hold-out) set-derived class (label and probability) predictions for the Arivale cohort. Because DeLong's test did not seem available in Python yet, DeLong's test was performed in another sub-notebook with R kernel.  
Output figures and tables:  
* Figure 4c, 4d  
* Tables for Supplementary Data 1, 10  
* Intermediate tables for the sub-notebook (class predictions)  

### 15. Code15_Obesity-classifier-DeLong_Arivale.ipynb  
This Jupyter Notebook (with R kernel) performed DeLong's test for the gut microbiome-based obesity classifiers in the Arivale cohort (as the sub-notebook).  
Output figures and tables:  
* Intermediate tables for the main notebook (ROC curve, test result)  

### 16. Code16_Obesity-classifier_TwinsUK-gut-microbiome.ipynb  
This Jupyter Notebook (with Python 3 kernel) generated the random forest models for classifying participants into normal vs. obese class (based on either BMI or MetBMI) from the TwinsUK gut microbiome dataset, and calculated the testing (hold-out) set-derived class (label and probability) predictions for the TwinsUK cohort. Because DeLong's test did not seem available in Python yet, DeLong's test was performed in another sub-notebook with R kernel.  
Output figures and tables:  
* Figure 4e, 4f  
* Tables for Supplementary Data 1, 10  
* Intermediate tables for the sub-notebook (class predictions)  

### 17. Code17_Obesity-classifier-DeLong_TwinsUK.ipynb  
This Jupyter Notebook (with R kernel) performed DeLong's test for the gut microbiome-based obesity classifiers in the TwinsUK cohort (as the sub-notebook).  
Output figures and tables:  
* Intermediate tables for the main notebook (ROC curve, test result)  

### 18. Code18_BMI-LASSO_Arivale-longitudinal.ipynb  
This Jupyter Notebook (with Python 3 kernel) calculated longitudinal BMI predictions from each of the Arivale time-series blood omic datasets, using the LASSO linear regression models that were fitted on the Arivale baseline datasets.  
Output figures and tables:  
* Intermediate tables for other notebooks (BMI predictions)  

### 19. Code19_Longitudinal-biological-BMI-LMM.ipynb  
This Jupyter Notebook (with Python 3 kernel) estimated longitudinal changes of the measured and omics-inferred BMIs during the Arivale program, using linear mixed model (LMM) with random effects for each participant.  
Output figures and tables:  
* Figure 5  

### 20. Code20_Network-interaction-analysis-GLM-GEE.ipynb  
This Jupyter Notebook (with Python 3 kernel) assessed the baseline analyte–analyte interactions with MetBMI using generalized linear model (GLM), and subsequently assessed the interactions between the siginificant analyte–analyte pairs and days in program using generalized estimating equations (GEE).  
Output figures and tables:  
* Figure 6b, 6c  
* Table for Supplementary Data 7  

### 21. Code21_Network-interaction-analysis-visualization.ipynb  
This Jupyter Notebook (with R kernel) visualized the analyte–analyte pairs that were significantly modified by MetBMI (i.e., GLM results) while highlighting the anayte–analyte pairs that were significantly modified by days in program (i.e., GEE results).  
Output figures and tables:  
* Figure 6a  

### 22. Code22_WHtR-LASSO_Arivale-baseline.ipynb  
This Jupyter Notebook (with Python 3 kernel) generated the LASSO linear regression models for predicting waist-to-height ratio (WHtR) (biological WHtR) from each of the Arivale baseline blood omic datasets, and calculated the testing (hold-out) set-derived WHtR predictions for the Arivale cohort.  
Output figures and tables:  
* Supplementary Figure 7d–i  
* Tables for Supplementary Data 1, 8, 10  
* Intermediate tables for other notebooks (WHtR predictions)  

### 23. Code23_WHtR-LASSO-bcoef.ipynb  
This Jupyter Notebook (with Python 3 kernel) visualized beta-coefficients of the blood omics-based WHtR LASSO models, and assessed relationships between WHtR and the retained variables using regression analysis (in the Arivale cohort).  
Output figures and tables:  
* Supplementary Figure 7j, 7k  
* Tables for Supplementary Data 9  

### 24. Code24_Biological-BMI-vs-WHtR.ipynb  
This Jupyter Notebook (with Python 3 kernel) compared the blood omics-based BMI LASSO models with the blood omics-based WHtR LASSO models. Also, this notebook visualized ∆WHtR correlations across omics categories, and assessed differences in ∆WHtR between clinically-defined metabolic health conditions (in the baseline Arivale cohort).  
Output figures and tables:  
* Supplementary Figure 7l, 7m, 8  
* Tables for Supplementary Data 10  

## Requirements  
The following package/library versions were used and hence confirmed at least.  
* Python (version 3.9.7)  
* NumPy (version 1.21.3)  
* pandas (version 1.3.4)  
* SciPy (version 1.7.1)  
* matplotlib (version 3.4.3)  
* seaborn (version 0.11.2)  
* scikit-learn (version 1.0.1)  
* statsmodels (version 0.13.0)  
* R (version 4.1.1)  
* tidyverse (version 1.3.1)  
* pROC (version 1.18.0)  
* circlize (version 0.4.15)  

## Log  
Last update on Jul 1, 2023  
* 2022-01-20 Generated this repository on GitHub.  
* 2022-01-24 Uploaded 9 Jupyter Notebooks, which were used for the preprint.  
* 2022-11-03 Uploaded 24 Jupyter Notebooks, which were used for the revised manuscript. (forced update...)  
* 2023-03-29 Updated README.  
* 2023-07-01 Updated README and released the current version for DOI.  
