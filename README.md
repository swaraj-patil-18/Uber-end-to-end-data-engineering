# Uber Data Analytics - End-to-End Data Engineering Project
This project focuses on performing end-to-end data engineering for Uber data analytics. The goal is to extract insights and visualize key metrics from the data using various technologies. The project involves data preparation, modeling, transformation, storage, analytics, and dashboard creation.

# Architecture

![architecture](https://github.com/swaraj-patil-18/Uber-end-to-end-data-engineering/assets/114085839/7746c2f5-084f-4856-b7de-dca3c3631151)

# Technologies Used
- Lucidchart: Used for data modeling and designing the data model.
- GCP Cloud Storage: Created a bucket and uploaded the dataset files.
- GCP Compute Engine: Created an instance to execute the project.
- Mage: Open-source data pipeline tool used for ETL processes.
- GCP BigQuery: Used for data analytics and querying.
- Looker Studio: Created interactive dashboards for data visualization.

# Project Steps
- Data Preparation: Combined and cleaned the Uber dataset files to create a unified dataset.
- Data Modeling: Designed a comprehensive data model using Lucidchart, including a fact table and dimension tables.

![Uber Data Model](https://github.com/swaraj-patil-18/Uber-end-to-end-data-engineering/assets/114085839/d3c2c909-183c-4228-8036-53f1baa33c64)

- Data Transformation: Developed Python scripts for data transformation and generating the necessary fact and dimension tables.
- Cloud Setup: Created a new project on Google Cloud Platform (GCP) and utilized GCP Cloud Storage to store the dataset securely.
- Compute Engine Provisioning: Created a GCP Compute Engine instance and installed the required software (pip, Python, Mage, pandas, google-cloud-bigquery).
- Data Pipeline: Utilized Mage to create an end-to-end data pipeline, including data loading, transformation, and exporting to GCP BigQuery.

![mage_pipeline](https://github.com/swaraj-patil-18/Uber-end-to-end-data-engineering/assets/114085839/fd690857-b944-4f31-9fcb-b880e27937d3)

- Data Analytics: Ran various queries in GCP BigQuery to extract insights, such as average fare amount by hour of the day, tip amount by payment type, top pickup --locations by the number of trips, and total trips by passenger count.
- Analytics Table Creation: Utilized SQL in GCP BigQuery to join the fact and dimension tables and create an analytics table.
- Dashboard Creation: Connected GCP BigQuery with Looker Studio to create an interactive and insightful dashboard.
- Dashboard Features: Designed a dashboard with dynamic filters, summary metrics (total revenue, record count), and a bubble map visualization of pickup locations.

![dashboard](https://github.com/swaraj-patil-18/Uber-end-to-end-data-engineering/assets/114085839/aa5f3951-edba-46c8-8ad4-b8add480e692)
- Total revenue: The total revenue generated from Uber taxi rides in New York in February 2023 is $2.9 million, indicating the financial performance for that specific month.
- Record count: The dataset contains 112,700 records, representing the total number of Uber taxi rides recorded in New York during February 2023.
- Average trip distance: The average trip distance for Uber rides in New York during February 2023 is 3.1 units, giving an idea of the typical distance covered in rides during that period.
- Average fare amount: The average fare amount per trip for Uber rides in New York during February 2023 is $17.3, providing insights into the average cost of rides during that month.
- Average tip amount: The average tip amount per trip for Uber rides in New York during February 2023 is $3.3, indicating the average level of tipping by passengers in that specific month.

Bubble map:

- Pickup locations: The map visualizes the pickup locations of Uber rides in New York during February 2023, highlighting areas with higher pickup activity.
- Tooltip: The tooltip provides the vendor ID, giving additional information about the specific vendor associated with each pickup location.
- Color dimension: The color represents the rate code name, allowing for differentiation of different rate codes observed at each pickup location.
- Size dimension: The size of the bubbles represents the tip amount, indicating the range of tip amounts received at each pickup location.
- Filtering:
The summary and map on Page 1 can be filtered by vendor ID, payment type, rate code, and trip distance to analyze specific segments or criteria within the dataset.

![dashboard_](https://github.com/swaraj-patil-18/Uber-end-to-end-data-engineering/assets/114085839/5e130e96-acf9-4f00-9296-ff8584eccba7)
- Bar chart: "Average Total Amount by Rate Code" compares the average total amount for different rate codes, providing insights into the pricing structure and revenue distribution across rate codes.
- Bar chart: "Total Amount and Passenger Count by Payment Type" presents a comparison of the total amount and passenger count for different payment types, helping understand the revenue and customer distribution by payment method.
- Bar chart: "Tip Amount by Pickup Zone" displays the tip amount for different pickup zones, highlighting zones where higher or lower tips are observed.
- Line chart: "Passenger Count by Pickup Zone" illustrates the passenger count for each pickup zone, providing insights into passenger demand trends across different zones.
These insights offer a focused view of the Uber taxi data specifically for February 2023 in New York, allowing for analysis and understanding of key metrics, trends, and patterns during that particular month.

Conclusion:
This project demonstrates proficiency in data engineering, utilizing a variety of technologies and tools. The end-to-end process includes data preparation, modeling, transformation, storage in GCP Cloud Storage, analytics in BigQuery, and visualization using Looker Studio. The project successfully delivers an interactive dashboard that allows users to explore and gain insights from the Uber dataset.
