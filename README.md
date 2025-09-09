Data Analysis & Dashboards

Modern data analysis, visualization & interactive dashboards using Python, SQL, Power BI, Tableau & Excel.

Table of Contents

Overview

Projects & Files

How to run / open each project

Suggested Python environment / requirements

Repository structure

Contributing

License

Contact

Overview

This repository collects hands-on data analysis projects and interactive dashboards built with a mix of tools commonly used in industry: Python (Pandas, NumPy, Matplotlib, Seaborn, Plotly), SQL (PostgreSQL), Power BI, Tableau, and Excel. The projects demonstrate data cleaning, exploratory data analysis (EDA), visualization, and dashboarding techniques with reproducible workflows.

Use this repo to learn practical techniques, inspect examples, and reuse components for your own data projects.

Projects & Files

Below are the main files / projects in this repository and a short description of each.

Excel - LOOKUP, INDEX, MATCH, SUMIFS.xlsx

A hands-on workbook that demonstrates advanced Excel lookup and aggregation techniques: VLOOKUP/HLOOKUP, INDEX+MATCH, and SUMIFS with practical examples. Great for quick reference and for building lightweight Excel-based reports.

Key features: worked examples, sample datasets inside workbook, formula explanations.

Excel - Sales Performance Dashboard.xlsx

An interactive sales dashboard built in Excel using pivot tables, slicers, charts, and KPI tiles to monitor sales performance (revenue, growth, top products/regions, salesperson rankings).

Open in: Microsoft Excel (recommended Excel 2016+). If the workbook uses macros, enable them only from trusted sources.

PostgreSQL-BI-CHALLENGE/

A folder containing SQL scripts and query solutions for a BI-style challenge using PostgreSQL. Includes schema definitions, example queries, and may include sample data and notes.

Contents (example): schema.sql, load_data.sql, challenge_queries.sql, README within the folder (if present).

Python - Movie Industry EDA Project.ipynb

A Jupyter Notebook performing Exploratory Data Analysis on the movie industry dataset. Typical workflow includes data loading, cleaning, feature extraction, visualizations (ratings, revenue, genre trends), and short insights.

Libraries used: pandas, numpy, matplotlib, seaborn, plotly (optional), scikit-learn (optional for preprocessing).

How to run: open with Jupyter Notebook / JupyterLab / VS Code and run cells.

SQL - Data Cleaning.sql

A standalone SQL script containing data cleaning steps implemented in SQL: deduplication, data type conversions, null handling, normalization and sample transformations — written for PostgreSQL compatibility.

How to run: execute with psql or any PostgreSQL client against your target database.

project-visualization_powerbi.pbix

A Power BI Desktop file containing interactive visuals and a report layout created from the project dataset. Visuals include slicers, time-series charts, KPI cards and drill-through pages.

Open in: Power BI Desktop (or publish to Power BI Service).

How to run / open each project

Clone the repo

git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>

Python Notebook

Create virtual environment (optional):

python -m venv .venv
source .venv/bin/activate  # macOS / Linux
.\.venv\Scripts\activate  # Windows

Install dependencies (see requirements.txt suggestion below):

pip install -r requirements.txt

Launch Jupyter:

jupyter lab   # or jupyter notebook

Open Python - Movie Industry EDA Project.ipynb and run cells.

SQL scripts / PostgreSQL

Create database and run SQL scripts with psql:

createdb bi_challenge
psql -d bi_challenge -f PostgreSQL-BI-CHALLENGE/schema.sql
psql -d bi_challenge -f PostgreSQL-BI-CHALLENGE/load_data.sql
psql -d bi_challenge -f "SQL - Data Cleaning.sql"

Update connection details in scripts if needed.

Power BI

Open project-visualization_powerbi.pbix with Power BI Desktop.

If data sources are disconnected, reconnect or update the data source settings.

Excel files

Open Excel workbooks directly in Microsoft Excel.

Check for embedded data, or re-link to CSV / database sources if necessary.

Suggested Python environment / requirements

Create a requirements.txt (example):

pandas
numpy
matplotlib
seaborn
plotly
jupyterlab
scikit-learn
ipython
openpyxl
psycopg2-binary

Adjust versions as needed.

Repository structure (recommended)
README.md
requirements.txt
Python - Movie Industry EDA Project.ipynb
SQL - Data Cleaning.sql
project-visualization_powerbi.pbix
Excel - LOOKUP, INDEX, MATCH, SUMIFS.xlsx
Excel - Sales Performance Dashboard.xlsx
PostgreSQL-BI-CHALLENGE/
  ├─ schema.sql
  ├─ load_data.sql
  ├─ challenge_queries.sql
  └─ data/ (optional)
Contributing

Contributions and improvements are welcome. If you want to add datasets, notebook enhancements, or new dashboards:

Fork the repo

Create a new branch

Open a Pull Request describing your changes

Please follow clear commit messages and include reproducible steps for any added project.

License

This repository is released under the MIT License by default. Replace with your preferred license if needed.

Contact

Author: Hassan Hatami

For questions or dataset requests, open an issue or create a pull request on this repository.
