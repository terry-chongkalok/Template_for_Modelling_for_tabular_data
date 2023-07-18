# Complete Template for Modelling for Tabular Data

This project, in particular the notebook `Template_for_Modelling_for_tabular_data.ipynb` aimed at serving as a reusable notebook template in the feature engineering and model building stage when developing prediction model for tabular data.

It consisted of the standard model building workflow, and included numerous tools and techniques that are commonly used or useful in machine learning model development, such as:
- Custom Sklearn Data Imputer for filling missing values
- Custom Sklearn Categorical Feature Encoder
- Sklearn Pipeline for assembling imputation, feature encoding and modelling together and avoid data leakage in cross validation
- LightGBM (Related paper: [Why do tree-based models still outperform deep learning on tabular data?](https://arxiv.org/abs/2207.08815))
- BayesSearch (on hyperparameters of LGBM **AND** categorical feature encoding strategy)
- Feature Elimination by RFECV

(The dataset used in the template is the `Titanic` training dataset from Kaggle.
Please note, however, that this project did not aim at achieving a high Kaggle ranking, since the notebook was only for the feature engineering and model building stage, and did not include EDA and Error Analysis which are equally, if not more, important for developing accurate and robust models.)

## Project Folder Structure:

    Template_for_Modelling_for_tabular_data/
    ├─ Dataset/
    ├─ Model/
    ├─ __init__.py
    ├─ Template_for_Modelling_for_tabular_data.ipynb
    ├─ requirement.txt
    └─ README.md