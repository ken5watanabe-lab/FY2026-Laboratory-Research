# Akari FUJIMOTO's Work

🇺🇸 English | [🇯🇵 日本語](./README_JPN.md)  
This directory contains the publicly shareable research outputs (e.g., Jupyter Notebooks, analysis scripts, and workflow programs) created by Akari FUJIMOTO during the FY2026 Laboratory Research, a third-year course at the Faculty of Medicine, Tokushima University.  

## Construction and evaluation of a biological age model derived from blood metabolome data in the Japanese population
This study used data from the Tohoku Medical Megabank Project to construct a biological age model derived from blood metabolome in the Japanese population.   
Seven age prediction models were created using LASSO regression from three platforms: metabolome, specific health checkups, and clinical laboratory tests.   
Furthermore, the difference between predicted age and actual age was calculated as Δage, and its association with clinical laboratory items and medical history was evaluated.   

## Notebooks and Other Materials
### Preprocess
1. 1_25117_TMM-BAge_Precheck-ver1.ipynb
- Loading the original data
- Checking the data structure
2. 2_260916_TMM_preprocess-ffq.ipynb
- Quality check
3. 3_260924_TMM-BAge_Preproceess_Metabolome.ipynb
- Extraction of data to be analyzed
- Quality check
4. 4_261008_TMM-BAge_lifestyle-preprocess.ipynb
- Extraction of data to be analyzed
5. 5_260930_TMM-BAge_specific-panel.ipynb
- Extraction of data to be analyzed
- Data preprocessed
6. 6_261005_TMM-BAge_laboratory-panel.ipynb
- Extraction of data to be analyzed
- Data preprocessed
7. 7_261002_TMM-BAge_MetAge-preprocess.ipynb
- Data preprocessed
### Model creation
8. 8_261016_TMM-BAge_MetAge-LASOO-regressionSHAP.ipynb
- Creating a metabolome-derived model
- Calculate SHAP value
9. 9_261019_TMM-BAge_SpeAge-LASSO.ipynb
- Creating a specific health check up-derived model
10. 10_261019_TMM-BAge_LaboAge-LASSO.ipynb
- Creating a laboratory test-derived model
### Plotting
11. 11_261019_TMM-BAge_model-comparision.ipynb
- Comparison between categorical models
### Regression analysis
12. 12_261019_TMM-BAge_pheno-panel-regression.ipynb
- Phenotypic regression analysis


## Requirements
- python 3.10.12
- pandas
- numpy
- scikit-learn
- matplotlib
- japanize-matplotlib
- seaborn
- statsmodels
- miss forest

## Licence
The analysis data will not be made public.

## Requirements, Licence, Acknowledgement, etc.
Data from the Tohoku Medical Megabuck Project was used.

## Log
- Created this directory: Oct. 21, 2026 (Kengo Watanabe)
- Uploaded the research output: Oct. 22, 2026 (Akari FUJIMOTO)
