# 44688-Data-Analytics-Capstone

Captone Project Report - Insurance Premium Charges

Author: Ashley Allen

Date:  3/20/2023


## Dataset

The dataset for this project can be found at: https://www.kaggle.com/datasets/teertha/ushealthinsurancedataset

## Report

The overleaf report can be found at: https://www.overleaf.com/read/fxvbrswhjxkb

## Research Goals
The goal of this research is to develop a machine learning model that accurately predicts the line-item value for antiretroviral drugs and HIV lab supplies that are to be shipped to countries negatively affected by the HIV/AIDS endemic. The goal is to make these predictions using a regression algorithm based off of known characteristics of the desired drug or lab test that could be found on a purchase order sent to a vendor or manufacturer. If a successful model is created, this could help nations and organizations better plan for future purchases of antiretroviral drugs and HIV supplies without having to wait for price quotes from manufacturers.


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

![Results](Regression Results.png)

## Future Work

The recommendation is to add additional datasets that provide more data, such as specific parts of the region and maybe the age of the children, to see if that had an effect on the insurance charges. Adding additional data will help predict insurance charges that are more accurately.
