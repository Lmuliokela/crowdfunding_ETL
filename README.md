# Project 2 - Crowdfunding_ETL

---

## Project Description

**Description:** For the ETL mini project, we worked in a group to build an ETL pipeline using Python, Pandas and Python dictionary methods to extract and transform the data. After transformation of the data, four csv files were created and further used to create an ERD and a table schema. At the end, the CSV files data was uploaded into a Postgres database.

---

## Setup:
- Imported the crowdfunding.xlsx excel data
- Extracted and transformed the data to create a category and subcategory dataframes and exported them as CSV files
- Extracted and transformed the data to create the campaign data frame
- Used python dictionary method to import the contacts.xlsx file into a dataframe where we iterated through the data and converted each row into a dictionary.
- Sketeched the ERD tables using Quick DBD and used the information from that to create a schema table for each csv file
- Imported the csv files into their corresponding SQL able.

  ---

## Dependenices

Import dependencies
import pandas as pd
import numpy as np
pd.set_option('max_colwidth', 400)

---

  ### Jupyter Notebook file

  - ETL_Mini_Project_LMuliokela_TNaran_RWilliams_AHabte (1).ipynb - script that was used for the anaysis

---

## Data Prep and Anaysis Steps

- Loaded the data into a Pandas DataFrame and displayed a brief summary of the crowdfunding info DataFrame
- Got the crowdfunding columns and assigned the category and subcategory values to category and subcategory columns.
- Got the unique categories and subcategories in separate lists. Put distinct values in the categories and subcategories lists.
- Created numpy arrays from 1-9 for the categories and 1-24 for the subcategories.
- Used a list comprehension to add "cat" and "subcat" to each category id.
- Created a category DataFrame with the category id array as the category id and categories list as the category name.Created a category 
  dataFrame with the subcategory id array as the subcategory id and subcategories list as the subcategory.
- Displayed category df
- Exported categories df and subcategories df as CSV files
- Renamed the blurb, launched_at, and deadline columns and converted the goal and pledged columns to a `float` data type. Displayed the 
  datatypes.
- Formated the launched date and end date columns to datetime format. Merged the campaign_df with the category_df on the "category" column and 
  the subcategory_df on the "subcategory" column.
- Dropped unwanted columns and exported the DataFrame as a CSV file
- Extracted the contacts.xlsx Data.Used Pandas to create the contacts DataFrame.
- Create a contact_info DataFrame and added each list of values, i.e., each row to the 'contact_id', 'name', 'email' columns. Displayed the 
  datatypes.
- Created a "first"name" and "last_name" column with the first and last names from the "name" column. Dropped the contact_name colum and reorder 
  the columns.
- Dispalyed the datatypes before exporting as CSV file.









  - 
