# DWDM-Snowflake-project-
An end-to-end Snowflake data warehousing project demonstrating cloud DDL object creation, batch data ingestion via SnowSQL, and advanced Time Travel recovery.
# ❄️ Snowflake Data Warehousing & Data Management (DWDM)

[![Snowflake](https://img.shields.io/badge/Platform-Snowflake-29B5EF?logo=snowflake&logoColor=white)](https://snowflake.com)
[![SnowSQL](https://img.shields.io/badge/CLI-SnowSQL-orange)](https://docs.snowflake.com)
[![Status](https://img.shields.io/badge/Status-Completed-success)](https://github.com)

An end-to-end cloud data warehousing project implementing DDL/DML operations, command-line staging, batch CSV loading via SnowSQL, and Time Travel recovery.

## 🚀 Quick Navigation

| Task ID | Module Description | Key Commands / Functions Used |
| :--- | :--- | :--- |
| **Task 1** | Session & CLI Login | `snowsql`, `CURRENT_USER()`, `CURRENT_ROLE()` |
| **Task 2** | DDL Objects & DML Lifecycle | `CREATE WAREHOUSE`, `INSERT`, `UPDATE`, `DELETE` |
| **Task 3** | Batch Staging & Ingestion | `PUT`, `COPY INTO`, `LIST` |
| **Task 4** | Historical Time Travel | `AT (OFFSET => ...)` |
| **Task 5** | Disaster Recovery / Rollback | `BEFORE (STATEMENT => LAST_QUERY_ID())` |

---

## ⚙️ Environment Configuration

* **Account Identifier:** `yjemxcs-hj02840`
* **Database:** `dwdm_db`
* **Schema:** `dwdm_schema`
* **Warehouse:** `dwdm_wh` (`XSMALL`)

---

## 📂 Repository Layout

```text
├── sql_scripts/          # Step-by-step SQL execution files for all tasks
├── screenshots/          # Output validation proofs for submission report
└── README.md             # Project documentation
