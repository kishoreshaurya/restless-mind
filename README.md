# Restless Mind
2020-05-05
library(nnet)
library(readxl)

library(MASS)
## Warning: package 'MASS' was built under R version 3.6.1
library(pROC)
## Warning: package 'pROC' was built under R version 3.6.1
## Type 'citation("pROC")' for a citation.
## 
## Attaching package: 'pROC'
## The following objects are masked from 'package:stats':
## 
##     cov, smooth, var
MNL_data <- read_excel("C:/Users/Shaurya/Downloads/MNL Model.xlsx", 
                       sheet = 3)
## New names:
## * Gold -> Gold...4
## * Gold -> Gold...10
MNL_data$Product_Choice <- as.factor(MNL_data$Product_Choice)
str(MNL_data)
