# Cryptocurrency Relational Database Analytics & SQL Pipeline

A reference implementation of an end-to-end data pipeline that models cryptocurrency transactions using a normalized SQLite database and extracts advanced analytical metrics via SQL.

## Features
- **3NF Schema:** Strict referential integrity, foreign keys, and check constraints.
- **Secure Ingestion:** Parameterized DML queries (`executemany`) to prevent SQL injection.
- **Advanced OLAP:** Window functions (`SUM() OVER`) for running totals and conditional aggregations (`CASE WHEN`) for risk metrics.
- **Optimization:** B-Tree indexes to speed up multi-table JOIN operations.

## Repository Structure
- `Crypto_SQL_Analytics_Pipeline.ipynb` – Main Jupyter Notebook with DDL, DML, and analytical queries.
- `crypto_analytics_queries.sql` – Standalone SQL queries.
- `requirements.txt` – Python dependencies.

## Quick Start

### 1. Clone, set up environment, and install dependencies:
```bash
git clone https://github.com/your-username/crypto-sql-analytics.git
cd crypto-sql-analytics
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
pip install -r requirements.txt
```

### 2. Run the Notebook:
```bash
jupyter lab
```
Open the notebook and select **Kernel -> Restart & Run All**.
