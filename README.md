# Vancouver Parks Data Analytics Projects

This repository showcases a series of data analytics projects focused on Vancouver parks data, utilizing AWS services to process, analyze, and visualize park usage patterns and trends. The projects span exploratory data analysis, diagnostic analysis, quality control measures, and advanced data wrangling. Each project aims to uncover valuable insights for city planners and decision-makers, while ensuring secure and efficient data management through the use of AWS technologies.

---

## **1. Exploratory Data Analysis (EDA) on Vancouver Parks Data**

### **Project Title**: Exploring Vancouver Parks: An EDA Approach

### **Objective**:  
Perform exploratory data analysis (EDA) on the Vancouver parks dataset to uncover trends, patterns, and relationships related to park usage, amenities, and geographic locations, while maintaining data security and ensuring efficient data processing.

### **Dataset**:
- **Park ID**: Unique identifier for each park
- **Park Name**: Name of the park
- **Location**: Geographic coordinates (latitude, longitude)
- **Size**: Area of the park in hectares
- **Amenities**: List of facilities (e.g., playgrounds, walking trails, sports fields)
- **Visitor Count**: Monthly or yearly visitor data
- **Type**: Park type (e.g., community, regional, nature park)

### **Methodology**:

1. **Data Collection and Security**:
   - Store raw data in **AWS S3**, encrypt it using **AWS Key Management Service (KMS)** for secure storage.
   - Use **AWS CloudTrail** to track data access and monitor activity for compliance and security.

2. **Data Cleaning and Transformation**:
   - Use **AWS Glue DataBrew** for interactive and visual data wrangling, cleaning, and normalizing raw data.
   - Utilize **AWS Glue** ETL jobs to perform advanced transformations like aggregations, parsing dates, and managing missing values.

3. **Querying and Analysis**:
   - Use **Amazon Athena** to perform SQL-based queries on the cleaned dataset for interactive data exploration.

4. **Visualization and Insights**:
   - Use **Amazon SageMaker** to build and train models for generating interactive visualizations and reports.
   - Create dashboards in **Amazon QuickSight** for real-time data insights and monitoring.

5. **Security and Compliance**:
   - Use **AWS CloudTrail** to track data access and actions taken on the dataset, ensuring secure handling and access control.

### **Deliverables**:
- EDA report containing detailed insights, trends, and relationships.
- Visualizations of park features, usage patterns, and trends through interactive dashboards in **SageMaker** and **QuickSight**.
- A comprehensive documentation of data wrangling, transformation, and visualization processes.

### **Additional Tools**:
- **Amazon QuickSight** for interactive and real-time data visualization.
- **AWS Lake Formation** for secure data lakes and centralized access to datasets.

---

## **2. Descriptive Analysis of Park Visitor Patterns**

### **Project Title**: Analyzing Visitor Trends at Vancouver Parks

### **Objective**:  
Perform a descriptive analysis of visitor trends at Vancouver parks, examining factors such as park type, amenities, time of year, and geographic location, to uncover patterns that could inform city planning and resource allocation.

### **Dataset**:
- **Visitor Count**: Daily, weekly, or monthly visitor data.
- **Park Features**: Information on park amenities and features.
- **Weather Data**: Data on temperature, precipitation, and seasonal trends.
- **Event Data**: Information on local events that may influence park visitation.

### **Methodology**:

1. **Data Integration and Preparation**:
   - Combine visitor data with weather and event data stored in **AWS S3** using **AWS Glue** ETL for data integration.
   - Secure data using **KMS** encryption and monitor access using **AWS CloudTrail**.

2. **Descriptive Statistics**:
   - Use **Amazon Athena** to perform SQL queries to calculate average visitors, identify peak seasons, and detect patterns by park type, location, and weather conditions.

3. **Visualization**:
   - Create visualizations using **Amazon SageMaker** for static and dynamic reports, highlighting seasonal trends and correlations between park features and visitor numbers.
   - Use **QuickSight** to generate real-time dashboards displaying key metrics, such as the average number of visitors per park and the impact of events on visitation.

4. **Insights**:
   - Identify key factors influencing park visitation trends, including weather patterns, special events, and park-specific amenities.

### **Deliverables**:
- A descriptive analysis report with clear visualizations showing visitor trends.
- Dashboards in **QuickSight** summarizing key visitor insights and park features.

### **Additional Tools**:
- **AWS Data Exchange** to acquire third-party datasets, such as detailed weather data or demographic information.
- **AWS Step Functions** to automate the data integration process for real-time analysis.

---

## **3. Diagnostic Analysis of Visitor Decline in Parks**

### **Project Title**: Diagnosing Visitor Decline in Vancouver Parks

### **Objective**:  
Identify the underlying causes of declining visitor numbers at certain parks and provide recommendations for improvements in park amenities, marketing strategies, or other factors affecting park usage.

### **Dataset**:
- **Visitor Count**: Historical visitor data for affected parks.
- **Park Features**: Data on amenities and features available at each park.
- **External Factors**: Data on economic conditions, local events, transportation changes, or nearby developments.

### **Methodology**:

1. **Data Wrangling and Enrichment**:
   - Use **AWS Glue DataBrew** to clean and transform the raw data.
   - Enrich data by adding external datasets, such as event schedules and transportation accessibility, using APIs.

2. **Diagnostic Analytics**:
   - Perform regression analysis and correlation analysis in **Amazon SageMaker** to identify factors influencing the decline in park visitation.
   - Query data using **Athena** to uncover historical patterns in visitation and correlate them with changes in park features or external events.

3. **Actionable Insights**:
   - Provide actionable recommendations for addressing visitor decline, such as modifying park amenities, improving marketing efforts, or organizing local events.
   - Generate visual reports and dashboards in **SageMaker** and **QuickSight** to present findings.

### **Deliverables**:
- Diagnostic report identifying the root causes of visitor decline.
- Dashboards and visualizations summarizing key findings and recommendations for improvement.

### **Additional Tools**:
- **Amazon Rekognition** for analyzing user-generated images (e.g., park photos shared on social media).
- **AWS Lambda** to automate triggers and notifications based on certain visitor behavior patterns (e.g., sudden decline in visitors).

---

## **4. Data Quality Control for Vancouver Parks Data**

### **Project Title**: Data Quality Control for Vancouver Parks Data

### **Objective**:  
Establish a robust data quality control framework to ensure the accuracy, completeness, and consistency of the Vancouver parks dataset, making it ready for further analysis and decision-making.

### **Methodology**:

1. **Data Profiling**:
   - Use **AWS Glue DataBrew** to perform an initial analysis of the dataset, identifying anomalies, missing values, and outliers.
   - Validate data consistency and ensure all entries conform to expected formats.

2. **Data Cleansing**:
   - Remove duplicates and apply standardization techniques using **AWS Glue** ETL.
   - Use **Amazon SageMaker** for applying validation rules and detecting anomalies in the data.

3. **Monitoring and Automation**:
   - Set up automated data validation and monitoring workflows using **AWS CloudWatch** and **AWS Step Functions**.
   - Use **CloudTrail** for tracking data modifications and access logs to ensure secure handling of data.

4. **Data Quality Reporting**:
   - Generate periodic data quality reports to monitor the health of the dataset.

### **Deliverables**:
- A comprehensive data quality control framework with validation rules and monitoring setups.
- Regular data quality reports and dashboards in **QuickSight** for tracking data health over time.

### **Additional Tools**:
- **Amazon EMR** for large-scale data processing and quality control.
- **AWS CodePipeline** for automating data preparation workflows.

---

## **5. Data Wrangling for Vancouver Parks Analytics**

### **Project Title**: Data Wrangling for Vancouver Parks Analytics

### **Objective**:  
Perform extensive data wrangling to prepare the raw Vancouver parks data for analysis. This process includes cleaning, transformation, and structuring the data for downstream analytical use.

### **Dataset**:
- **Park Data**: Raw data on parks, locations, amenities, and visitor information.
- **Weather Data**: Raw temperature and weather data from external sources.
- **Event Data**: Information about local events affecting park visitation.

### **Methodology**:

1. **Data Collection**:
   - Gather raw datasets from multiple sources, including public datasets and external APIs, and store them in **AWS S3**.

2. **Data Profiling**:
   - Profile the data using **AWS Glue DataBrew** to identify missing values, outliers, and inconsistencies.

3. **Data Transformation**:
   - Clean the data by handling missing values, removing duplicates, and standardizing formats.
   - Apply transformation logic using **AWS Glue** ETL jobs to create calculated fields and aggregate data.

4. **Data Consolidation**:
   - Merge data from different sources (e.g., weather data, park data) into a unified dataset using **AWS Glue**.

5. **Data Validation**:
   - Use **Jupyter notebooks** on **AWS SageMaker** to validate the transformed data and ensure it’s ready for analysis.

### **Deliverables**:
- A cleaned and structured dataset ready for detailed analysis.
- A detailed report documenting the steps taken in the data wrangling process.

### **Additional Tools**:
- **AWS Glue** for ETL processing and data wrangling.
- **Amazon Athena** for querying and aggregating the final dataset for analysis.

---

## **Additional Resources**

For further details on the steps taken in each project, along with images, screenshots, and additional insights, please refer to the following PDFs:

- **[CC - Part 1](path-to-CC-Part-1-pdf-file)**: Detailed breakdown of each step, including data collection, cleaning, and analysis methods.
- **[CC - Part 2](path-to-CC-Part-2-pdf-file)**: Visualizations, results, and additional insights into the data analysis processes.

---

### **Conclusion**

These projects demonstrate the power of AWS in managing, processing, and analyzing large datasets. By leveraging a variety of AWS services, including **S3**, **Glue**, **Athena**, **SageMaker**, **QuickSight**, and **KMS**, these analytics projects provide actionable insights into park management, resource allocation, and urban planning in Vancouver. This repository not only focuses on data science techniques but also emphasizes secure and scalable data management practices.

Feel free to explore the code and detailed reports in this repository. Contributions and feedback are always welcome!
