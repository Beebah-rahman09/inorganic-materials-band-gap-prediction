# Machine Learning-Based Prediction of Electronic Band Gaps in Inorganic Materials for Energy Applications

## Project Overview

This project explores the application of machine learning to predict electronic band gaps in inorganic materials using composition-based numerical features.

Electronic band gap is an important property in materials science, particularly in the investigation of materials for energy conversion, electronic devices and related technologies.

The study uses the MatBench MP gap dataset and a Random Forest regression model implemented in Python.

## Research Question

How effectively can machine learning predict the electronic band gaps of inorganic materials using composition-based numerical features?

## Research Objectives

- Explore a large dataset of inorganic materials and their calculated band gaps.
- Extract numerical features from material compositions and structures.
- Develop a Random Forest regression model.
- Evaluate model performance using MAE, RMSE and R-squared.
- Investigate the effect of increasing dataset size on predictive performance.

## Dataset

The study uses the MatBench MP gap dataset, containing approximately 106,113 material records.

The target variable is the PBE-calculated electronic band gap, measured in electron volts (eV).

Materials with positive band-gap values were selected for the regression experiments.

A larger sample of 5,000 materials was used, divided into:

- Training set: 4,000 materials
- Testing set: 1,000 materials

## Methodology

The research workflow included:

1. Dataset acquisition and exploration
2. Statistical analysis of band-gap distribution
3. Selection of positive band-gap records
4. Extraction of seven numerical features
5. Training and testing using an 80:20 split
6. Random Forest regression
7. Comparison with baseline and Extra Trees models
8. Model evaluation and visualisation

## Extracted Features

- Number of atoms
- Number of elements
- Mean atomic number
- Minimum atomic number
- Maximum atomic number
- Mean atomic mass
- Atomic number variation

## Model Performance

The larger Random Forest experiment produced the following results:

| Metric | Result |
|--------|--------|
| MAE | 0.8972 eV |
| RMSE | 1.1905 eV |
| R-squared | 0.4425 |

## Effect of Dataset Size

Increasing the sample size from 1,000 to 5,000 materials resulted in:

- 11.61% improvement in MAE
- 12.94% improvement in RMSE
- An increase in R-squared from 0.1444 to 0.4425

These results indicate improved predictive performance with the larger dataset.

## Limitations

The model uses a limited set of composition-based features and does not fully represent crystal geometry, atomic positions or bonding environments.

The study focuses on positive PBE-calculated band gaps and does not establish experimental band-gap accuracy.

The R-squared value also indicates that substantial variation remains unexplained. Therefore, the model should be considered an exploratory baseline rather than a validated materials-screening tool.

## Future Research

Potential improvements include:

- Incorporating more detailed crystal-structure descriptors
- Exploring additional materials informatics features
- Applying cross-validation and chemical-system-based testing
- Evaluating gradient boosting and other machine learning approaches
- Testing model performance on independent datasets

## Tools and Technologies

Python | Google Colab | Pandas | NumPy | Matplotlib | Scikit-learn | Pymatgen | MatBench

## Conclusion

This project demonstrates an exploratory machine learning approach to predicting electronic band gaps in inorganic materials.

The findings show that increasing the dataset size improved model performance. Further research using more comprehensive structural descriptors and rigorous validation could improve predictive accuracy.

The work provides a foundation for further investigation in computational materials science and data-driven materials discovery for energy applications.
