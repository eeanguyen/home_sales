# Home Sales Analysis

This project analyzes home sales data using PySpark and SparkSQL. It explores various aspects of home sales, such as average home prices by year, room configurations, and specific features, leveraging Spark's processing capabilities for big data analysis.

## Project Structure

- **Installation and Setup**: Sets up the environment for PySpark, including downloading and configuring Spark and Java.
- **Data Loading**: Loads the home sales dataset from an AWS S3 bucket into a PySpark DataFrame.
- **Data Analysis**: Uses SparkSQL queries to perform the following analyses:
  - **Average Price by Bedroom Count**: Calculates the average price of four-bedroom homes by year.
  - **Price by Build Year**: Finds the average price for homes built in different years with specific bedroom and bathroom counts.
  - **Feature-Specific Pricing**: Examines the average price of homes with three bedrooms, three bathrooms, two floors, and a minimum square footage.
  - **Price by View Rating**: Analyzes average prices based on the view rating, filtering for homes priced above $350,000 and measuring query execution time.

## Usage

1. **Setup the Environment**: Run the cells to install Spark and Java.
2. **Load Data**: The dataset is fetched directly from an AWS S3 bucket.
3. **Execute Queries**: Each analysis section runs a SparkSQL query to gather insights into various pricing metrics based on home attributes.
4. **Caching**: To optimize query performance, cache the DataFrame for repeated queries.

## Dependencies

- Python
- PySpark
- Java (OpenJDK 11)

## Key Features

- Efficient data handling with PySpark for large datasets.
- SQL-style querying with SparkSQL for structured analysis.
- Performance measurement for queries, demonstrating Spark's capability for handling substantial data volumes.
