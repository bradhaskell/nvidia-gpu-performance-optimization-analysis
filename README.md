# NVIDIA GPU Performance Optimization Analysis

## 🛠 Tech Stack
- Python (pandas, SQLAlchemy)
- SQL (PostgreSQL)
- AWS RDS (MySQL + PostgreSQL)
- GitHub Actions
- PopSQL
- Jupyter Notebook
- draw.io (Data pipeline diagrams)

## 🎯 Project Objective
This project supports NVIDIA’s data team by identifying the key product specifications that influence GPU pricing and performance. By combining real product specification data and benchmarked gaming performance, this analysis provides actionable insights into product-market fit and consumer value perception. The end-to-end pipeline demonstrates the ability to extract, transform, and visualize critical business data—skills essential for technical data roles.

## 💼 Job Description
The job posting was for a Data Analyst position at NVIDIA focused on product and market performance. The role emphasized SQL analysis, data visualization, and business problem-solving using real-world hardware and sales data. This project mirrors those requirements by analyzing GPU specs from an API, scraping benchmark performance metrics, and deriving insights that inform pricing and product positioning strategies.

[📄 Job Description PDF](proposal/Job_Description.pdf)

## 📊 Data

### Sources
- [TomsHardware GPU Benchmark Database (Web Scraped)](https://www.tomshardware.com/reviews/gpu-hierarchy,4388.html)
- [Kaggle GPU Specs API Dataset](https://www.kaggle.com/datasets/alanjo/graphics-card-full-specs)

### Characteristics
- **API Source:** Product specs (e.g., memory, GPU chip, clock speed)
- **Web Source:** FPS benchmark performance (e.g., 1080p, 1440p, 4K Ultra), MSRP prices

## 📓 Notebooks / Python Scripts

| File | Purpose |
|------|---------|
| `notebooks/Kaggle_API_Extract_Load_Raw.ipynb` | Extracts and loads raw GPU specs from Kaggle |
| `notebooks/Web_Scrape_Extract_Load_Raw.ipynb` | Extracts and loads benchmark performance data |
| `notebooks/Kaggle_API_SQL_Analysis.ipynb` | Performs descriptive and diagnostic SQL analysis on specs |
| `notebooks/Web_Scrape_SQL_Analysis.ipynb` | Performs descriptive and diagnostic SQL analysis on benchmark performance |
| `elt/basket_craft_website_sessions_extract_load_raw.py` | (Lesson 10 Quiz) Python pipeline for MySQL → Postgres ETL |
| `models/` | dbt transformations: staging and warehouse models for the quiz pipeline |

## 🔮 Future Improvements
- Normalize tables across sources to enable easier readability and usage of data
- Incorporate dbt to help transform and clean the data
- Incorporate time-series price trends to evaluate depreciation or value retention
- Include customer purchases to further analyze successes of each GPU
