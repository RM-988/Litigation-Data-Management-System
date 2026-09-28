# Litigation Data Management System

A beginner-friendly portfolio project that simulates organizing fictional litigation case records. It demonstrates data validation, filtering, summary reporting, and CSV export using Python.

> **Disclaimer:** This is a learning project using fictional sample data. It is not a legal case-management or e-discovery platform and does not use Relativity.

## Features
- Load fictional case records from CSV
- Validate required fields and identify duplicate case IDs
- Filter cases by status or client
- Summarize open and closed cases
- Export a cleaned CSV report

## Tech stack
- Python 3
- Standard library: `csv`, `argparse`, `collections`

## Setup
Python 3.9+ recommended. No third-party packages are required.

```bash
git clone https://github.com/YOUR-USERNAME/Litigation-Data-Management-System.git
cd Litigation-Data-Management-System
python src/litigation_manager.py --help
```

## Usage
Show all cases:
```bash
python src/litigation_manager.py --input data/sample_cases.csv --list
```

Filter by status:
```bash
python src/litigation_manager.py --input data/sample_cases.csv --status Open
```

Filter by client:
```bash
python src/litigation_manager.py --input data/sample_cases.csv --client "Northstar Foods"
```

Show summary:
```bash
python src/litigation_manager.py --input data/sample_cases.csv --summary
```

Validate records:
```bash
python src/litigation_manager.py --input data/sample_cases.csv --validate
```

Export validated records:
```bash
python src/litigation_manager.py --input data/sample_cases.csv --export cleaned_cases.csv
```

## Data fields
- `case_id`: unique fictional case identifier
- `client`: fictional client name
- `case_name`: fictional matter name
- `status`: Open or Closed
- `opened_date`: date in YYYY-MM-DD format
- `document_count`: non-negative integer

## Learning outcomes
- Reading and writing CSV files
- Basic data quality checks
- Filtering and grouping records
- Building a command-line Python utility
- Documenting a reproducible workflow

## Future improvements
- Add a SQL database
- Add Excel/Power BI reporting
- Add user permissions and audit logs
- Add a simple web interface
