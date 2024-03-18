# Sales-Dashboard
Sales Analysis PowerBI Dashboard is to provide stakeholders with a concise and visually compelling platform for analyzing sales data. It enables users to quickly gain insights into sales performance, trends, and customer behavior, empowering them to make data-driven decisions, enhance strategic planning, and maximize profitability.

# Sales Dashboard 

### Dashboard Link : ![Sales Dashboard](https://github.com/Ishikamate/Sales-Dashboard/assets/85469773/d6cee0a9-9b8d-4cae-bf5c-023162b9c77d)

## Problem Statement

The business request for this data analyst project was an executive sales report for sales managers. Based on the request that was made from the business we following user stories were defined to fulfill delivery and ensure that acceptance criteria’s were maintained throughout the project.


1	Sales Manager(role)
-	To get a dashboard overview of internet sales	Can follow better which customers and products sells the best (request / demand)
-	A Power BI dashboard which updates data once a day
2	Sales Representative(role)
-	A detailed overview of Internet Sales per Customers	Can follow up my customers that buys the most and who we can sell more to(request / demand)
-	A Power BI dashboard which allows me to filter data for each customer(user value)
3	Sales Representative(role)	
A detailed overview of Internet Sales per Products	Can follow up my Products that sells the most (request / demand)
-	A Power BI dashboard which allows me to filter data for each Product (user value)
4	Sales Manager(role)	
-A dashboard overview of internet sales	Follow sales over time against budge(request / demand)	- A Power Bi dashboard with graphs and KPIs comparing against budget.(user value)



### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : It was observed that in none of the columns errors & empty values were present except column named "Arrival Delay".
- Step 5 : For calculating average delay time, null values were not taken into account as only less than 1% values are null in this column(i.e column named "Arrival Delay") 
- Step 6 : In the report view, under the view tab, theme was selected.
- Step 7 : Since the data contains various ratings, thus in order to represent ratings, a new visual was added using the three ellipses in the visualizations pane in report view. 
- Step 8 : Visual filters (Slicers) were added for four fields named "Class", "Customer Type", "Gate Location" & "Type of travel".
- Step 9 : Two card visuals were added to the canvas, one representing average departure delay in minutes & other representing average arrival delay in minutes.
           Using visual level filter from the filters pane, basic filtering was used & null values were unselected for consideration into average calculation.
           
           
  # Data Cleansing & Transformation (SQL)
To create the necessary data model for doing analysis and fulfilling the business needs defined in the user stories the following tables were extracted using SQL.

One data source (sales budgets) were provided in Excel format and were connected in the data model in a later step of the process.

Below are the SQL statements for cleansing and transforming necessary data.

 #  Tables Uses


-DIM_Coustomer:
![Screenshot 2024-03-18 121302](https://github.com/Ishikamate/Sales-Dashboard/assets/85469773/da4c3c2b-abb0-4888-9346-46869875cd8d)

-DIM_Products:

![Screenshot 2024-03-18 121442](https://github.com/Ishikamate/Sales-Dashboard/assets/85469773/ec7546f5-0013-4ea9-9578-c6a6fe245b39)

-FACT_InternetSales:

![Screenshot 2024-03-18 121420](https://github.com/Ishikamate/Sales-Dashboard/assets/85469773/fca6239b-8cec-40b1-98d8-ea52b4599455)




# Data model
![Screenshot 2024-03-18 121551](https://github.com/Ishikamate/Sales-Dashboard/assets/85469773/1cb87b43-9854-47f7-b405-400d91edd00b)

#  Sales Management Dashboard
The finished sales management dashboard with one page with works as a dashboard and overview, with two other pages focused on combining tables for necessary details and visualizations to show sales over time, per customers and per products.

Click the above link to to open the dashboard.
