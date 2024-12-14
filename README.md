<h1 align="center">City of Vancouver DAP Design for Vancouver Parks</h1>
<p align="center">
Abdulgafar Abdulrasaq Tosin (2210112) <br>
University Canada West<br>
BUSI 653, Section 07<br>
Instructor: Mahmood Mortazavi Dehkordi<br>
</p>

___

# Project Description: Descriptive Analysis of City Parks
In this assignment I will be describing the details of the City of Vancouver project mainly about the Data Analytic Platform (DAP) implementation (the datasets used and the various derivations and DAP design using the datasets I selected. For this assignment I used the website [City of Vancouver Open Data Portal](https://opendata.vancouver.ca/explore/dataset/parks/table/?dataChart=eyJxdWVyaWVzIjpbeyJjaGFydHMiOlt7InR5cGUiOiJjb2x1bW4iLCJmdW5jIjoiU1VNIiwieUF4aXMiOiJoZWN0YXJlIiwic2NpZW50aWZpY0Rpc3BsYXkiOnRydWUsImNvbG9yIjoiIzAyNzlCMSJ9XSwieEF4aXMiOiJuZWlnaGJvdXJob29kbmFtZSIsIm1heHBvaW50cyI6NTAsInNvcnQiOiIiLCJzZXJpZXNCcmVha2Rvd25UaW1lc2NhbGUiOiIiLCJjb25maWciOnsiZGF0YXNldCI6InBhcmtzIiwib3B0aW9ucyI6e319fV0sInRpbWVzY2FsZSI6IiIsImRpc3BsYXlMZWdlbmQiOnRydWUsImFsaWduTW9udGgiOnRydWV9&location=11,49.22852,-123.12388) for getting some open source available datasets for various segments related to the Vancouver City operations.

## Project Title: Understanding  City Parks
The primary need of this project is to conduct a descriptive and Exploratory Analysis of Vancouver City Parks based on the datasets taken from [City of Vancouver Open Data Portal](https://opendata.vancouver.ca/explore/dataset/parks/table/?dataChart=eyJxdWVyaWVzIjpbeyJjaGFydHMiOlt7InR5cGUiOiJjb2x1bW4iLCJmdW5jIjoiU1VNIiwieUF4aXMiOiJoZWN0YXJlIiwic2NpZW50aWZpY0Rpc3BsYXkiOnRydWUsImNvbG9yIjoiIzAyNzlCMSJ9XSwieEF4aXMiOiJuZWlnaGJvdXJob29kbmFtZSIsIm1heHBvaW50cyI6NTAsInNvcnQiOiIiLCJzZXJpZXNCcmVha2Rvd25UaW1lc2NhbGUiOiIiLCJjb25maWciOnsiZGF0YXNldCI6InBhcmtzIiwib3B0aW9ucyI6e319fV0sInRpbWVzY2FsZSI6IiIsImRpc3BsYXlMZWdlbmQiOnRydWUsImFsaWduTW9udGgiOnRydWV9&location=11,49.22852,-123.12388). The hope with this question was to gain insight into how accessible washrooms are in city parks and perhaps assess how well a park is outfitted to meet the needs of a visitor.
## Project Objective:
* Data Analysis Process (DAP) is the methodical way of viewing data and discovering useful insights or patterns, helping to make decisions.
* It takes the form of steps including data collection, profiling, data cleaning, transformation, visualization, and ending with actionable conclusions.
* The dataset taken by me is about the  “Parks” segment of the “Parts, Recreation and Pets” module of the Vancouver city portal.
* In this we have key features like the ‘Park Name’, ‘Special Features’, ‘Facilities’, ‘Washroom’,  ‘Address’ and other details.
* From this, the main objective is to do descriptive analysis on “What is the count of parks in each ‘Neighbourhood’ of Vancouver recorded with a Washroom facility?” using this, we can further analyze the population segmentation around these areas and other details.
* We aldo do an exploratory analysis on question of “What is the count of Official Parks in each Neighbourhood?” to further analyse and find any trends available.
## Datasets
* There is one datasets which I will be using here.
* The dataset is **"Parks"**, it contains information about the Vancouver Board of Parks and Recreation maintains over 220 parks and 40 major facilities throughout the City of Vancouver.
* This dataset provides information of the parks and facilities that are available in them. Additional details are found in related datasets:
  * Parks washrooms
  * Parks facilities
  * Parks special features
* This data set contain the information of data columns like:
  * ParkID: Id issued for each park
  * Name: Name issued for each park
  * Official: '1' if official and '0' if not
  * Advisories: 'N' if no and 'Y' if yes
  * Special Features: 'N' if no and 'Y' if yes
  * Facilities:'N' if no and 'Y' if yes
  * Washroom:'N' if no and 'Y' if yes
  * Street Number: The street number of park
  * Street Name: The name of the street of park
  * EW Street: The east-west street name of park
  * NS Street: The north-south street name of park
  * Neighbourhood  Name: The neighbourhood name of park
  * Neighbourhood url: The url pointing ti the Neighbourhood of park
  * Hectare: The are of park in hectares
  * GoogleMap Dest: The google destination coordinates of park
  * [2024-parks-infomration.xlsx](https://github.com/user-attachments/files/18117379/2024-parks-infomration.xlsx) contains the information of this dataset.
## Methodology:
* The process of DAP designing and implementation is complex.
* This involves 3 stages namely:
### Part 1 - [Descryptive Analysis of Vancouver city Parks](https://abdul-busi653.github.io/Descriptive-Analysis-of-Vancouver-City-Parks/)
* The dataset taken by me is about the  “Parks” segment of the “Parts, Recreation and Pets” module of the Vancouver city portal.
* In this we have key features like the ‘Park Name’, ‘Special Features’, ‘Facilities’, ‘Washroom’,  ‘Address’ and other details.
* From this, the main objective the teammate has taken to do analysis is “What is the count of parks in each ‘Neighbourhood’ of Vancouver recorded with a Washroom facility?”.
* Using this, we can further analyze the population segmentation around these areas and other details.
* Data Questions (Metric)
First we need to gather a few details below:
•	Total count of parks in each neighborhood
•	Total count of parks in each neighborhood with washroom facility
•	Find the ration of the parks with washroom to the total count of parks in each neighbourhood respectively.
#### Data Questions (Metric)
First we need to gather a few details below:
* Total count of parks in each neighborhood
* Total count of parks in each neighborhood with washroom facility
* Find the ration of the parks with washroom to the total count of parks in each neighbourhood respectively.<br>
Below I mentioned the 4 step process involved in the DAP design related to the descriptive question posted above analysis (highlighted and underlined).<br>
We are going to use the AWS services like S3, Glue, Glue DataBrew as per our need to store the results and other details of the project.
#### Dap Design
![image 000](https://github.com/user-attachments/assets/4121d110-4bfd-4b89-bfa0-93d88a47e082)<br>
The above image displays the DAP design we are implementing for the descyptive analysis.
#### Descriptive  Question for Analysis
![image 001](https://github.com/user-attachments/assets/f33d2ea7-0f6b-4f7a-9238-27cf63efb456)<br>
The above images displays the descryptive analysis of our DAP model.
#### Step 1: Data Ingestion
This step explains about the Data ingestion into AWS Environment
#### Step 2: Data Profiling
This step explain the data profiling in the AWS environment.
#### Step 3: Data Cleaning 
This step explaing the Data cleaning done using the AWS DataBrew service.
#### Step 4: Data Pipeline Design 
This step explain the process of designing a ETL pipeline to transform raw data into structured data.
### Part 2 - [Exploratory Analysis of Vancouver city Parks](https://abdul-busi653.github.io/Exploratory-Analysis-of-Vancouver-City-Parks/)
* The dataset taken by me is about the  “Parks” segment of the “Parts, Recreation and Pets” module of the Vancouver city portal.
* In this we have key features like the ‘Park Name’, ‘Special Features’, ‘Facilities’, ‘Washroom’,  ‘Address’ and other details.
* From this, the main objective the teammate has taken to do analysis is “What is the count of parks in each ‘Neighbourhood’ of Vancouver recorded with a Washroom facility?”.
* Using this, we can further analyze the population segmentation around these areas and other details.
* Data Questions (Metric)
First we need to gather a few details below:
•	Total count of parks in each neighborhood
•	Total count of parks in each neighborhood with washroom facility
•	Find the ration of the parks with washroom to the total count of parks in each neighbourhood respectively.
#### Data Questions (Metric)
First we need to gather a few details below:
* Total count of parks in each neighborhood
* Total count of parks in each neighborhood with washroom facility
* Find the ration of the parks with washroom to the total count of parks in each neighbourhood respectively.<br>
Below I mentioned the 4 step process involved in the DAP design related to the descriptive question posted above analysis (highlighted and underlined).<br>
We are going to use the AWS services like S3, Glue, Glue DataBrew as per our need to store the results and other details of the project.
#### Dap Design
![image 000](https://github.com/user-attachments/assets/4121d110-4bfd-4b89-bfa0-93d88a47e082)<br>
The above image displays the DAP design we are implementing for the descyptive analysis.
#### Descriptive  Question for Analysis
![image 002](https://github.com/user-attachments/assets/b9db6e00-d7c1-453e-bf1f-67058be627b7)<br>
The above images displays the exploratory analysis of our DAP model.
#### Step 1: Data Ingestion
This step explains about the Data ingestion into AWS Environment
#### Step 2: Data Profiling
This step explain the data profiling in the AWS environment.
#### Step 3: Data Cleaning 
This step explaing the Data cleaning done using the AWS DataBrew service.
#### Step 4: Data Pipeline Design 
This step explain the process of designing a ETL pipeline to transform raw data into structured data.
### Part 3 - [DAP Advanced Procedures of Data Enriching, Protection, Governance and Observability](https://abdul-busi653.github.io/Vancouver-City-Project-Advanced-DAP-Procedures/)
This step involves the 4 major steps namely:
#### Step 1: Data Enriching
Data enrichment in data management is all about augmenting raw data with relevant context and information that provides more value for analytical purposes.<br>
This cleanses the data and transforms it to provide meaningful insights, which again are useful to make better decisions. 
#### Step 2: Data Protection
In AWS, one can protect sensitive data by encrypting it to protect its confidentiality and security.<br>
AWS KMS provides a centralized control point for encryption keys so that users can create, manage, and use them to perform encryption and decryption automatically and with control over access to the keys using IAM policies.<br>
It improves data protection to be compliant with security standards.
#### Step 3: Data Governance 
Data governance is the discipline for establishing, implementing, and maintaining the structure for data across the enterprise.<br>
This means defining data quality, privacy, security, and compliance with regulatory standard policies, roles, and procedures.<br>
Starting with creating access controls, auditing data usage, enabling encryption capabilities for your data, and using features such as AWS Glue Data Catalog for managing and cataloging metadata, data governance in AWS is a combination of setup, management, and maintenance.
#### Step 4: Data Observability 
The real-time performance and health of the data platform in the Parks, Recreation, and Pets (PRP) domain is visualized using the data observability dashboard displayed in AWS CloudWatch.<br>
A customized dashboard tracks key metrics, including bucket storage utilization, number of objects in buckets, and associated estimated charges, giving a full view of data operations. 
