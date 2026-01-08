# PubMed HIV Publications Analysis (2020)

## Overview

This project analyzes HIV-related publications indexed in **PubMed** between **January 1, 2020 and August 30, 2020**. Using Python, we scraped article metadata, cleaned and structured the data, stored it in an SQLite database, and produced statistical summaries and visualizations to examine publication trends over time.

The project was developed from October 2023 to December 2023.

## Authors

* Aaron Niecestro
* Jack Mittenthal
* Yukuan Pan
* Jung Yang

## Project Workflow

1. **Data Collection (Web Scraping)**

   * Scraped PubMed for articles containing the keyword **“HIV”** in the abstract
   * Extracted titles, abstracts, author lists, and publication dates

2. **Data Cleaning**

   * Filtered publications to the specified time window
   * Checked for missing values and formatted date fields
   * Exported cleaned data to CSV

3. **Database Creation**

   * Built an SQLite database from the cleaned dataset
   * Enabled querying publications by author name

4. **Data Analysis & Visualization**

   * Monthly publication counts
   * Summary statistics
   * Bar chart and time-series trend analysis

## Technologies Used

* **Python**
* **Jupyter Notebook**
* **SQLite**
* **Libraries**:

  * BioPython
  * pandas
  * numpy
  * matplotlib
  * plotly
  * BeautifulSoup
  * sqlite3

## Key Results

* **Total publications:** 5,540
* **Average per month:** ~693
* **Highest month:** July (770 publications)
* **Lowest month:** January (529 publications)

Publication activity increased early in the year, remained consistently above average through mid-2020, and declined slightly toward August.

## How to Run the Project

### 1. Setup

* Install **Anaconda**
* Launch **Jupyter Notebook**
* Install required packages:

```bash
pip install biopython pandas numpy matplotlib plotly beautifulsoup4
```

### 2. Run the Scraper

> **Warning:** Scraping PubMed can take up to **2 hours**

* Open `PubMed_Scraper.ipynb`
* Run all cells to generate `pubmed_capstone.csv`

### 3. Clean the Data

* Open `Data_Cleaning.ipynb`
* Run all cells to produce `pubmed_capstone2.csv`

### 4. Build the Database

* Open `SQLite_Database.ipynb`
* Query publications by author name

### 5. Visualize Results

* Open `Visualization.ipynb`
* Generate bar charts, summary tables, and trend lines

## Notes

* Scraper performance depends on system resources
* Disable sleep mode while scraping
* Ensure a stable internet connection

## License

This project is for **academic and educational purposes only**.
