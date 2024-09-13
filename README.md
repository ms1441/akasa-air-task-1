# Akasa Air Data Analysis Report

This README provides an overview of the Akasa Air Data Analysis Report, detailing the steps taken in data cleaning and normalization, insights derived from data analysis, and recommendations based on these insights. Additionally, key visualizations illustrating the findings are included in the report.

## Summary of Data Cleaning and Normalization Steps

1. **Load the Data**: The dataset was imported into a Pandas DataFrame for analysis.
   
2. **Handling Missing Values**: Missing values in the `DelayMinutes` column were filled with the median value to maintain data integrity.
   
3. **Remove Duplicates**: Duplicate entries were removed using `df.drop_duplicates()` to ensure clean data.
   
4. **Corrected Time Inconsistencies**: `DepartureTime` and `ArrivalTime` were converted to datetime objects. Adjustments were made to `ArrivalTime` if it occurred earlier than `DepartureTime` to correct inconsistencies.
   
5. **Standardize Formats**: Dates in `DepartureDate` and `ArrivalDate` were standardized to `YYYY-MM-DD` format, and times were converted to a 24-hour format.
   
6. **Calculate Flight Duration**: A `FlightDuration` column was added by calculating the difference between `ArrivalTime` and `DepartureTime`.

## Insights Derived from the Data Analysis

1. **Average Delays**: The analysis revealed an average delay of 17 minutes across all flights, with United Airlines experiencing the most delays.
   
2. **Peak Delay Times**: Delays were found to be more frequent during peak hours, notably between 5 PM and 8 PM.
   
3. **Customer Feedback**: Passengers frequently highlighted punctuality and staff behavior as critical factors in their feedback.

## Recommendations Based on the Analysis

1. **Operational Adjustments**: It is recommended to reschedule flights during peak delay times to less busy periods to enhance on-time performance.
   
2. **Customer Service Training**: Staff training programs should be enhanced, focusing on improving customer interaction and punctuality.
   
3. **Feedback Mechanism**: Implementing regular surveys to capture passenger feedback can help in making necessary adjustments and improving service quality.
   
4. **Route Optimization**: Routes with higher delays should be investigated for possible scheduling adjustments or additional resources.

## Visualizations Illustrating the Key Findings

The report includes visualizations that effectively illustrate the key findings, helping to provide a clearer understanding of the data insights and supporting the recommendations.

---

This README file serves as a concise guide to understanding the contents and findings of the Akasa Air Data Analysis Report. For further details, please refer to the full PDF report.
