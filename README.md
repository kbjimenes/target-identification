# About

This repository provides an official implementation of 253 Target-centric models (TCM) develop over CHEMBL database.

# File structure

```
+-- TCM
|    +-- data
|    +-- SCALE
|        +-- DSC
|        +-- FUS
|    +-- AD
|        +-- DISTANCE
|            +-- FGP
|            +-- DSC
|    +-- MODELS
|        +-- FGP
|            +-- DTREE
|            +-- GM
|            +-- KNN
|            +-- RF
|            +-- SVM
|        +-- DSC
|            +-- DTREE
|            +-- GM
|            +-- KNN
|            +-- RF
|            +-- SVM
|        +-- FUS
|            +-- DTREE
|            +-- GM
|            +-- KNN
|            +-- RF
|            +-- SVM
```


# Resources
**Files:**

* '253TCM.csv'.- List of targets and their codes used for modeling TCM.
    + ﻿TARGET_ID.- Target ID
    + UNIPROT_ID.- Uniprot ID
 
**Directories:**

* '/data'.- Clean data for the CHEMBL releases 27, 28 and 31.
* '/TCM/SCALE'.- Models for scaling compound data for the physichochemical properties (DSC) and the fusion of morgan figer print and DSC descriptors (FUS)
* '/TCM/DcoS'.- Application domain based on distance for the TCM models. Inside there is the centroid(vector) and the limit used for training and validate each model.
* '/TCM/MODELS'.- TCM models trained with morgan’s  fingerprint (FGP), molecular properties (DSC) and the fusion of both (FUS) descriptors; and the algorithms of decision tree (DT), gaussian naive bayes (GM), k-nearest neighbors (KNN), random forest (RF) and support vector machine (SVM).

**Requirements**

- scikit-learn          0.23.2
- scipy                 1.7.1
- numpy                 1.19.5
- rdkit                 2021.03.5

**For more information:**
Please check the article (It will be available soon).

# Credit/Acknowledgment
This research was supported by Universidad de las Américas & Universidad da Coruña
