# Bike Rental Data Management
The project demonstrates how to create a relational database with analytics-ready views by integrating Citi Bike trip records with weather data.

## Project Overview
__Data Preparation:__ Inspecting and cleaning datasets from Citi Bike and NOAA.

__Database Design:__ Developing a relational database schema in PostgreSQL.

__Data Insertion:__ Implementing the database and inserting the cleaned data.

__Analytics Views:__ Creating flexible SQL views for advanced analytics.

## Folder Structure
__bike-rental.ipynb:__
Jupyter Notebook for preparing and cleaning the data.

__tables.sql:__
SQL script containing commands to create the database tables.

__views.sql:__
SQL script with queries to create analytics-ready views.

## data/

newark_airport_2016.csv: NOAA weather data from Newark Airport for 2016.

JC-2016xx-citibike-tripdata.csv: Twelve monthly Citi Bike data files from Jersey City (replace "xx" with the corresponding month).

## data-dictionaries/

citibike.pdf: Details on the Citi Bike datasets (source: Citi Bike website).

weather.pdf: Details on the NOAA weather data (source: NOAA website).
