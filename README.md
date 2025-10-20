# Analysis Code: Higher Dietary Omega-3 Fatty Acid Intake and CKM Syndrome

This repository contains the complete R code for the statistical analyses in the manuscript:

**"Higher Dietary Omega-3 Fatty Acid Intake Attenuates CKM Syndrome Progression and Mortality in US Adults: NHANES 1999-2018"**

## 📁 Repository Structure

- `weighted_cox_analysis.R` - Weighted Cox proportional hazards models for mortality analysis
- `weighted_ordinal_logistic.R` - Weighted ordinal logistic regression for CKM stage progression  
- `wqs_analysis.R` - Weighted quantile sum (WQS) regression for n-3 PUFA mixture effects
- `session_info.txt` - R session information for reproducibility
- `LICENSE` - MIT License for code reuse

## 🔧 Requirements





### R Packages
```r
# Core analysis packages
install.packages(c(
  "survival", "survey", "dplyr", "tidyr", "stringr", "readr",
  "broom", "ggplot2", "purrr", "MASS", "gWQS", "kableExtra",
  "gridExtra", "ggpubr"
))
```

## 📊 Data Source

All data used in this study are publicly available from the National Health and Nutrition Examination Survey (NHANES):  
[https://wwwn.cdc.gov/nchs/nhanes/Default.aspx](https://wwwn.cdc.gov/nchs/nhanes/Default.aspx)

## 🚀 Usage

1. Download NHANES data (1999-2018 cycles) from the official website
    
2. Preprocess data according to methods described in the manuscript
    
3. Run analysis scripts in sequence:
    

r

# CKM stage progression analysis
source("weighted_ordinal_logistic.R")

# Mortality analysis
source("weighted_cox_analysis.R")

# n-3 PUFA mixture effects
source("wqs_analysis.R")

## 📝 Citation

If using this code, please cite the original publication.

## ❓ Contact

For technical questions regarding the code, please contact the corresponding author.
