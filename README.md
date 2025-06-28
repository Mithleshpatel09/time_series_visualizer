# 📈 Time Series Visualizer

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=matplotlib)
![Seaborn](https://img.shields.io/badge/Seaborn-005571?style=for-the-badge&logo=seaborn)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy)

---

### 📊 Overview

This project analyzes and visualizes **time series data** of daily page views from the freeCodeCamp.org forum. It identifies trends, seasonality, and outliers in web traffic data, providing insights into user engagement over time.

---

### 💡 Problem Statement

The goal is to visualize daily page views data to observe and represent the following:
* Overall trend of page views over several years.
* Monthly and yearly seasonality patterns.
* Data cleaning to filter out extreme outliers.

---

### 📈 Data Source

* **Source:** [fcc-forum-pageviews.csv](https://raw.githubusercontent.com/freeCodeCamp/boilerplate-time-series-visualizer/main/fcc-forum-pageviews.csv) (FreeCodeCamp's Data Analysis with Python certification)
* **Description:** Contains daily page views data for the freeCodeCamp.org forum from May 2016 to December 2019.

---

### 🚀 Methodology

1.  **Data Loading & Cleaning:**
    * Reading the `fcc-forum-pageviews.csv` dataset, parsing 'date' column, and setting it as index.
    * Filtering out outliers by removing the top 2.5% and bottom 2.5% of page views.
2.  **Line Plot Generation:**
    * Creating a line plot showing daily page views over the entire period.
    * Highlighting the overall trend of forum page views.
3.  **Bar Plot Generation:**
    * Resampling data to monthly average page views.
    * Creating a bar plot to show average daily page views for each month, grouped by year, illustrating yearly trends and monthly seasonality.
4.  **Box Plots Generation:**
    * Creating two box plots (Year-wise and Month-wise) to visualize the distribution of page views per year and per month, clearly showing trend and seasonality.

---

### 🎯 Results & Visualizations

*(**Important:** Yahan par apne bane hue `line_plot.png`, `bar_plot.png`, aur `box_plot.png` ke screenshots daalna.)*

* **Daily Page Views (Line Plot - `line_plot.png`):**
    * ![Daily Page Views Line Plot](line_plot.png)
    * *This plot displays the raw daily page view data, illustrating the long-term upward trend of forum engagement.*

* **Average Page Views by Month (Bar Plot - `bar_plot.png`):**
    * ![Average Page Views Bar Plot](bar_plot.png)
    * *The bar plot shows the average page views per month across different years, revealing consistent seasonal patterns where some months (e.g., summer) tend to have lower activity.*

* **Year-wise and Month-wise Box Plots (`box_plot.png`):**
    * ![Box Plots](box_plot.png)
    * *These box plots clearly demonstrate the yearly trend of increasing page views (left) and the consistent monthly seasonality (right), allowing for detailed observation of data distribution and outliers.*

---

### 🛠️ How to Run This Project

To set up and run this project locally, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/Mithleshpatel09/time_series_visualizer.git](https://github.com/Mithleshpatel09/time_series_visualizer.git)
    cd time_series_visualizer
    ```
2.  **Ensure data file is present:** Make sure `fcc-forum-pageviews.csv` is in the project root. (Download from [here](https://raw.githubusercontent.com/freeCodeCamp/boilerplate-time-series-visualizer/main/fcc-forum-pageviews.csv) if missing).
3.  **Create and activate a virtual environment:**
    ```bash
    python -m venv venv
    .\venv\Scripts\activate # For Windows
    # source venv/bin/activate # For macOS/Linux
    ```
4.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
5.  **Run the project to generate plots:**
    ```bash
    python # Open Python interpreter
    >>> import time_series_visualizer as tsv
    >>> tsv.draw_line_plot()
    >>> tsv.draw_bar_plot()
    >>> tsv.draw_box_plot()
    >>> exit() # Exit interpreter
    ```
    *This will generate `line_plot.png`, `bar_plot.png`, and `box_plot.png` in the project folder.*

---

### 📧 Connect with Me

* **LinkedIn:** [linkedin.com/in/mithleshpatel09](https://www.linkedin.com/in/mithleshpatel09)
* **Email:** [mithleshsinghpatel779@gmail.com](mailto:mithleshsinghpatel779@gmail.com)

---
