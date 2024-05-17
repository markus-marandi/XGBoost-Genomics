# XGBoost-Genomics

## Description
This repository contains code for processing phenotypic and genomic data for machine learning. It includes steps for parsing data, generating MatrixTables, data aggregation, and preparing datasets. It also covers implementing and evaluating XGBoost models to advance clinical genetics analysis.

## Overview
This project investigates the complexities of genomic data analysis for detecting disease-related mutations, with a focus on hereditary breast cancer. Utilizing a dataset of 7,498 patient records from Tartu University Hospital, including 2,449 identified with breast cancer, we reannotated all VCF files using the Variant Effect Predictor (VEP) to align with current genomic standards.

## Key Features
- **Data Reannotation**: VCF files reannotated using VEP.
- **Feature Selection**: Selected critical fields such as 'IMPACT', 'QUAL', 'DP', 'QD', and 'MAX_AF' for training.
- **Model Training**: Trained an XGBoost model to enhance predictive accuracy.
- **Handling Imbalanced Data**: Addressed challenges of imbalanced datasets to improve model performance.

## Challenges and Findings
- The model achieved high overall accuracy but demonstrated high specificity and low sensitivity.
- Precision-recall curves provided a more accurate depiction of model performance than ROC curves.
- The model significantly reduced the number of rows for clinical review but had limited success in detecting true positive cases.
- Highlighted the need for improved techniques to handle imbalanced datasets and suggested future studies to incorporate additional genomic parameters.

## Methodology
- **Dataset**: 7,498 patient records from Tartu University Hospital.
- **Annotation Tool**: Variant Effect Predictor (VEP).
- **Machine Learning Model**: XGBoost.
- **Feature Selection**: Selected fields such as 'IMPACT', 'QUAL', 'DP', 'QD', and 'MAX_AF'.
- **Evaluation**: Precision-recall curve and ROC curve analysis.

## Future Directions
- Incorporate additional genomic parameters such as CADD and PolyPhen scores.
- Explore advanced methods like natural language processing for genomic data analysis.

## Research Context
- **Project**: Oligogenic Inheritance in Genetic Diseases.
- **Funding**: Estonian Research Council.
- **Ethics**: Conducted under protocol 362/T-6 of the University of Tartu Research Ethics Committee.
- **Data Privacy**: Data analysis performed according to the data protection plan; data is not publicly available.

## Supervisors
- PhD Hedi Peterson
- MD Villem Pata

## Principal Investigator
- Dr. Sander Pajusalu, University of Tartu, Faculty of Medicine, Institute of Clinical Medicine.

## Keywords
- Machine learning
- Variant annotation
- Predictive modelling
- Imbalanced dataset
- Data reannotation
- Genomic diagnostics

## CERCS Classification
- B110 Bioinformatics

## License
This project is licensed under the terms of the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License. For more information, please refer to the LICENSE file in the repository.