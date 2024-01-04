# Data Preparation and Cleaning

## Overview
This section outlines the steps taken to prepare and clean the Cyclistic trip data for analysis.

## 1. Data Download
- Downloaded relevant files covering the period from 01/2023 to 09/2023 from [Divvy Trip Data](https://divvy-tripdata.s3.amazonaws.com/index.html).
- All files were in CSV format, and the download included compacted folders.

## 2. Folder Structure
- Created two folders: `source_data` and `clean_data`.
- Extracted contents of downloaded files into the `source_data` folder.

## 3. Data Cleaning
- Opened each CSV file to inspect and clean the data.
- Checked for duplicate entries.
- Filled missing values in columns `start_station_name`, `start_station_id`, `end_station_name`, `end_station_id` with "not specified" for consistency.
- Explored and addressed outliers in `rideable_type` and `member_casual` columns.
- Converted the started_at and ended_at column to datetime format.
- Replace missing or invalid values (NaN) in latitude and longitude columns using the Pandas replace method.
- I aggregated all the data into one (stupidly big) file.

## 4. Exploration and Additional Columns
- Created two new columns: `day_of_week` to identify the day of the week for each ride and `ride_length` to calculate the duration of each ride.
- Conducted a basic exploration, checking for patterns and outliers.
  
## 5. File Format
- Saved cleaned files as Excel workbooks (.xlsx).

## 6. Repository Upload
- Due to the large file sizes, the cleaned data files were uploaded to Kaggle instead of GitHub.

### Note
The dataset may not be uploaded to the GitHub repository directly due to its size. Refer to Kaggle for the cleaned [data files](https://www.kaggle.com/datasets/marcoshsq/divvy-tripdata/data).

For further details and technical insights into the data preparation and cleaning process, please refer to the specific Jupyter notebook or script used for the analysis.
