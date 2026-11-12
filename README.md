# 🌍 Global News & Event Intelligence Analytics

An end-to-end data analytics project that collects, cleans, integrates, and analyzes global news articles using the Currents API, Python, Pandas, and Matplotlib.

## 📌 Project Overview

This project explores news articles collected through the Currents API. It focuses on analyzing news publishers, category distributions, and source contributions through data cleaning, exploratory data analysis (EDA), and visualizations.

## 🎯 Project Objectives

- Collect real-time news article data using an API.
- Inspect and understand raw datasets.
- Identify and handle missing values and duplicate records.
- Clean and integrate data from multiple API calls.
- Analyze news categories and publishers.
- Create meaningful visualizations to communicate findings.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Data processing |
| Pandas | Data cleaning and analysis |
| NumPy | Data handling |
| Matplotlib | Data visualization |
| Requests | API integration |
| Currents API | News data source |
| Google Colab | Development environment |
| VS Code | Local development |
| Git & GitHub | Version control |

## 📡 Data Source

**Currents API**

Endpoint: `https://api.currentsapi.services/v1/latest-news`

Data collected includes:
- Article ID
- Title
- Description
- Article URL
- Author
- Image
- Language
- Category
- Source category
- Published date

The project uses two API calls with a requested page size of 20 articles per call. Duplicate articles are removed during integration.

## 🧹 Data Cleaning & Processing

The project includes:

1. Raw data inspection.
2. Missing-value identification.
3. Empty-string handling.
4. Duplicate ID and URL removal.
5. Publication date conversion to datetime.
6. Data type validation.
7. Integration of multiple API responses.
8. Final dataset validation.

## 📊 Data Visualizations

Four visualizations were created:

### 1. Top 10 News Publishers
Horizontal bar chart showing the most frequently represented publishers.

### 2. News Distribution by Category
Donut chart showing the distribution of category and location tags.

### 3. News Category Contribution by Top Publishers
Stacked bar chart comparing category labels across leading publishers.

### 4. News Source Contribution – API Call 2
Pie chart showing the contribution of different news sources in the second API response.

## 📁 Project Structure

```text
Global-News-Event-Intelligence/
│
├── data/
│   ├── raw/
│   │   ├── news_raw.csv
│   │   └── news_raw.json
│   │
│   └── processed/
│       ├── news_cleaned.csv
│       └── news_final_cleaned.csv
│
├── visualizations/
│   ├── top_10_news_publishers.png
│   ├── news_category_distribution.png
│   ├── publisher_category_comparison.png
│   └── news_source_contribution_api2.png
│
├── Global_News_Analysis.ipynb
├── global_news_analysis.py
├── .gitignore
└── README.md
```

## 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/KRISHNAPRASATH90/Global-News-Event-Intelligence.git
```

### 2. Navigate to the project directory

```bash
cd Global-News-Event-Intelligence
```

### 3. Install dependencies

```bash
pip install requests pandas numpy matplotlib
```

### 4. Run the notebook

Open `Global_News_Analysis.ipynb` in Google Colab or Jupyter Notebook.

### 5. Configure API access

Obtain an API key from Currents API and enter it when prompted by the notebook. Do not hardcode or publish your API key.

## 🔍 Key Findings

- Articles from two API calls were combined.
- Duplicate article IDs and URLs were identified and removed.
- The verified sample contained 24 unique articles after deduplication in one collection run.
- Category analysis includes both subject classifications and location-specific tags.
- Publisher and source distributions were explored through visualizations.

*Note: API results change over time. The 24-article result describes the verified sample from one run, not a permanent dataset size.*

## ⚠️ Project Limitations

- The analysis uses a small sample of API results.
- The sample covers a short collection period.
- Category labels may include geographical tags as well as subject classifications.
- Findings should not be interpreted as long-term global news trends.

## 👨‍💻 Author

**Krishna Prasath**

GitHub: [KRISHNAPRASATH90](https://github.com/KRISHNAPRASATH90)

---

⭐ If you find this project interesting, feel free to explore the repository!
