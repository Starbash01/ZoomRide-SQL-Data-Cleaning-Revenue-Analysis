# ZoomRide_SQL
Analyzed and cleaned ZoomRide’s messy trip data using MySQL. The project identified duplicate records, corrected inconsistent city names, handled missing fares, and analyzed revenue by city, month, and vehicle type. SQL queries were also used to identify top customers and customers who had never booked a trip.

## Structured Query Language Queries
- <a href="https://onecompiler.com/mysql/455p9v8ra"> Feel free to explore and interact with this project. You're welcome to use it as a reference, adapt it to your own database, and experiment with different analyses. I hope it provides useful insights and serves as a helpful resource for your own learning and projects.

If you find this project valuable, consider giving it a ⭐ and sharing your feedback or suggestions. Your support and contributions are always appreciated!
 </a>

 ### KPI Questions
 * How many trips are recorded in the database?
 * Which city generates the highest revenue?
 * Which month has the highest number of rides?
 * Which month generates the highest revenue?
 * Which vehicle type generates the highest revenue?
 * What is the average fare by city?
 * How many completed trips have missing fares?
 * Which customers spend the most on completed trips?
 * How many customers have never booked a trip?
 * How many duplicate trip records exist?

### Processes Followed
1. Data Exploration: Examined the customers, drivers, and trips tables and their relationships.
2. Data Quality Check: Used COUNT, GROUP BY, and HAVING to identify unusual city names, duplicates, and missing fares.
3. Data Cleaning: Used TRIM() to remove unnecessary spaces and UPDATE statements to standardize city names.
4. Duplicate Removal: Identified duplicate trips using customer, driver, date, and fare, then deleted the later duplicate records.
5. Data Validation: Re-ran the city count and total row queries to confirm that the cleaning process worked.
6. Revenue Analysis: Used SUM(), AVG(), COUNT(), GROUP BY, and ORDER BY to analyze revenue.
7. Time Analysis: Used DATE_FORMAT() to analyze trips and revenue by month.
8. Table Joins: Joined trips with drivers to analyze revenue by vehicle type and customers with trips to identify customer activity.
9. Customer Analysis: Identified customers with no trips and ranked customers by total completed-trip spending.

### Outcome
* Reduced the dataset from 300 to 298 rows after removing duplicate records.
* Standardized inconsistent city names.
* Identified 9 completed trips with missing fares without inventing replacement values.
* Identified Lagos as the highest-revenue city, generating ₦218,890.
* Identified December 2025 as the month with the most rides, with 31 trips.
* Identified Economy vehicles as the highest-revenue vehicle type, generating ₦262,550.
* Identified customers who had never booked a trip.
* Identified the top customers based on total completed-trip spending.

## Structured Query Language
