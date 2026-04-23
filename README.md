# Liquor Database Management System

A relational database system for **liquor inventory and sales tracking** across Iowa state retail stores — built on PostgreSQL with a fully normalized 8-table schema, complex joins, and analytical queries.

## Problem Statement

Retailers struggle with overstocking, stockouts, and poor demand visibility. This system provides a structured, queryable database to track in-demand products, manage warehouse space, and fulfill customer demand efficiently.

## Dataset

- **Source:** Iowa state liquor sales records
- **Contents:** Product name, type, price, quantity, store location, county-level sales data
- **Scope:** Individual containers and packages sold across multiple Iowa counties

## Schema Design

8 tables with primary keys, foreign keys, and referential integrity:

```
Stores --< Sales >-- Products
              |
           Categories
              |
         Vendors / Suppliers
```

- Fully normalized (3NF)
- Primary and foreign key constraints on all tables
- Designed and built using **PostgreSQL**

## Key Queries

- Top-selling products by county and season
- Inventory turnover rate per store
- Revenue by product category
- Supplier performance analysis

## Tech Stack

`PostgreSQL` · `SQL` · `Relational Database Design` · `ERD Modeling`

## Setup

```bash
git clone https://github.com/mitalildeshpande/Liquor-Database-Management-System.git
psql -U postgres -f schema.sql
psql -U postgres -f data.sql
```