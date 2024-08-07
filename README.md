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

         ![differentcategory](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/0d18c344-d033-4547-8a1a-dd1d5956c625)
 
         
+ I exported (named bikestore_update) the data for visualization and analysis.





+ EDA: 
I used Power BI for visualization and analysis. I built an interactive Dashboard that contents 15 different charts such as clustered bar chart, clustered column chart, line chart, map chart, pie chart and donut chart. (Total revenue by Year, Total revenue by States, Total revenue by Store, Total revenue by Brand, Total revenue by Category, Total revenue by state and sales Representant, Top 10 revenue by cities, Bottom 10 revenue by cities, Top 10 revenue by customers, Bottom 10 revenue by customers, Total revenue by weekday, Total Revenue by Year and month, Total unit Sold by Year and month, Total revenue by Year and category, Total unit Sold by Year and category. 

+ Dashboard Validation:
Before moving forward, I used SQL queries to validate the dashboard.

      - Total revenue by Year

![V rev by year](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/9ce5f871-7e73-4c01-90ff-9e9abc1e97d6)

      - Total revenue by State
    
![V rev by state](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/a374ebea-d550-48ee-95e6-2cb805324a4e)

      - Total revenue by Store

![V rev by store](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/8d64d9c1-97aa-44f8-acc5-aadf612936bb)

      -	Total revenue by Brand
      
![V rev by brand](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/6e13fa09-71d3-4d02-8799-8af30c5923b6)

      -	Total revenue by Category

![V rev by category](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/c2d1b195-9095-4e5f-aa95-01a05749c44d)

      -	Total revenue by state and sales Representant

![V rev by state and sales_rep](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/452f20bc-c789-4bc4-ad89-3a33aed6e777)

      -	Top 10 revenue by cities

![V top 10 rev](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/f1373fce-1f9e-4b6a-a9f1-57b98df632e5)

      -	Bottom 10 revenue by cities

![V bottom 10 rev by city](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/860700ff-ea91-40f4-9cf8-7a74f92651a9)

      -	Top 10 revenue by customers

  ![V top 10 rev by customers](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/c5dce5e2-5039-468c-b1bd-c1af1ac1259a)

      -	Bottom 10 revenue by customers

  ![V bottom 10 rev by customer](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/6390361c-6c7d-414c-8eb0-4990e6b8bbfd)
  
      -	Total revenue by weekday

  ![V rev by weekday](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/a8345cf5-77dc-43b9-a98a-e2327e4bcc2b)
  
      -	Total Revenue by Year and month

  ![V rev by year and month](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/a1c181f2-69ae-46e0-bb3e-292cb4991787)
  
      - Total units Sold by Year and month

  ![V unitsold by year and month](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/81d0fe55-c218-4b22-b491-d7f198d51ae6)

      -	Total revenue by Year and category

  ![V rev by year and category](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/1c74369d-727a-41ab-bfc6-fac05a7342f7)
  
      -	Total units Sold by Year and category

  ![V unitsold by year and category](https://github.com/RobesGael/Data-Analysis_Bike-s_Sales/assets/155399653/fec9922b-faa6-4302-8b90-e0ea46c8fb5f)


## Share findings and insights to Stakeholders

I used the interactive Power Bi dashboard , the executive summary and PowerPoint slides to share my findings to stakeholders.





