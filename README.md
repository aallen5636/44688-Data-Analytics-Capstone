# 44688-Data-Analytics-Capstone

Captone Project Report - Insurance Premium Charges

Author: Ashley Allen

Date:  3/20/2023


## Dataset

The dataset for this project can be found at: https://www.kaggle.com/datasets/teertha/ushealthinsurancedataset

## Report

The overleaf report can be found at: https://www.overleaf.com/read/fxvbrswhjxkb

## Research Goals
This project aims to determine medical costs billed by health insurance depending on age, BMI, dependents, and whether or not the patient smokes. The rest of this paper is organized by the methodology, cleaning data, and results. 


## Setup
The following applications installed for ta his project:
- Python 3: https://www.python.org/downloads/
- numpy: https://pypi.org/project/numpy/
- pandas: https://pypi.org/project/pandas/
- matplotlib: https://pypi.org/project/matplotlib/
- seaborn: https://pypi.org/project/seaborn/
- scikit-learn: https://pypi.org/project/scikit-learn/
- jupyterlab: https://jupyter.org/install

## Results

After completing the linear, polynomial, and elastic net regression, all of the models performed about the same. One exception is the Linear Regression for region which appears to be performing under the mean of the target with an $R^2$ at 0.0001 for the training set and -0.0015 for the test set. This means that the independent variable, region, increases, and the dependent variable, charges, decreases. This means that Region has a very low correlation to charges. Charges are similar in all regions. Even though Sex and children don't have a negative $R^2$, we can see a low correlation. It was determined after the project that additional data may be beneficial to get a better prediction in the future for insurance charges. 

<img width="717" alt="Regression Results " src="https://user-images.githubusercontent.com/95989498/233857065-6abccdcc-e06a-4bf7-8920-3c6b40128e95.png">

## Future Work

The recommendation is to add additional datasets that provide more data, such as specific parts of the region and maybe the age of the children, to see if that had an effect on the insurance charges. Adding additional data will help predict insurance charges that are more accurately.
