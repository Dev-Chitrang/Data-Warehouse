## Project Overview

This project is a data warehousing solution that extracts, transforms, and loads data from various sources into a centralized database. The project consists of multiple layers, including bronze, silver, and gold, each serving a specific purpose in the data processing pipeline.

## Project Structure

The project is organized into the following directories:

scripts: Contains SQL scripts for creating database objects, loading data, and performing quality checks.
tests: Contains SQL scripts for testing data quality and integrity in the gold schema.
Database Schema

The project uses a three-layered database schema:

Bronze: The bronze layer is the raw data layer, where data is loaded from external sources.
Silver: The silver layer is the transformed data layer, where data is cleaned, transformed, and aggregated.
Gold: The gold layer is the presentation layer, where data is formatted for analytical purposes.
Quality Checks

The project includes quality checks to ensure data integrity, consistency, and accuracy. These checks are performed on the gold schema and cover the following aspects:

Uniqueness of surrogate keys in dimension tables
Referential integrity between fact and dimension tables
Validation of relationships in the data model from analytical purpose
Usage

To use this project, follow these steps:

Create a new database named DataWarehouse.
Run the scripts in the scripts directory to create the database objects and load the data.
Run the quality checks in the tests directory to ensure data integrity and accuracy.
Notes

This project uses SQL Server as the database management system.
The project assumes that the external data sources are in CSV format.
The project uses BULK INSERT to load data into the bronze layer.