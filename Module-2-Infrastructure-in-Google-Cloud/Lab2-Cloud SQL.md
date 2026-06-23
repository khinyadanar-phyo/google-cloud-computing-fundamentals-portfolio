# Cloud SQL for MySQL – Google Cloud Lab

## Introduction

Cloud SQL is a fully managed relational database service provided by Google Cloud that simplifies the setup, maintenance, management, and administration of databases. It supports popular database engines such as MySQL, PostgreSQL, and SQL Server. In this lab, a Cloud SQL for MySQL instance was created and configured, followed by the creation of a database and the insertion of sample data using the MySQL client in Cloud Shell.

## Objectives

* Create a Cloud SQL for MySQL instance in Google Cloud.
* Connect to the database instance using Cloud Shell.
* Create a new database within the Cloud SQL instance.
* Create tables and insert sample records.
* Retrieve and verify stored data using SQL queries.
* Gain practical experience in managing cloud-hosted relational databases.

## Key Steps Performed

### 1. Cloud SQL Instance Creation

* Opened the Cloud SQL service from the Google Cloud Console.
* Selected MySQL as the database engine.
* Configured the instance using the Development preset.
* Set the database version to MySQL 8.
* Created a Cloud SQL instance named **myinstance**.

### 2. Connecting to the Database

Opened Cloud Shell from the Google Cloud Console.
Connected to the Cloud SQL instance using the MySQL client.
Authenticated using the root user credentials.

### 3. Database Creation

Created a new database named **guestbook** within the Cloud SQL instance.
Verified successful database creation.

### 4. Table Creation and Data Insertion

Selected the guestbook database.
Created a table named **entries** with fields for guest name, content, and entry ID.
Inserted sample records into the table using SQL commands.

### 5. Data Retrieval

Executed SQL queries to retrieve records from the table.
Verified that the inserted data was stored successfully in the database.

## Results

A Cloud SQL for MySQL instance was successfully created and configured. A database named **guestbook** was created, and a table was populated with sample guest entries. SQL queries were used to retrieve the stored records, confirming successful database creation, data insertion, and database connectivity. The lab demonstrated the fundamental processes involved in deploying and managing a relational database using Google Cloud SQL.

## Conclusion

This lab provided hands-on experience with Google Cloud SQL for MySQL. The activities covered instance creation, database configuration, table management, data insertion, and data retrieval. The exercise highlighted how Cloud SQL simplifies database administration while providing a scalable and reliable platform for cloud-based applications.
