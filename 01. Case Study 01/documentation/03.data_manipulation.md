## Data Preparation and Cleaning

### Data cleansing report

This document describes the steps taken to prepare and clean the data for analysis.

### 1. Data download
- The downloaded data refers to the period from 01/2019 to 12/2019.
- The raw data can be found at [Divvy Trip Data](https://divvy-tripdata.s3.amazonaws.com/index.html).
- All files were in CSV format in compressed folders.

### 2. Data cleaning process
- I renamed the DataFrame columns to make the names more friendly and coherent.
- Searched and replaced null values in different columns.
- I filled the null values in the 'gender' column with the string 'unknown'.
- I filled in the null values in the 'birthyear' column with the average of the non-null values.
- Converted the 'start_time' and 'end_time' columns to date and time format.
- I calculated the difference between 'end_time' and 'start_time' to create the 'ride_length' column in hours.
- I extracted the day of the week from the 'start_time' column and created the 'day_of_week' column, where 1 represents Sunday, 2 Monday, etc.
- I renamed the columns again, this time to match the new names specified.
    
### Observation
The raw dataset could not be uploaded directly to the GitHub repository due to its size. See the original website [Divvy Trip Data](https://divvy-tripdata.s3.amazonaws.com/index.html) to access them.
