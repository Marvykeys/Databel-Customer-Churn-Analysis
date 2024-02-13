# Databel-Customer-Churn-Analysis :chart_with_downwards_trend:
## Scope :page_with_curl:
This report is focused on investigating a dataset from an example telecom company called Databel and analyze their churn rates. Analyzing churn doesn’t just mean knowing what the churn rate is, it’s also about figuring out why customers are churning at the rate they are, and how to reduce churn.
Useful insights were obtained.
## Data Design :bar_chart:
The raw data provided were downloaded in CSV file formats and it came with some of its contents being improperly formatted hence, a proper data cleaning had to be done.
## Import and Transform Data :scroll:
After downloading the data which was in CSV file format, I imported the data into Microsoft Power BI being the tool I’ll be using for analysis and visualization.                 

<img width="587" alt="DATABEL BI 1" src="https://github.com/Marvykeys/Databel-Customer-Churn-Analysis/assets/130637591/ae38d644-583b-48c5-a3cf-d19d2045a221">

##
Now, you see below, All columns in the dataset are loaded.                                                                                                                                 
<img width="238" alt="DATABEL BI 2" src="https://github.com/Marvykeys/Databel-Customer-Churn-Analysis/assets/130637591/2642ac24-28ae-45a5-b9f5-f36b05665624">

## Data Cleaning/Check :shower:
I created two measures to check if the count of customer ids is equal to the count of unique customer ids to make sure there aren't duplicate rows.

<img width="399" alt="DATABEL BI 3" src="https://github.com/Marvykeys/Databel-Customer-Churn-Analysis/assets/130637591/2e101ad6-2b43-44d1-8f3c-c0a7115f1115">

##

<img width="211" alt="DATABEL BI 7a" src="https://github.com/Marvykeys/Databel-Customer-Churn-Analysis/assets/130637591/d9a60c3e-71e2-40a2-b28c-c2f7eecdc154">


##

<img width="465" alt="DATABEL BI 4" src="https://github.com/Marvykeys/Databel-Customer-Churn-Analysis/assets/130637591/ca83a5e5-8d9a-4938-9c3c-5debfa9cd19e">

##
There is a column called "Churn Label" that indicates "Yes" or "No". I converted this column into a column indicating if a customer churned or not.     

<img width="401" alt="DATABEL BI 5" src="https://github.com/Marvykeys/Databel-Customer-Churn-Analysis/assets/130637591/72b61b74-fc96-4726-b2be-eddf1a0b2e3c">

##
I used the churned column I created to create a measure called "Number of Churned Customers".                                                                           

<img width="448" alt="DATABEL BI 6" src="https://github.com/Marvykeys/Databel-Customer-Churn-Analysis/assets/130637591/e746b0b5-9cc3-46cd-890f-79e45abdf0d9">

##
I calculated the churn rate and formatted as a percentage. 

<img width="545" alt="Churn Rate" src="https://github.com/Marvykeys/Databel-Customer-Churn-Analysis/assets/130637591/82c422ca-3a63-4e63-998a-b4112e41c810">

##

<img width="157" alt="DATABEL BI 7b" src="https://github.com/Marvykeys/Databel-Customer-Churn-Analysis/assets/130637591/7b98d0f8-32f5-463f-84e3-248a69b7273e">


##
I visualize the reasons why customers become churners by using "Number of Customers" & "Churn Reasons".                                                                                                             
<img width="582" alt="DATABEL BI 9" src="https://github.com/Marvykeys/Databel-Customer-Churn-Analysis/assets/130637591/31033329-13aa-4df2-902a-5df96c737bea">

##
I visualize the churners by Churn Category.

<img width="391" alt="DATABEL BI 10" src="https://github.com/Marvykeys/Databel-Customer-Churn-Analysis/assets/130637591/e6d66108-72af-4bfa-ab4a-b29c2827bfdb">

##
I added the churn rate, number of customers & number of churned customers to the tooltips and visualized using the Map visual.

<img width="593" alt="DATABEL BI 11" src="https://github.com/Marvykeys/Databel-Customer-Churn-Analysis/assets/130637591/2441fb97-ee97-49dc-a74e-be66d2c7f9df">

##
I created a new column called "Demographics" with 3 categories "Senior", "Under 30" & "Other".

<img width="644" alt="DATABEL BI 12" src="https://github.com/Marvykeys/Databel-Customer-Churn-Analysis/assets/130637591/2890225d-bc9e-49e2-ae14-036d564fa1c6">

##

<img width="376" alt="DATABEL BI 13" src="https://github.com/Marvykeys/Databel-Customer-Churn-Analysis/assets/130637591/66eec313-4d3c-498a-9592-ca83e45b5ae7">

##
I created a line and stacked column chart which shows the number of customers and churn rate for every age bracket.

<img width="475" alt="DATABEL BI 14" src="https://github.com/Marvykeys/Databel-Customer-Churn-Analysis/assets/130637591/c697743c-7119-48c6-b182-2ba8ce13a963">

##
I created a bar chart which plots the average monthly phone bill charge by "Number of customers in Group".

<img width="421" alt="DATABEL BI 15" src="https://github.com/Marvykeys/Databel-Customer-Churn-Analysis/assets/130637591/b1e427a3-5df8-48ae-8a96-349319ce25d0">

##
Created a new column named "Contract Category" to help observe the difference between customers who have only yearly contracts and those having monthly contracts.

<img width="585" alt="DATABEL BI 16" src="https://github.com/Marvykeys/Databel-Customer-Churn-Analysis/assets/130637591/52f30bb6-6b8b-45fc-9f92-7ce5ff2950fc">

##
To observe how yearly and monthly contracts affect the churn rate, I use a multi-row card visualization, to clearly see the difference.

<img width="405" alt="DATABEL BI 17" src="https://github.com/Marvykeys/Databel-Customer-Churn-Analysis/assets/130637591/45c5f9f2-1249-454d-b0b9-46763cfaa6eb">

##
**KEY INSIGHT**
Customers with monthly contracts, churn more compared to cusyomers with yearly contracts.

##
In the process of investigating how the "Unlimited Data Plan" influences the churn rate, I create a column named "Grouped Consumption" which classifies the Average Monthly GB Download into "Less than 5 GB", "Between 5 & 10 GB" and "10 or more GB".
I created a Table vizualisation which displays the churn rate for customers who have the unlimted plan and for customers who don't. I also created a Clustered Bar Chart to display Churn rate by Unlimited data plan and by the 3 newly created groups.

<img width="549" alt="DATABEL BI 18" src="https://github.com/Marvykeys/Databel-Customer-Churn-Analysis/assets/130637591/dc0e8564-c6b1-433a-a46a-465318ea2c90">

##

<img width="529" alt="DATABEL BI 19" src="https://github.com/Marvykeys/Databel-Customer-Churn-Analysis/assets/130637591/e0a46916-0497-4dd0-b989-0b583124b952">

##
To better understand the international activity of customers and its relationship to churn, I created a Matrix Vizualisation which displays the churn rate by "Intl Plan" & "Intl Active" columns. To focus on a state by state basis, I changed the category of state to "State or Province".

<img width="544" alt="DATABEL BI 20" src="https://github.com/Marvykeys/Databel-Customer-Churn-Analysis/assets/130637591/769e228d-ba73-45fb-bf38-a037572fc735">

## The Dashboard Before Design


## THE FINAL INTERACTIVE DASHBOARD :art:

