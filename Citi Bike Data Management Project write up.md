Bike Rental Data Management Project

Project Overview:
This project integrates Citi Bike trip records and NOAA weather data from 2016 into a robust PostgreSQL database. The objectives were to clean and normalize the datasets, design a relational database schema, load the data using Python (SQLAlchemy and pandas), and develop analytics-ready SQL views.

Data Cleaning & Preparation:

Citi Bike Data:

Inspected monthly trip records and identified issues such as missing days, incomplete demographic data, and outliers (e.g., trip durations exceeding 24 hours).

Preserved unknown values for further analysis and created additional columns (e.g., trip duration in minutes/hours) along with flags for anomalies.

Weather Data:

Processed daily NOAA weather data, dropping columns with all null values and retaining key metrics like wind speed, precipitation, temperature, and snow.

Added binary indicators for rain and snow to support filtering in analysis.

Database Design & Implementation:

Developed an Entity Relationship Diagram and normalized the Citi Bike data by separating station and demographic details into distinct tables.

Created a date_dim table to store each day as both a date and an integer (yyyymmdd format), facilitating reliable joins between trip and weather data.

Implemented the database schema in PostgreSQL and used SQLAlchemy with pandas to insert the cleaned data.

Analytics Views:

daily_data: Provides a daily summary of rides, including date breakdowns, ride types, weather data, and flags for missing or unusual records.

monthly_data: Aggregates daily data by month, breaking down rides by user type and summarizing key weather statistics.

Additional views (e.g., for investigating late returns and trip demographics) further support detailed analytics.

This project showcases a comprehensive approach to data management—from cleaning raw data to designing a relational schema and developing SQL views that enable insightful analytics for bike rental operations.