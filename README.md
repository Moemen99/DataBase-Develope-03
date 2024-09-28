# SQL and Database Overview

## History and Variants

- **ANSI SQL**: Standardized by the American National Standards Institute (ANSI)
- **T-SQL (Transact-SQL)**: Microsoft's implementation
- **PL/SQL**: Oracle's implementation
- **SQL/PL**: IBM's implementation
- **MySQL**: Open-source implementation

## SQL Categories

### 1. DDL (Data Definition Language)
Focus: Metadata and structure

Operations:
- CREATE
- ALTER
- DROP

Examples:
```sql
CREATE TABLE
CREATE VIEW
CREATE FUNCTION
CREATE DATABASE
ALTER TABLE
DROP TABLE
```

### 2. DML (Data Manipulation Language)
Focus: Data operations

Operations:
- INSERT
- UPDATE
- DELETE
- MERGE

### 3. DCL (Data Control Language)
Focus: Security and permissions

Operations:
- GRANT
- DENY
- REVOKE

### 4. DQL (Data Query Language)
Focus: Data retrieval and analysis

Main operation:
- SELECT

Features:
- Aggregate functions
- Grouping
- UNION
- JOINS
- Subqueries

### 5. TCL (Transaction Control Language)
Focus: Transaction management

Operations:
- BEGIN TRANSACTION
- COMMIT
- ROLLBACK

## Database Objects

- Tables
- Views
- Functions
- Stored Procedures
- Indexes

## Simple Diagram

```mermaid
graph TD
    A[SQL] --> B[DDL]
    A --> C[DML]
    A --> D[DCL]
    A --> E[DQL]
    A --> F[TCL]
    B --> G[CREATE]
    B --> H[ALTER]
    B --> I[DROP]
    C --> J[INSERT]
    C --> K[UPDATE]
    C --> L[DELETE]
    C --> M[MERGE]
    D --> N[GRANT]
    D --> O[DENY]
    D --> P[REVOKE]
    E --> Q[SELECT]
    F --> R[BEGIN TRANSACTION]
    F --> S[COMMIT]
    F --> T[ROLLBACK]
```

This overview provides a structured look at SQL categories, their focuses, and main operations. It also includes a simple diagram to visualize the relationships between different SQL components.


# Creating a Database in SQL Server Management Studio (SSMS)

## Steps to Create a Database

1. **Open SQL Server Management Studio (SSMS)**
   - SSMS is a graphical tool for managing SQL Server databases

2. **Create a New Query**
   - Click on "New Query" to open a new query window

3. **Write the CREATE DATABASE command**
   ```sql
   CREATE DATABASE CompanyG02
   ```

4. **Execute the command**
   - Select the command and press F5, or click the "Execute" button

5. **Refresh the database list**
   - Right-click on "Databases" in the Object Explorer and select "Refresh"

6. **Verify the new database**
   - Look for "CompanyG02" in the list of databases
   - It will have folders for different object types (Tables, Views, etc.)

7. **Set the context to the new database**
   ```sql
   USE CompanyG02
   GO
   ```

## Visual Process Flow

```mermaid
graph TD
    A[Open SSMS] --> B[Create New Query]
    B --> C[Write CREATE DATABASE Command]
    C --> D[Execute Command]
    D --> E[Refresh Database List]
    E --> F[Verify New Database]
    F --> G[Set Database Context]
```

## Key Points

- This process uses Data Definition Language (DDL), specifically the CREATE command
- The database name (CompanyG02) can be changed as needed
- After creation, the database will be empty and ready for you to add tables and other objects
- Using the USE command ensures subsequent commands apply to your new database
