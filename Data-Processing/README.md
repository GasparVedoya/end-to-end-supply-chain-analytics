# Data Processing Layer

## Overview

This folder contains the foundational database design and setup for the End-to-End Supply Chain Analysis project.

The objective of this layer is to transform raw transactional data into a structured, normalized relational database that supports analytical modeling and reporting.

This represents the data engineering component of the project.

---

## Database Design

The database is structured using relational modeling principles, including:

- Parent and child table relationships
- Primary and foreign key constraints
- Index creation for performance optimization
- Normalization to reduce redundancy

Core entities include:

- Vendors
- Products (Brands / Items)
- Stores
- Transactions / Invoices

The schema is designed to support:

- Supplier-level aggregation
- Item-level profitability analysis
- Lead time tracking
- Store-level performance metrics

---

## Contents

### `optimization.sql`

This file contains:

- CREATE TABLE statements
- Primary and foreign key definitions
- Index creation
- Data insertion logic

The script initializes the full relational structure required for downstream analytics.

---

## Design Considerations

- Ensured referential integrity through foreign keys
- Structured tables to allow multi-level aggregation (Vendor → Item → Store)
- Created indexes to support efficient query performance
- Separated structural logic from analytical logic for modularity

---

## Role in Overall Project

This layer enables:

- Supplier segmentation modeling
- Inventory optimization calculations
- Profitability analysis
- Store performance analytics

Without this structured foundation, advanced analytics would not be reliable or scalable.

