# Predict-Future-Sale-EDA

This repository documents a data science project. In the project, we analyze a electronic retail company's sale records, perform EDA and Cleaning on the data. The dataset we use is due to this [Kaggle competition](https://www.kaggle.com/c/competitive-data-science-predict-future-sales/data).

To-do: we have yet to build predictive models to predict future sale.


### Table of Contents


1. [Overview](#overview)
2. [File Descriptions](#files)
3. [Environment](#installation)
4. [Acknowledgement](#source)
5. [Licensing](#licensing)



## Overview<a name="overview"></a>

In this project, we work with a challenging and realistic time-series dataset consisting of daily sales data of an electronic retail company.

We first perform data cleaning, EDA, feature engineering (in 1_Notebook).

Some challenges dealt with so far:

- Train and Test data are not homogeneous:
the train data consists of sale history of various items in various shops. If an item is not sold in a particular shop, it will not appear in the train data. However, we need to predict the monthly sale of every items in every shops.
We transform the train data into the the form of the test/output data.

- Long-tail data:
the target values in the train data range from -13 to 2000+ but with an exponentially decaying distribution. We perform a [1%, 99%] truncation of the data, narrowed the number of target values to 19. This will be a highly imbalanced classification problem.

To-be-added:

2_Notebook: More feature engineering and Time series analysis.
3_Notebook: Modeling.

## File Descriptions <a name="files"></a>

- 1_Notebook: Data Cleaning and EDA.

- 1_raw_train: cleaned raw training data from 1_Notebook.

- 1_train: processed and engineered training data from 1_Notebook.

- 1_test: processed testing data from 1_Notebook.

- the zip file: raw data


## Environment <a name="installation"></a>

- The Anaconda distribution of Python3.
- Jupyter Notebook.  
- XGBoost. See [here](https://xgboost.readthedocs.io/en/latest/build.html) for installation guide.

## Acknowledgement <a name="source"></a>

The dataset comes from to this [Kaggle Competition](https://www.kaggle.com/c/competitive-data-science-predict-future-sales/data).

## Licensing <a name="licensing"></a>

 You can find the Licensing for the dataset and other descriptive information in the link above.  Other than that, feel free to use anything here as you would like!
