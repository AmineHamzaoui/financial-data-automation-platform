# 📈 Automated Stock Market Intelligence Pipeline  
### **Enterprise-Grade Financial Data Automation, Enrichment & Analytics Infrastructure**

---

## 1. Introduction

This repository provides a full, end-to-end **Stock Market Intelligence System** designed for:

- Analysts  
- Financial engineers  
- Quantitative researchers  
- Decision-makers  

…who require **high-quality, deeply enriched, continuously updated financial datasets**.

The pipeline automates the complete lifecycle of financial market data:

- Acquisition of raw market, corporate, and technical data  
- Data normalization, cleaning, and structuring  
- Extensive feature engineering (technical, financial, structural, performance)  
- Storage in an analytics-ready SQL Data Warehouse  
- Automated reporting via Power BI  
- Daily & quarterly refresh via scheduling (Cron + SQL Server Agent)

Built for **accuracy, scalability, reliability, and enterprise workflows**, the system ensures that business users always access the **latest, cleanest, most enriched dataset** — with zero manual work.

---

## 2. What This System Provides

### ✔ **Market Data Exploration**
- Daily OHLC data  
- Corporate actions (splits, dividends, capital gains)  
- Volatility measures  
- Rolling highs & lows  

### ✔ **Feature-Rich Technical Dataset**
- 200+ TA indicators  
- Candlestick patterns  
- Swing structure analysis  
- Market structure shifts  
- Liquidity sweeps  
- Fair value gaps  
- Order blocks  

### ✔ **Fully Enriched Fundamental Dataset**
- Revenue  
- Net income  
- EPS  
- Free cash flow  
- ROE, ROA, ROIC  
- Debt structure  
- Liquidity ratios  

### ✔ **Performance & Growth Analytics**
- YTD, 1Y, 3Y, 5Y performance  
- TTM growth  
- Multi-year rolling growth  
- Factor-style financial metrics  

### ✔ **Power BI Automation**
- Fully refreshed dashboard every day  
- Integrated via Power BI Gateway  
- Connected to SQL Data Warehouse  

### ✔ **SQL Warehouse Integration**
- Structured fact & dimension modeling  
- Daily enrich & historical preservation  
- Ideal for BI, quant models, portfolio analytics, risk engines  

---

## 3. Libraries Used + Documentation Links

Below are the core technologies powering the system—each chosen for reliability and industry adoption.

---

### 🔹 **Python Core Libraries**

| Library | Purpose | Docs |
|--------|---------|------|
| **pandas** | Cleaning, merging, feature engineering, time-series | https://pandas.pydata.org/docs/ |
| **numpy** | Vectorized numerics for financial math | https://numpy.org/doc/ |
| **requests** | API & HTTP data extraction | https://requests.readthedocs.io/ |
| **json / datetime** | Data parsing & time logic | https://docs.python.org/3/library/json.html |

---

### 🔹 **Web Extraction Libraries**

| Library | Purpose | Docs |
|--------|---------|------|
| **Scrapy** | Large-scale, robust web extraction | https://docs.scrapy.org/en/latest/ |
| **Selenium** | Dynamic JS rendering | https://www.selenium.dev/documentation/ |
| **undetected-chromedriver** | Bypass Cloudflare/anti-bot | https://github.com/ultrafunkamsterdam/undetected-chromedriver |
| **BeautifulSoup (bs4)** | HTML parsing | https://www.crummy.com/software/BeautifulSoup/bs4/doc/ |

---

### 🔹 **Financial & Technical Indicator Libraries**

| Library | Purpose | Docs |
|--------|---------|------|
| **yfinance** | OHLCV + dividends + financials | https://aroussi.com/post/python-yahoo-finance |
| **TA-Lib** | 200+ indicators (RSI, ATR, MACD…) | https://mrjbq7.github.io/ta-lib/ |
| **pandas_ta** | Extra TA indicators | https://github.com/twopirllc/pandas-ta |

---

### 🔹 **Database & ETL Libraries**

| Library | Purpose | Docs |
|--------|---------|------|
| **pyodbc** | SQL Server integration | https://github.com/mkleehammer/pyodbc/wiki |
| **SQLAlchemy** | ORM + high-level SQL | https://docs.sqlalchemy.org/ |
| **fastparquet / pyarrow** | High-performance Parquet storage | https://fastparquet.readthedocs.io/ |

---

### 🔹 **Visualization**

- **matplotlib** — QA charts, diagnostics  
  https://matplotlib.org/stable/contents.html  
- **plotly** — (optional) interactive financial charts  
  https://plotly.com/python/

---

### 🔹 **Automation & Scheduling**

| Tool | Purpose | Docs |
|------|----------|------|
| **WSL** | Linux environment for Cron automation | https://learn.microsoft.com/windows/wsl/ |
| **Cron** | Daily scripts and tasks | https://wiki.archlinux.org/title/Cron |
| **SQL Server Agent** | Daily ETL + SSIS automation | https://learn.microsoft.com/sql/ssms/agent/sql-server-agent |
| **Power BI Gateway** | Auto-refresh cloud dashboards | https://learn.microsoft.com/power-bi/connect-data/service-gateway-onprem |

---

## 4. SSIS Data Warehouse Overview

The SQL Data Warehouse uses a standard analytic model:

- **Company Dimension** (industry, sector, ticker)  
- **Date Dimension**  
- **Fact Table** for all financial/market features  
- **Raw staging layer** for ingestion  

SSIS packages:

- Clean + standardize data  
- Enforce business logic  
- Perform surrogate key lookups  
- Manage controlled inserts/updates  

Daily scheduling is managed by **SQL Server Agent**.

---

## 5. End-User Perspective: Why This System Matters

This platform is designed for **people who need reliable data**, not pipeline builders.

### ✔ Always-Fresh

- Prices update daily  
- Financial statements update quarterly  
- Power BI refreshes automatically  

### ✔ Clean, Unified Dataset  
No missing tickers  
No duplicated rows  
No corrupted financials  
No broken merges  

### ✔ Advanced Feature Engineering  
- Technical indicators  
- Candlestick patterns  
- SMC  
- Fundamental ratios  
- Multi-year performance  

### ✔ Enterprise Reliability  
- ETL via SSIS  
- Scheduling via SQL Server Agent + Cron  
- Reporting via Power BI Gateway  

Everything is fully automated.


