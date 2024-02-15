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
       
       ![Select from bikebikestore](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/f1f45746-2047-46d0-90c2-ce75ca1291d7)

    * __For check the all the columns name and format types__
 
      ![Describe 1](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/6636c806-89fe-4159-8305-7ba3918aa2a8)

    * __For Rename some columns and modify data type__
 
      ![renamecolumn and datatype](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/ee3bc7ce-8109-4e28-aa1b-698a8a6f0d12)
      
   	* __I added three new columns: weekdays, months, and years.__
 
      ![daymonthyear](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/9451a35a-78c5-4d37-a31e-d2f19fe79856)

    * __Quick validation: I opened the CSV file and check the total revenue and total_units Revenue = 8578989 and Total_units = 7078. Everything looks good.__
 
      ![revenue validation](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/4e49173e-547f-45a3-be2a-360cc8fad232)
 
      ![units validation](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/a5de228f-fb98-45e6-8c7b-d0668a1e9d21)
      
    * __Quick analysis:__
       -	Total revenue by year:
   
         ![revenue by year](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/67757aca-0730-44d9-b7c9-64ec335aa54e)

       -	Total revenue by state:
   
         ![revenue by state](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/b8672c55-139b-4ebe-a583-4ffbe943f242)

       -	Total_units_sold by year:
   
         ![totalunit by year](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/fde75f0f-334e-42e0-844b-524ff554dfcf)

       -	Total_units_sold by state:
   
         ![totalunit by state](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/2fd8643e-edd0-4297-8d12-805f052d6916)
      
       -	Different stores:
   
         ![differentstore](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/9eefa2c9-eeb8-4fa9-964c-24183d66a983)

       -	Different bike’s category:
 
         
+ I exported (named bikestore_update) the data for visualization and analysis.





+ EDA
I used Power BI for visualization and analysis. I built an interactive Dashboard that contents 15 different charts such as clustered bar chart, clustered column chart, line chart, map chart, pie chart and donut chart. (Total revenue by Year, Total revenue by States, Total revenue by Store, Total revenue by Brand, Total revenue by Category, Total revenue by state and sales Representant, Top 10 revenue by cities, Bottom 10 revenue by cities, Top 10 revenue by customers, Bottom 10 revenue by customers, Total revenue by weekday, Total Revenue by Year and month, Total unit Sold by Year and month, Total revenue by Year and category, Total unit Sold by Year and category. 

+ Dashboard Validation
Before moving forward, I used SQL queries to validate the dashboard.




