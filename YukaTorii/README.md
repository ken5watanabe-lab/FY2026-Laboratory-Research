# Yuka TORII's Work

🇺🇸 English | [🇯🇵 日本語](./README_JPN.md)  
This directory contains the publicly shareable research outputs (e.g., Jupyter Notebooks, analysis scripts, and workflow programs) created by Yuka Torii during the FY2026 Laboratory Research, a third-year course at the Faculty of Medicine, Tokushima University.  

# Research Theme

**Development and Performance Evaluation of a Pancreatic Cancer Classification Model Using Blood Proteomic Data**

## Notebooks and Other Outputs

The `Proteomics_valildation398_Aichi` directory contains analysis code using pancreatic cancer status (presence or absence of pancreatic cancer) as the outcome.

The `Proteomics_valildation398_Aichi_Progress` directory contains analysis code using pancreatic cancer progression status as the outcome.

Descriptions of the individual notebooks are provided below.

### 1. Data Preprocessing, Visualization, and Quality Control

**`01A-preprocessing.ipynb`**

Loads and preprocesses proteomic data and sample metadata. The data are organized into a suitable format for subsequent statistical analyses and machine learning.

**`01B-Visualization.ipynb`**

Performs basic visualization of proteomic data and sample characteristics to explore data distributions and identify key features before analysis.

**`11-QC_Spearman.ipynb`**

Calculates pairwise Spearman correlation coefficients between samples to assess the similarity of proteomic expression profiles, evaluate sample consistency, and identify potential outliers.

**`12-QC_PlateEffect.ipynb`**

Evaluates the effects of measurement plates on proteomic data to determine whether systematic plate-related variation may affect comparisons between pancreatic cancer cases and controls.

**`12-QC_WELL_COUNT.ipynb`**

Examines well counts and data availability to assess measurement quality and identify potential missing-data issues.

**`12-QC_WELL_NPX.ipynb`**

Examines the distribution of Olink Normalized Protein eXpression (NPX) values and well-level measurement characteristics to identify potential measurement abnormalities and data quality issues.

### 2. Principal Component Analysis and Regression

**`02-pca_analysis.ipynb`**

Uses principal component analysis (PCA) to assess the overall structure of high-dimensional proteomic data. The distribution of pancreatic cancer cases and controls and the major patterns of variation in the data are examined.

**`03-regression_on_pca.ipynb`**

Uses regression analysis to investigate associations between principal components and pancreatic cancer status or other sample characteristics, identifying components associated with pancreatic cancer.

**`04-pca_violinplots.ipynb`**

Visualizes principal component scores by group using violin plots and related visualizations to examine differences in score distributions between pancreatic cancer cases and controls.

### 3. Protein Mapping, Differential Expression Analysis, and Functional Enrichment

**`10-Olink-Assay-Mapping.ipynb`**

Maps Olink assays to protein names and identifiers. Proteins are matched across datasets to establish the features used in subsequent analyses.

**`11-Limma.ipynb`**

Uses the `limma` package to statistically evaluate differences in protein expression between pancreatic cancer cases and controls. Differentially expressed proteins (DEPs) are identified using criteria that include multiple-testing correction.

**`12-EnrichmentAnalysis.ipynb`**

Performs enrichment analyses using Gene Ontology (GO) and pathway databases on DEPs and other selected protein sets to investigate biological functions and pathways associated with pancreatic cancer.

**`ORA.ipynb`**

Performs over-representation analysis (ORA) to determine whether specific biological functions or pathways are over-represented among selected proteins.

### 4. WGCNA and Module Analysis

**`13-WGCNA.ipynb`**

Uses weighted gene co-expression network analysis (WGCNA) to group proteins with similar expression patterns into co-expression modules. Associations between modules and pancreatic cancer status are investigated to identify relevant protein groups.

**`14-EigengeneML.ipynb`**

Uses module eigengenes, which represent the overall expression patterns of WGCNA modules, as features to develop and evaluate machine learning models for classifying pancreatic cancer status.

**`Module_enrichment.ipynb`**

Performs functional enrichment analysis for individual WGCNA protein modules to investigate their associated biological functions.

**`Module_enrichment-Connect.ipynb`**

Investigates module functions and potential key proteins while considering the relationships and connectivity among proteins within each module.

### 5. Pancreatic Cancer Classification and Model Interpretation

**`21A-Classifier.ipynb`**

Develops classification models, including Random Forest models, using proteomic data as features and pancreatic cancer status as the outcome.

**`21B-Classifier-SHAP.ipynb`**

Uses SHapley Additive exPlanations (SHAP) to interpret classification model predictions. The contribution of individual proteins to pancreatic cancer predictions is evaluated to identify important features.

**`21B-Classifier-Stratify.ipynb`**

Evaluates pancreatic cancer classification performance using stratified cross-validation and related approaches. The data are split while preserving group proportions to assess the robustness and reliability of model performance estimates.

**`21D-Classifier-ICD.ipynb`**

Uses ICD-related diagnostic information and classification codes to organize diagnostic categories and labels for use in pancreatic cancer classification analyses.

**`22-SHAPvalue.ipynb`**

Aggregates SHAP values to evaluate protein importance in the pancreatic cancer classification model and visualize proteins with substantial contributions to predictions.

**`22-SHAPvalue2.ipynb`**

Performs additional analyses and visualizations of SHAP values to further investigate protein importance and model prediction characteristics.

### 6. CA19-9-Related Analyses

**`21C-Classifier-predictCA19-9.ipynb`**

Develops and evaluates regression models to predict CA19-9 levels from proteomic data. The relationship between predicted and measured CA19-9 levels is examined, along with potential applications to pancreatic cancer classification.

**`21C-predictCA19-9_Limma.ipynb`**

Focuses on the residuals between predicted and measured CA19-9 levels and uses `limma` and related analyses to identify proteins associated with these residuals. The analysis explores whether these residuals reflect biological characteristics not fully captured by measured CA19-9 alone.

**`ca19-9relation.ipynb`**

Investigates relationships among CA19-9, proteomic data, and pancreatic cancer status. The diagnostic performance of CA19-9 alone and its associations with other proteins are examined.

## Requirements

Software, package, and environment requirements should be specified as needed. Please ensure that the required dependencies are installed before running the notebooks.

## License

Please specify the applicable license, if any, or include a `LICENSE` file in this directory as appropriate.


## Log
- Created this directory: Oct. 21, 2026 (Kengo Watanabe)
- Uploaded the research output: Oct. 29, 2026 (Yuka Torii)
