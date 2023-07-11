# Data Migration from PostgreSQL to SQLServer using PySpark


This project is to design, implement and execute an ETL pipeline using PySpark to migrate data from a PostgreSQL database to a SQL Server database. The pipeline should be designed to handle large amounts of data and ensure data integrity during the migration process. The ETL pipeline should include steps for extracting data from the PostgreSQL database, transforming the data to match the schema of the SQL Server database, and loading the data into the SQL Server database. The ultimate goal is to have the data in the SQL Server database accurately reflect the data in the PostgreSQL database with minimal data loss and minimal disruption to ongoing operations.

## Architecture
![Architecture](./src/archi.png)

## Run Locally

- Clone the project

    ```bash
    git clone https://github.com/ArkanNibrastama/Data-Migration-PostgreSQL-to-SQLServer-use-PySpark.git
    ```
- Make a database on PostgreSQL and import data from **dataset** folder
- Install all the dependencies
    ```bash
    pip install -r reuquirements.txt
    ```
- Fill the blank variable with your own data
    <br>example:
    ```python
    uid = '{YOUR USER ID ON POSTGRESQL}'
    pwd = '{YOUR PSSWORD}'
    host = 'localhost'
    port = '5432' #this is the default port
    db = '{YOUR DB NAME}'
    driver = "org.postgresql.Driver"
    url = f"jdbc:postgresql://{host}:5432/{db}?user={uid}&password={pwd}"
    ```
- Finally, you can run the program on your local computer
