# DWDM-Snowflake-project-
An end-to-end Snowflake data warehousing project demonstrating cloud DDL object creation, batch data ingestion via SnowSQL, and advanced Time Travel recovery.
# Snowflake Data Warehousing & Data Management (DWDM) Project

An end-to-end Snowflake data warehousing project demonstrating cloud DDL object creation, batch data ingestion via SnowSQL, and advanced Time Travel recovery.

## Project Overview

This repository contains SQL implementation scripts and verification records for the DWDM tutorial assignment, executed on a Snowflake cloud data warehouse instance via SnowSQL and the web console.

## Tasks & Implementation Details

### Task 1: SnowSQL Connection & Session Verification
* Established a secure command-line session using SnowSQL.
* Verified user context, role, active warehouse, database, and schema settings.

### Task 2: DDL Object Creation & DML Operations
* Created core enterprise objects: Warehouse (`XSMALL`), Database, Schema, and Internal Stage.
* Created the `student_records` table and performed full lifecycle DML operations (`INSERT`, `SELECT`, `UPDATE`, and `DELETE`) on 10 student records.

### Task 3: Batch Data Loading via SnowSQL
* Prepared a structured CSV dataset containing multi-record student information.
* Staged the local file to Snowflake using the internal `PUT` command and loaded data into the target table via `COPY INTO`.

### Task 4: Snowflake Time Travel (Historical Querying)
* Executed data modifications (`UPDATE` and `DELETE`) on a demonstration table.
* Queried historical table states prior to the modifications using the `AT (OFFSET => ...)` clause.

### Task 5: Data Recovery Using Time Travel
* Simulated accidental data loss by purging a table using `DELETE`.
* Restored the lost data using the `BEFORE (STATEMENT => LAST_QUERY_ID())` recovery pattern.

## Repository Structure
* `sql_scripts/`: Contains step-by-step SQL scripts for all tasks.
* `screenshots/`: Output validation screenshots for each task stage.
