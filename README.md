# SQL_DatabaseQueries_for_CrimeAnalysis
This set of SQL queries is designed for crime analysis, exploring relationships and patterns within a criminal justice database. The queries focus on officers, criminals, sentences, appeals, and crime charges.

Below is a brief summary of each query:

- Officers with High Crime Involvement:
Retrieves the last and first names of officers who have a crime involvement count greater than the average count.
Utilizes a right join between crime_officers and officers tables.
- Criminals with No Pending Cases:
Fetches the last and first names of criminals with 'N' status (indicating no pending cases).
Applies a right join between crimes and criminals tables.
- Appeals with Swift Processing:
Selects records from the appeals table where the time gap between hearing and filing dates is less than the average gap.
Utilizes date calculations and the AVG function.
- Probation Officers Handling Multiple Cases:
Retrieves probation officers with a case count equal to or greater than the average case count.
Applies a right join between sentences and prob_officers tables.
- Most Appealed Crimes:
Fetches crime records that are the most appealed, based on the highest count of appeals for a crime.
Involves nested subqueries to identify the most appealed crime_id.
- Crime Charges with Financial Deviations:
Selects records from crime_charges where the fine amount is below the average and the amount paid is above the average.
Utilizes subqueries and conditional filtering.
- Criminals Associated with a Specific Crime:
Retrieves distinct records from the criminals table for individuals associated with a specific crime_id (10091).
Utilizes a right join between criminals and crimes tables.
- Query 7 Revisited (Que: 7):
Selects last and first names from the criminals table for individuals linked to crimes that share the same crime_code as the crime with id 10091.
Involves nested subqueries to identify relevant crime_ids.
# Note:

These queries are tailored for a specific database schema and might need adjustments for different datasets.
The README provides an overview, and users should refer to the actual SQL script for detailed implementation.
