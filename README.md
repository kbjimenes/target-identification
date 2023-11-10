# About

Target-centric models (TCM) develop over CHEMBL database.

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

* File '253TCM.csv'.- List of targets and their codes used for modeling TCM.
    + ﻿TARGET_ID.- Target ID
    + UNIPROT_ID.- Uniprot ID
* Directory '/data'.- Clean data for the CHEMBL releases 27, 28 and 31.
* Directory '/TCM/SCALE'.- Models for scaling compound data for the physichochemical properties (DSC) and the fusion of morgan figer print and DSC descriptors (FUS)
* Directory '/TCM/DS'.- Application domain based on distance for the TCM models. Inside there is the centroid(vector) and the limit used for training and validate each model.
* Directory '/TCM/MODELS'.- TCM models trained with morgan’s  fingerprint (FGP), molecular properties (DSC) and the fusion of both (FUS) descriptors; and the algorithms of decision tree (DT), gaussian naive bayes (GM), k-nearest neighbors (KNN), random forest (RF) and support vector machine (SVM).

**For more information:**
Please check the article (It will be available soon).

# Credit/Acknowledgment
Copyright @ Universidad de las Américas & Universidad da Coruña
