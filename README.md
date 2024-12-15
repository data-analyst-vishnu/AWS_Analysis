# Data-analysis_AWS

## Comprehensive Data Analysis for Traffic Department Efficiency

### Project Title
Exploring The Operational Efficiency for Traffic Department

### Objective
The primary goal is to determine the closure rate of service requests and identify operational inefficiencies and areas for improvement within the Traffic Department.

### Dataset
The dataset used in this project, identified as `3-1-1-service-requests`, was sourced from Open Data Vancouver. It comprises a variety of service requests handled by the City of Vancouver's Traffic Department, providing a detailed record of each request including identifiers, closure rates, and the types of requests made. This dataset is part of the city's initiative to enhance transparency and operational efficiency in government services.

![Dataset Overview](https://github.com/user-attachments/assets/15f8b99f-2280-490c-b594-966f76e00c5f)

### Methodology
#### Data Ingestion
- **Collection**: Data is sourced from Open Data Vancouver, consolidating service request records.
- **Storage**: Data is ingested and stored in an AWS S3 bucketnamed "van-eng-traffic-service-raw-vishnu", ensuring high availability and security.

#### Data Profiling and Cleaning
- **Profiling**: Using AWS Glue DataBrew, the data is profiled to identify missing values and anomalies.
- **Cleaning**: Cleansing tasks include formatting timestamps correctly, removing unnecessary whitespace, and standardizing data entries.

#### Analytical Processes
- **Descriptive Analysis**: Calculation of key metrics such as average closure rate and the distribution of request types.

  ![image](https://github.com/user-attachments/assets/5a938e2d-2e17-4af6-9150-e4a9996283a8)

  ![image](https://github.com/user-attachments/assets/ca576582-8437-4e03-90d0-3b7d68931898)



- **Exploratory Analysis**: Analysing  the influence of various communication channels  on the closure rates of customer inquiries , highlighting differences across departments."
  
  ![image](https://github.com/user-attachments/assets/5dc2592b-cd90-43bd-a6a3-c20f92d97139)

  ![image](https://github.com/user-attachments/assets/bdee8219-e4db-48db-bde5-9312b8648d27)




### AWS Services:
- **S3**: 
  - **Usage**: S3 is utilized to store both historical and real-time service request data collected from Open Data Vancouver.
  - **Example Use**: This storage includes comprehensive data attributes like timestamps, request types, status updates, and detailed information regarding the closure of requests through various communication channels.

- **Glue**: 
  - **Usage**: AWS Glue is employed to organize and prepare the dataset for analysis.
  - **Example Use**: It automates the ETL processes by cataloging the data as it’s ingested from the Open Data platform, creating schemas to match the dataset structure, and transforming data by cleaning and validating it to ensure analytical accuracy and consistency.

- **DataBrew**: 
  - **Usage**: Used for data cleaning and preparation without the need for coding.
  - **Example Use**: DataBrew manages tasks such as removing duplicates, correcting data entries (e.g., adjusting date formats, standardizing text fields for request types), and filtering incomplete records to enhance data quality for more reliable analysis.

- **Athena**: 
  - **Usage**: Athena facilitates querying the prepared data stored in S3 using SQL.
  - **Example Use**: Perform SQL queries to analyze the closure rates associated with different communication channels (such as phone, email, web portal, and mobile app) across various departments. Queries might focus on comparing the effectiveness of digital versus traditional communication channels in resolving service requests, enabling insights into operational efficiencies.

### Deliverables
- **Visualizations**: Graphs and charts that highlight key insights from the data.
- **AWS Architecture Diagrams**: Visual representations of the data workflow and service architecture.
- **Final Analysis Report**: A comprehensive document detailing the findings, methodology, and recommendations for improving the Traffic Department's efficiency.

- **Insights on Communication Channels**:
  - **Observation**: The variance in closure rates across communication channels (phone, email, web, mobile app) indicates distinct impacts on customer inquiries and sales.
  - **Action Required**: Department-specific analysis is essential to identify pain points and optimize channel efficiency. 
  - **Strategies for Improvement**:
    - Enhance mobile user experience.
    - Reduce response times on phone lines.
    - Increase utilization of the Web for customer engagement.
  - **Outcome**: These tailored communication strategies are expected to significantly improve inquiry resolution and boost sales performance.



