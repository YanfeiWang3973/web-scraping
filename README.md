# Web Scraping & Real Estate Modeling 🏡

This project focuses on end-to-end data analysis of real estate listings scraped from Craigslist Toronto (Real Estate section). The goal was to explore listing patterns across the Greater Toronto Area (GTA), including price, square footage, and bedroom count, and to create an interactive visual report for insights.

---

## 🛠️ Project Pipeline

### 1. **Web Scraping**
- Source: [https://toronto.craigslist.org/search/rea](https://toronto.craigslist.org/search/rea)
- Used `requests` and `BeautifulSoup` to extract property titles, prices, locations, links, square footage, bedroom/bathroom count, and addresses.
- JavaScript-rendered data was excluded.

### 2. **Data Cleaning & Structuring**
- Cleaned the raw HTML output into a structured Pandas DataFrame
- Removed inconsistent or missing values
- Standardized text and numerical fields (e.g., city names, sqft, price format)

### 3. **Exploratory Analysis & Modeling**
- Created calculated fields such as `Price per Sqft`
- Explored outliers and filtered unrealistic entries
- Exported final dataset to CSV

### 4. **Dashboard Visualization (Tableau)**
- Designed an interactive Tableau dashboard to showcase:
  - Listings by Bedroom Count
  - Price vs Sqft scatterplot
  - Avg Price per Sqft by City (bar chart and bubble map)
  - Map visualization of listing hotspots
  - Global filters (Price, Sqft, Bedrooms, Bathrooms, City)
  - link: https://public.tableau.com/app/profile/yan.fei.wang/viz/craigslistrealestatereport/Dashboard2?publish=yes 

---

## 📁 Files Included
| File | Description |
|------|-------------|
| `real_estate_data_scraping.ipynb` | Web scraping script (Python + BeautifulSoup) |
| `real_estate_data_analysis(clean).ipynb` | Data cleaning, transformation & export |
| `craigslist_analysis_data(clean).csv` | Final cleaned dataset used for dashboard |
| `craigslist_dashboard.png` | Screenshot of the final Tableau dashboard |
| `README.md` | This documentation file |

---

## 📊 Dashboard Highlights
- Visualizes market trends in listing size, price, and city-based value
- Interactive filters enable deep-dive exploration
- Clear map representation of pricing clusters by city

> *Built entirely using open-source tools and Tableau Public.*

---

## 🚀 Tools Used
- Python (Pandas, BeautifulSoup)
- Google Colab
- Tableau Public
- GitHub

---


