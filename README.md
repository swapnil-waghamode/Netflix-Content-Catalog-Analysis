# Netflix Content Catalog Analysis

A data analysis project exploring Netflix's content catalog — covering data cleaning, feature engineering, exploratory analysis, and anomaly detection.

## Business Scenario
Netflix management wants insights into country-wise content production, popular directors, content ratings, and genre popularity.

## Dataset
[netflix_titles.csv](https://raw.githubusercontent.com/allenkong221/netflix-titles-dataset/refs/heads/main/netflix_titles.csv) — 6,234 titles (Movies & TV Shows) with metadata like director, cast, country, date added, release year, rating, and duration.

## Contents
- **Part 1 – Data Understanding:** Load data, descriptive stats, unique value counts.
- **Part 2 – Data Cleaning:** Remove duplicates, handle nulls (fill director/cast/country, drop rows missing date_added/rating).
- **Part 3 – Feature Engineering:** Build `movies_df` with `year_added`, `month_added`, `content_age`, `movie_duration_minutes`.
- **Part 4 – Exploratory Data Analysis:** Dashboard with 6 charts — ratings countplot, duration distplot, top 5 years bar plot, top 10 directors bar plot, content age vs duration scatter plot, content age by rating boxplot.
- **Part 5 – Anomaly Detection:** Monthly content addition trend with Z-score-based outlier detection and visualization.

## Requirements
```
pandas
numpy
matplotlib
seaborn
scipy
```

## Usage
Open `Netflix_Content_Analysis.ipynb` in Jupyter and run all cells.

## Key Findings
- Nov 2019 and Dec 2019 stand out as anomalous months with unusually high content additions (|Z-score| > 2).
