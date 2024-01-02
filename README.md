# HR ANALYSIS

## Table of Contents

   - [Project Overview](#project-overview)
   - [Data Source](#data-source)
   - [Tools utilized](#tools-utilized)
   - [Data Cleaning steps](#data-cleaning-steps)
   - [Exploratory Data Analysis(EDA)](#exploratory-data-analysis(eda))
   - [DAX codes used for analysis](#dax-codes-used-for-analysis)
   - [Results and findings](#results-and-findings)
   - [Recommendition](#recommendition)

### Project Overview
  This data analysis project aims to provide insoghts into the HR analystics of a chocaltier company. By analysis various asspects of data, we seek to identify trends, make data driven recomendations, and gain a deeper understanding of the emplyee wages and recruitment.

### Data Source
HR Data: The primary dataset usedd for this analysis is an excel format dataset cantaining detailed information about employees and wages.

### Tools Utilized

- Cleansing the data : Microsoft Excel and Power query editor.
     - [Download](https://microsoft.com)
- Visualization and Analysis : Power BI

### Data Cleaning steps

In th intial data prepation phase, I performed the following tasks:
     1. Data Loading and inspection
     2. Handling the missing values
     3. Data cleansing and formating
     4. Merging different tables and prepared Master table. 

### Exploratory Data Analysis(EDA)

   EDA involved in exploring the HR data to answer the key questions, such as:

         1.How many people are in each job?
         2.Gender breakdown of th employees
         3.Age spread of the employees.
         4.Which job pay more?
         5.Qualificatiob vs salary
         6.Employee growth trend overr time
         7.Leave balance analysis

  ### DAX codes used for analysis
        
       - Average salary = Average(data[Salary]) 
       - Avg.Leavebalance = Average(data[Leave Balance])
       - Cumulatuve Count = VAR Currentdate =LASTDATE(data[Date of Join])
                   Return
                   Calculate([Head Count],all(data[Date of Join]),data[Date of Join] <= Currentdate)
       - Head Count = count(data[Emp ID])
       - LBL over 20days = Calculate([Head Count],data[Leave Balance] >20
       - Max_Salary = Max(data[Salary])
       - Min_Salary = Min(data[Salary])


  ### Results and findings:

       1. Increase in recruitment over time.
       2. Product Manager Job title has the highest salary
       3. Maximum nuber of employees are in mid 30years

  ### Recommendition:

    Based on the analysis I recomend the following actions:

       1. Pay grade of packing associate should be increaseed.
       2. There are 29 employees with LBL over 20 days need to be given time for vacation so that there is work life balance.
       3. Number of female employees need to be increaseed.


#### Limitations:

     As sample size is very small, I cannot get perfect insights from the data.

🙂
  






   
