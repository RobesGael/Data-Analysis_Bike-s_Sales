# Data-Analysis_Bike-s_Sales 
## Overview
The Management wants to know the conditions of sales activities within the company and gain insights into the various trends happening in the sales revenue and quantity over the 2016 to 2018 period.
## Getting Started
Prerequisites: Word, Excel, PowerPoint, SQL, Power BI.
## Usage
+ Understand the problem and build the project proposal using Word.
  
+ Collect and gather the data: 
  -	Data source: I used the link within the description of this video to download the data. https://youtu.be/1pHYKdyRvrw?si=xtlKY-EUXwLuAQew
  -	Data format: The dataset (bikestore) is a CSV file and has 4 722 rows and 12 columns.
  -	Data type: No idea. (It’s important to know if the data along the first-party data, the second-party data, or the third-party data. That could be helpful when dealing with missing values)
    
+ Data cleaning and preprocessing:
  -	The data has no missing values. To check this, open the Excel file and go to the Home Tab, Click to Find & Select – Go to Special – Check Blanks and then Ok.
  -	No duplicates records found: Go the Data Tab – Data Tools group – Click to Remove duplicates and then Ok.
  -	I formatted the Order_date column: Select the entire column - Go to Data Tab – Text to column – Next – Next – Check Date and choose DMY – Finish.
  -	I changed the format date from mm-dd-yyyy to yyyy-mm-dd: Select Order_date column – Right click – Format cells – custom – Type yyy-mm-dd – ok.
  -	I Opened MySQL Workbench and imported the bikestore dataset.
  -	I Preformed the following SQL queries:
     * __For discover the data__
