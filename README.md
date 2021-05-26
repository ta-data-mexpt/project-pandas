![IronHack Logo](shark-attack.jpg)

# Project: "Shark attacks" Data Cleaning and Manipulation with Pandas.

## Overview

The goal of the project is wrangling, cleaning, and manipulation a Shark attack dataset with Pandas. If you will follow the project download the dataset from [Shark Attack](https://www.kaggle.com/teajay/global-shark-attacks/version/1). 
at the end we will export it as a clean CSV data file.

## Technical Requirements

* The dataset shark-attacks.
* Pandas library.
* A Jupyter Notebook ** shark-attack-data-cleaning.ipyng ** with code.
* A clean shark_attack_clean_dataset.csv file.

## Development procedure

* 1- Import libraries we'll use ``Pandas``, ``Numpy``, ``digists`` and ``DateTime``.
* 2- Import shark-attack dataset into a pandas dataframe.
* 3- Analize data with pandas methods like **info(), head() and datacolums**.
* 4- Develop functions to treat data as follow:
    * 1 ``select_useful_columns_1()`` - Chosing relevants columns from main data.
    * 2 ``rename_columns()`` - Change some titles names to best undertanding.
    * 3 ``data_nulls()`` - null's treatment.
    * 4 ``to_numeric()`` - return just numeric values in string.
    * 5 ``get_numeric()`` - get numeric values from data.
    * 6 ``fill_na()`` - fill NaN with an specific value.
    * 7 ``cast_colum()`` - Change column type.
    * 8 ``extract_date()`` - Extract date from a object.
    * 9 ``get_date()`` - Extract date from field with date in.
    * 10 ``select_useful_columns_2()`` - Select final columns.
    * 11 ``re_order_columns()`` - to arrange columns appropriately.
* 5-**Main Pipeline** transform data from a function to another.
* 6-Export final dataframe to a **shark-attack.csv** file.

## Useful Resources

* [Pandas Documentation](https://pandas.pydata.org/pandas-docs/stable/)
* [Pandas Tutorials](https://pandas.pydata.org/pandas-docs/stable/tutorials.html)
* [StackOverflow Pandas Questions](https://stackoverflow.com/questions/tagged/pandas)
* [Awesome Public Data Sets](https://github.com/awesomedata/awesome-public-datasets)
* [Kaggle Data Sets](https://www.kaggle.com/datasets)
