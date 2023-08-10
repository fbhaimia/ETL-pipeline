# ETL-pipeline
This notebook is a part of my learning journey which i have been documenting from Data Science Program which helped me lot to learn ETL Pipeline.

## DATASET: 
I have taken 2 datasets for my analysis namely disaster_messages and disaster_categories. 
  1. Disaster_messages deals with all types of disaster related messages.
  2. Disaster_categories deals with all types of disaster categories.
     
Source: https://www.kaggle.com/code/chintan5384/etl-pipeline-preparation/input

## OUTLINE OF THIS NOTEBOOK:
### EXTRACT:
  1. Loading necessary libraries for the analysis.
  2. Data is extrscted from csv files.
  3. Understanding the datasets.

### TRANSFORM
  1. Dataset 1 - Cleaning:
     * Null Value Treatment - dropping the columns with more than 50% of null values.
  2. Dataset 2 - Cleaning:
       * Splitting Dataset - splitting performed as category column had jumbled data.
       * Renaming Column - column name renamed as per row title.
       * Label Encoding - converting categorical values to 0 and 1.
  3. Merging: combing the processed dataset 1 and dataset 2 with respect to ID.
  4. Duplicate Treatment: Droping duplicate values as minimun counts of duplicates are found in the merged dataset.

### LOAD
  1. Loading the processed dataset into SQL Database.
  2. Reading the dataframe from the database.
  3. Closing the database connection.


