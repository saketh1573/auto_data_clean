# Data Cleaning and Handling Null Values in Pandas

## Overview

This repository contains Python code for data cleaning and handling null values in a pandas DataFrame. The code is designed to be used as part of a data preprocessing pipeline for data warehousing and mining projects. It provides functionality to:

1. **Remove Columns with High Null Percentage**
   - Identify columns with null values exceeding a specified threshold percentage.
   - Allow users to choose whether to remove these columns from the DataFrame.

2. **Remove Tuples with Less Data**
   - Identify tuples with a number of non-null values less than a user-specified minimum.
   - Allow users to choose whether to remove these tuples from the DataFrame.

3. **Fill Null Values with Mean/Median/Mode based on User Choice**
   - Allow users to choose specific columns and fill null values in those columns using mean, median, or mode.

4. **Fill Null Values with Global Constant**
   - Identify columns with around 10% null values.
   - Allow users to enter a global constant value to fill null values in these columns.

5. **Fill Null Values by Class with User Input**
   - Allow users to choose a column representing the class variable.
   - Display null values and their percentages by class.
   - Allow users to choose columns and fill null values based on the mean or median of the class.

## Prerequisites

- Python 3.x
- Pandas library (`pip install pandas`)

## Usage

1. **Clone the Repository:**
git clone https://github.com/saketh1573/auto_data_clean


2. **Run the Code:**
- Execute the `fill_null_values.ipynb` script.

3. **Follow the Prompts:**
- Enter the path to the CSV file containing your data when prompted.
- Follow the menu to perform various data cleaning tasks.

## Example Usage
  Assuming 'your_data' is your DataFrame.
  1. **Cleaned data after removing columns with high null percentage**
     - cleaned_data = remove_columns_with_high_null_percentage(your_data)
  2. **Cleaned data after removing tuples with less data**
     - cleaned_data = remove_tuples_with_less_data(your_data)
  3. **DataFrame after filling null values with user choice**
     - data_filled = fill_nulls_with_3m(your_data)
  4. **DataFrame after filling null values with a global constant for columns with around 10% null values**
     - data_filled = fill_nulls_with_global_constant(your_data)
  5. **DataFrame after filling null values by class with user input**
     - data_filled = fill_nulls_by_class_user_input(your_data, 'class_column')

## Contributors
  -  [Sai Saketh Motamarry ](https://github.com/saketh1573)
  - Snehasri Motamarri 
  - Himasri Bandaru
  - Cheeli Deepthi
