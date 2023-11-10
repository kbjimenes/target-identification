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

# Requirements

- scikit-learn          0.23.2
- scipy                 1.7.1
- numpy                 1.19.5
- rdkit                 2021.03.5


## Resources
**Files:**

* '253TCM.csv'.- List of targets and their codes used for modeling TCM.
    + ﻿TARGET_ID.- Target ID
    + UNIPROT_ID.- Uniprot ID
 
**Directories:**

* '/data'.- Clean data for the CHEMBL releases 27, 28 and 31.
* '/TCM/SCALE'.- Models for scaling compound data for the physichochemical properties (DSC) and the fusion of morgan figer print and DSC descriptors (FUS)
* '/TCM/AD'.- Application domain based on distance for the TCM models. Inside there is the centroid(vector) and the limit used for training and validate each model.
* '/TCM/MODELS'.- TCM models.


# Datasets

CHEMBL 27, 28 and 31 releases were extracted and clean to get reliable data about interactions between compound and targets of HomoSapiends. These data was also used to train and test the 253 TCM. 

# Target-centric model (TCM)

A total of 253 targets were considered  with their compound interactions. The compound descriptors used were morgan’s fingerprint (FGP), molecular properties (DSC) and the fusion of both (FUS) descriptors with a model for scaling (TCM/SCALE) data was built for DSC and FUS descriptors; as well as, a limit threshold that was lated used to test the application domain (TCM/AD). Finally, the TCM were built considering each of the three descriptors and the algorithms of decision tree (DT), gaussian naive bayes (GM), k-nearest neighbors (KNN), random forest (RF) and support vector machine (SVM).

#  For more information:
Please check the article (It will be available soon).

# Credit/Acknowledgment
This research was supported by Universidad de las Américas & Universidad da Coruña
