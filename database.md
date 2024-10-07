
# Overview of Database Credential GitHub Dork

This GitHub dork is designed to search for repositories that may expose sensitive database connection credentials. It aims to identify files containing various environment variables and configuration parameters related to database connections. 

## Key Parameters

The dork targets a range of database-related environment variables, including:

- **General Database Parameters**:
  - `DATABASE_HOST`
  - `DATABASE_NAME`
  - `DATABASE_PASSWORD`
  - `DATABASE_PORT`
  - `DATABASE_USER`
  - `DATABASE_USERNAME`
  - `DB_CONNECTION`
  - `DB_DATABASE`
  - `DB_HOST`
  - `DB_PASSWORD`
  - `DB_PORT`
  - `DB_PW`
  - `DB_USER`
  - `DB_USERNAME`
  
- **MongoDB**:
  - `MONGO_URI`
  - `MONGODB_URI`
  
- **MySQL**:
  - `MYSQL_HOST`
  - `MYSQL_USER`
  - `MYSQL_PASSWORD`
  - `MYSQL_DATABASE`
  
- **PostgreSQL**:
  - `POSTGRES_HOST`
  - `POSTGRES_USER`
  - `POSTGRES_PASSWORD`
  - `POSTGRES_DB`
  
- **SQL Server**:
  - `SQL_SERVER`
  - `SQL_USER`
  - `SQL_PASSWORD`
  - `SQL_DATABASE`
  - `SQL_HOST`
  
- **Amazon RDS**:
  - `RDS_HOSTNAME`
  - `RDS_DB_NAME`
  - `RDS_USERNAME`
  - `RDS_PASSWORD`
  
- **Redis**:
  - `REDIS_HOST`
  - `REDIS_PASSWORD`
  - `REDIS_PORT`
  
- **Oracle**:
  - `oracle_host`
  - `oracle_user`
  - `oracle_password`
  - `oracle_sid`
  
- **Cassandra**:
  - `CASSANDRA_USERNAME`
  - `CASSANDRA_PASSWORD`
  
- **Elasticsearch**:
  - `elasticsearch_host`
  - `elasticsearch_username`
  - `elasticsearch_password`
  
- **DB2**:
  - `DB2_DATABASE`
  - `DB2_USER`
  - `DB2_PASSWORD`

## Purpose

The primary purpose of this dork is to discover misconfigured repositories where developers might have accidentally committed sensitive database credentials. Exposed credentials can lead to unauthorized access, data breaches, and other security risks.

## Usage

To use this dork effectively:
1. Enter the dork into the GitHub search bar.
2. Analyze the search results for any repositories that may contain sensitive information.
3. Follow responsible disclosure practices if you discover exposed credentials.

## Conclusion

Using this GitHub dork can help security researchers, developers, and ethical hackers identify potential security vulnerabilities related to database configurations. It is crucial to handle any findings responsibly and report them to the appropriate parties.


```bash
(DATABASE_HOST= OR DATABASE_NAME= OR DATABASE_PASSWORD= OR DATABASE_PORT= OR DATABASE_USER= OR DATABASE_USERNAME= 
 OR databaseEnabled= OR datadog_api_key= OR datadog_app_key= OR DB_CONNECTION= OR DB_DATABASE= 
 OR DB_HOST= OR DB_PASSWORD= OR DB_PORT= OR DB_PW= OR DB_USER= OR DB_USERNAME= 
 OR MONGO_URI= OR MONGODB_URI= OR MYSQL_HOST= OR MYSQL_USER= OR MYSQL_PASSWORD= OR MYSQL_DATABASE= 
 OR POSTGRES_HOST= OR POSTGRES_USER= OR POSTGRES_PASSWORD= OR POSTGRES_DB= OR SQL_SERVER= 
 OR SQL_USER= OR SQL_PASSWORD= OR SQL_DATABASE= OR SQL_HOST= OR RDS_HOSTNAME= OR RDS_DB_NAME= 
 OR RDS_USERNAME= OR RDS_PASSWORD= OR REDIS_HOST= OR REDIS_PASSWORD= OR REDIS_PORT= 
 OR oracle_host= OR oracle_user= OR oracle_password= OR oracle_sid= OR CASSANDRA_USERNAME= 
 OR CASSANDRA_PASSWORD= OR elasticsearch_host= OR elasticsearch_username= OR elasticsearch_password= 
 OR DB2_DATABASE= OR DB2_USER= OR DB2_PASSWORD=)
```
