# Bike-Analysis
<img width="708" alt="image" src="https://github.com/user-attachments/assets/702a3729-4b37-4acf-a9a0-74882f463ece">

This analysis is all about getting to know the bike sales market better with an interactive excel dashboard.
To view the interactive dashboard: [https://1drv.ms/x/s!Asnw8nz7tJTEgXCXbpbFtH_-Tmri?e=ZJK1tq&nav=MTVfe0ZGMzUwOEQ5LTk5NTMtNDc0OC05OTUxLUZCREJGRTVFM0M5Mn0](https://1drv.ms/x/s!Asnw8nz7tJTEgXCXbpbFtH_-Tmri?e=OqUT9J&nav=MTVfe0ZGMzUwOEQ5LTk5NTMtNDc0OC05OTUxLUZCREJGRTVFM0M5Mn0)

## Summary
This analysis is here to share some great ideas on how we can make the market even bigger and more appealing to a wide range of consumers. We want to dive deep into the market's patterns, learn what makes people buy bikes, and see how we can encourage more bike purchases. As we explore the dataset, we'll uncover valuable insights that shed light on the factors that drive bike sales and influence customer behavior.

## Analysis
Overall there has been growth of bike purchases. Across different factors such as age brackets, marital status, education, etc the trend has been the same. There can several reasons for that such more people are conscious about their own health, the environment and the ease of transportation. Across different country the development in infrastructures such as roads and bike lines may have also encouraged this.

## Dataset (raw)
13 columns and 1027 rows. Columns: unique ID; Marital Status (Married or Single); Gender (Female or Male); Income Children (Number of Children); Education (Bachelors, Graduate degree, High School, Partial College, Partial High school); Occupation; Home Owner (Ownership of Home); Cars (# of Cars); Commute Distance (Distance travelled to work); Region; Age (in numerical form); Purchased Bikes (whether a customer purchased bikes or not).

## Data Cleaning
* Removing duplicates from the whole dataset: 26 rows were found using the func ‘remove duplicates’
* For Marital Status column, to differentiate from the ‘M’ and in gender, both column inputs were changed to their full form, i.e. M→ Married, S→Single for marital status, M→ Male, F→Female in gender column. This was easily performed using the Find & Select function.
* The data type column of the income column was changed from ‘General’ to ‘Accounting’.
* Age brackets are a great way for comparison hence a new column created. For that column, for better visualization and understanding in the dashboard, each age range was given a name: ‘Adolescent’, ‘Middle age’ and ‘Old age’. This was done using the nested if statement:
``` excel
=IF(L2>=54,"Old Age 55+",IF(L2>=31,"Middle Age 31-54",IF(L2<31, "Adolescent 0-30", "Invalid")))
```
## Pivot Tables:

Next for analyzing the dataset across different factors the following tables were created:

1. **Average income of Males and Females based on bike purchased  or notd**
<img width="482" alt="image" src="https://github.com/user-attachments/assets/dc36502d-34f4-4867-aa09-80626e3630f6">

2. **Count of purchased bikes based on commute distance**
<img width="482" alt="image" src="https://github.com/user-attachments/assets/bc80badb-c1d6-428c-a678-2cf6d0c2455d">

3. **Count of purchased bikes based on age brackets**
<img width="457" alt="image" src="https://github.com/user-attachments/assets/e167e51d-2460-403f-b1e5-a7b844bb56f8">

## Pivot Charts
From the pivot table, we can then create the pivot charts. Excel makes it easy to add the desired columns as rows, columns, values and filters and choose from the various chart designs. 
1. **Income vs Gender**
<img width="481" alt="image" src="https://github.com/user-attachments/assets/3676875b-1f62-4640-a709-5ce10259c9a5">

2. **Bike purchased over commuted distance**
<img width="481" alt="image" src="https://github.com/user-attachments/assets/5be58b1b-3df1-4f04-8730-2c33f569aa15">

3. **Count of bikes purchased over age brackets**
<img width="530" alt="image" src="https://github.com/user-attachments/assets/9cdfbf86-8016-488d-bd94-9ebc7f3941c8">

