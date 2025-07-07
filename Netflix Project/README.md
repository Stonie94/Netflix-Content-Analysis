# Netflix Content Analysis 📺🔥

This project analyzes Netflix’s TV Shows and Movies using SQL and visualizes key insights with Tableau.

## 📊 Tools Used
- **Kaggle** for data source
- **DB Browser for SQLite** for SQL-based data cleaning and analysis
- **Tableau** for data visualization

## 🔍 Key Questions Answered
- What types of content does Netflix focus on?
- How has Netflix's content production changed over time?
- Which countries produce the most Netflix content?

## 🛠️ Process

### 1. Data Source
- Dataset: [Netflix Movies and TV Shows](https://www.kaggle.com/datasets/shivamb/netflix-shows)
- File: `netflix_titles.csv`

### 2. Data Cleaning in SQL
- Removed rows with missing `title`, `type`, or `country`
- Saved clean data as `netflix_clean.csv`
- Sample query:
```sql
SELECT type, COUNT(*) AS total_count
FROM netflix_clean
GROUP BY type;
