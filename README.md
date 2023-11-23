

# 👋 Hi there, I'm Alexandre

Currently working in data engineering, this page serves as a portfolio for my personal projects.
<br>

<div align="center">

### Tools I'm familiar with:  

<br>

![image](https://img.shields.io/badge/PowerBI-F2C811?style=for-the-badge&logo=Power%20BI&logoColor=white)
![image](https://img.shields.io/badge/Microsoft%20SQL%20Server-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white)
![image](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)  
![image](https://img.shields.io/badge/Google_Cloud-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white)
![image](https://img.shields.io/badge/microsoft%20azure-0089D6?style=for-the-badge&logo=microsoft-azure&logoColor=white)
  
</div>

<div align="left">


<br>





<br>


# Data Analysis Projects :

<br>



## &ensp;&ensp;&ensp;&ensp;&ensp;Sales Analysis Report (Power BI )

<br>

The report was made from the SuperStore Global dataset, an open-source artificial sales dataset featuring the customer orders of a global ecommerce store from 2011 to 2014.  
Data was first uploaded to a Azure SQL Database then queried from Power BI.  

### Questions :
  - What is the current trends in sales?
  - Were the Sales/Profits objectives fulfilled?
  - Which category of products should we focus on?
  - Which locations should we focus on?
  - Should we optimize certain types of orders when it comes to shipping mode and order priority?
  
### Insights:
  - Sales have been trending up for the last 3 years.
  - The objectives for 2014 in Sales ($400k) and Profits ($50k) were fulfilled.
  - Tables, Copiers, Bookcases, Appliances, Machines and Phones have higher than average sales per order.
  - Copiers and Phones have higher than average profit per order, and growing.
  - The Asia-Pacific and European-Union have higher than average sales per order.
  - Products with low discounts (0 to 7% off) have higher than average sales per order.
  - Our first market is the US (~18% of sales)
  - A second group of countries form another big part of our sales (~38% of sales) : Mexico, the United Kingdom, France, Germany, India, China and Australia.
  - A third group is composed of the rest of the world (~43% of sales).
  - Our top cities for sales are mainly in North-America and Asia-Pacific markets.
  - Ship Mode : 80% of all orders are Standard or Second class orders.
  - Order priority: 88% of all orders have Medium or High priority.

### Recommendations:
  - In cooperation with the marketing team, we should focus on attracting customers interested in Tables, Copiers, Bookcases, Appliances, Machines and Phones. Within those, a more targeted push on Copiers and Phones could also significantly boost profits.
  - Within those categories, products with no discounts or low discounts should also be a focus. An ad hoc analysis on those products could detail more fine-grained characteristics if needed.
  - Because Asia-Pacific and European-Union markets have higher average sales per order, developing our activities in those regions could be beneficial.
  - We should make sure that the compliance & regulatory costs associated with operating in the rest of the world outside the US market and the second group of countries (see Insights) is not out of proportion with its sales contribution of 43%.
  - Business events should be organized our top sales cities mainly located in North America and Asia: New York City, Los Angeles, Manilla, Sydney and Jakarta.
  - We must seek to optimize the cost of processing Standard and Second class orders.
  - We must seek to optimize the cost of processing Medium and High priority orders.

<br>

*Power BI report:*
<br>

<p align="center">
  <img src="https://github.com/AlexandreGarito/pbi_demo_1/blob/main/images/demo1_0001.jpg" width="33%" />
  <img src="https://github.com/AlexandreGarito/pbi_demo_1/blob/main/images/demo1_0002.jpg" width="33%" />
  <img src="https://github.com/AlexandreGarito/pbi_demo_1/blob/main/images/demo1_0003.jpg" width="33%" />
  <img src="https://github.com/AlexandreGarito/pbi_demo_1/blob/main/images/demo1_0004.jpg" width="33%" />
  <img src="https://github.com/AlexandreGarito/pbi_demo_1/blob/main/images/demo1_0005.jpg" width="33%" />
  <img src="https://github.com/AlexandreGarito/pbi_demo_1/blob/main/images/demo1_0006.jpg" width="33%" />  
  <img src="https://github.com/AlexandreGarito/pbi_demo_1/blob/main/images/demo1_0007.jpg" width="33%" align="left"/>
</p>  

<br>  

</div>

<br>  
<br>  
<br>  
<br>  
<br>  
<br>  
<br>  
<br>
<br>
<br>  

## &ensp;&ensp;&ensp;&ensp;&ensp;Credit Risk Analysis (Power BI)

The report was made from a synthetic credit risk dataset.
Data was first uploaded to a Azure SQL Database then queried from Power BI.

### Question:

The company built a machine learning model to decide to allow or deny customers loans.
The project is for you to analyze this dataset and make sure the stakeholders and engineering teams have a more reason-based understanding of the data on which the model was trained on.
Task is the find the key factors that correlate with loan defaults.


### Insights:

After our analysis, it was found that the top factors strongly associated with loan defaults are:
- Loan Grade: G grades are associated with 80% defaults. A, B, C grades are particularly less riskier than the rest.
- Income: People with an income lower than $20k have 80% chance of defaulting. Higher income is usually associated with less defaults.
- Home ownership: Renting one's home, as well as customers falling into the 'other' category, is associated with roughly 2x more risk of default than having a mortgage or owning a home.
- Loan to Income %: The higher % of a person's income a loan accounts for, the higher the risk of default. When Loan to Income % gets higher than ~35%, the probability of defaulting hovers between 60-80% depending on the individual.
- Past Defaults History: People who defaulted in the past have roughly 2 times more risk of defaulting on their current loan.

Additional findings:
- Interest rates: the influence of interest rates on defaults is present but quite weaker than other factors.
- Loan intent: "Home improvement" is the only loan intent where the average non-defaulted loan is of higher amount than the defaulted loans. 


### Recommendations:

- According to the findings above, manual heuristic checks could be put in place to make sure that certain specific outlier decisions made by the ML model regarding accepting/denying certain loans can be reviewed by humans for confirmation (for example, the ML model decides to deny a loan with a Loan to Income % lower than 15%). Heuristics could be designed based on those 5 factors: Loan Grade, Income, Home Ownership, Loan to Income % and Past Default history.
- These heuristics must first be tested in a development environment and tuned to only send an alert on rare outlier decisions.
- The "home improvement" loans could become a category of loans where higher amounts could be allowed compared to other loan intents.

<br>

*Power BI report:*
<br>
<p align="center">
  <img src="https://github.com/AlexandreGarito/pbi_demo_2/blob/main/images/demo2_0001.jpg" width="33%" />
  <img src="https://github.com/AlexandreGarito/pbi_demo_2/blob/main/images/demo2_0002.jpg" width="33%" />
  <img src="https://github.com/AlexandreGarito/pbi_demo_2/blob/main/images/demo2_0003.jpg" width="33%" />
  <img src="https://github.com/AlexandreGarito/pbi_demo_2/blob/main/images/demo2_0004.jpg" width="33%" />
  <img src="https://github.com/AlexandreGarito/pbi_demo_2/blob/main/images/demo2_0005.jpg" width="33%" />
  <img src="https://github.com/AlexandreGarito/pbi_demo_2/blob/main/images/demo2_0006.jpg" width="33%" />
</p>  

<br>
<br>
<br>
<br>


# Data Engineering

<br>




## &ensp;&ensp;&ensp;&ensp;&ensp;GCP-hosted Micro-ETL Data Pipeline and Dashboard  

![illustration pipeline1](https://github.com/AlexandreGarito/data-pipeline-demo-1/blob/main/images/illustration%20pipeline%20demo-1.png)

<p align="center">
  <img src="https://github.com/AlexandreGarito/data-pipeline-demo-1/blob/main/images/screencapture-data-pipeline-demo-1.png" width="50%; margin: 0 auto;" />
</div>

A Python-coded and GCP-hosted micro-ETL data pipeline and interactive dashboard that displays API data using the Dash-Plotly web framework, updated daily using DevOps tools such as CI/CD, Docker, and Airflow.

GitHub repo link : https://github.com/AlexandreGarito/data-pipeline-demo-1

Tools & skills in this project :  

✅ Python (API calls, pandas, pytest unit testing, Dash-Plotly, code documentation) 

✅ Docker (managing dependencies and interactions with GCP environment)  

✅ Google Cloud Platform:  
    ✔ Cloud Build (CI/CD from GitHub repo)  
    ✔ Cloud Run (runs Docker containers)  
    ✔ Cloud Composer (Managed Airflow)  
    ✔ Secret Manager (secure access to secrets hosted in GCP)  

This project has been stopped in July 2023.

<br>
<br>

## &ensp;&ensp;&ensp;&ensp;&ensp;SQL Database Setup and Analysis of a Glassdoor Job Listings Dataset

![illustration pipeline2](https://github.com/AlexandreGarito/SQL-database-demo-2/blob/main/images/illustration%20pipeline%20demo-2.png)

<p align="center">
  <img src="https://github.com/AlexandreGarito/SQL-database-demo-2/blob/main/images/looker1.PNG" width="24.5%" />
  <img src="https://github.com/AlexandreGarito/SQL-database-demo-2/blob/main/images/looker2.PNG" width="24.5%" />
  <img src="https://github.com/AlexandreGarito/SQL-database-demo-2/blob/main/images/looker3.PNG" width="24.5%" />
  <img src="https://github.com/AlexandreGarito/SQL-database-demo-2/blob/main/images/looker4.PNG" width="24.5%" />
</p>

A practice exercise to set up and interact with a PostgreSQL database, clean and validate a large and dirty dataset with Python, as well as visualize the resulting data with BigQuery and Looker.

GitHub repo link : https://github.com/AlexandreGarito/SQL-database-demo-2  
GCP Looker dashboard link : https://lookerstudio.google.com/reporting/127231ff-fc3c-464a-a6b5-28d075df9672

<br>

Tools & skills in this project : 

  ✅ Clean and validate a large (1.5GB) and dirty (web-scraped) dataset using Python pandas  
  
  ✅ Design and create a multi-dimensional database schema using SQL  
  
  ✅ Manage compatibility issues involved in the data upload to a PostgreSQL database hosted on GCP  
  
  ✅ Perform SQL-based querying and gain insights using GCP BigQuery  
  
  ✅ Visualize data using GCP Looker (formerly Data Studio)  

<br>

<div align="center">



  
<br>
<br>

![image](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=AlexandreGarito&theme=vue)

</div>

<br>
<br>


### Hobby-related accessory skills:
- SideFX's Houdini (3D modelisation & rendering)
- Unity (real-time 3D)
- Zbrush (3D sculpting)
- Substance Designer (3D texturing)
- Adobe Photoshop (photo montage)
- Adobe Premiere (video montage)
- Stable Diffusion (image generation)
- Photogrammetry (3D modelisation from photos)
- SLA 3D printing
- NFC tags




