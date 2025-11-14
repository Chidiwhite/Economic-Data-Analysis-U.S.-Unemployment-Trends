📊 Economic Data Analysis — U.S. Unemployment Trends

A data-driven exploration of national and state-level unemployment patterns using the Federal Reserve Economic Data (FRED) API.

📁 Project Overview

This project provides an end-to-end analysis of U.S. unemployment indicators using time-series data retrieved directly from the FRED API. It demonstrates the full workflow of data acquisition, cleaning, analysis, and visualization, focusing on both national trends and state-level variations.

🎯 Objective

The primary goal of this analysis is to examine how unemployment rates have evolved across U.S. states, identify periods of significant economic disruption, and visualize patterns in employment changes over time.
This project also highlights key data skills, including:

API-based data extraction

Time-series data manipulation

Exploratory data analysis (EDA)

Visual storytelling with Python

🔗 Data Source

Data was sourced programmatically using the Federal Reserve Economic Data (FRED) API.

Data Retrieval Steps:

A FRED client object was created to connect to the database.

Unemployment-related series were located via keyword search.

Each series was downloaded using fred.get_series() and stored in pandas DataFrames.

Multiple series were merged into a unified dataset (unemp_states) for state-by-state comparison.

🧹 Data Preparation & Cleaning

The raw dataset included missing values and outdated historical periods. Key cleaning steps included:

Filtering for monthly, seasonally adjusted, percentage-based unemployment series

Dropping non-state columns and those with >50% missing data

Imputing remaining missing values using column means

Removing old data (1929–1980) to retain focus on modern labor trends

These steps ensured a consistent and analysis-ready dataset.

📈 Analysis & Visualization

Multiple exploratory analyses were carried out to uncover underlying trends:

Visualizations Included:

Line charts showing unemployment trends nationally and across states

Horizontal bar chart highlighting April 2020 unemployment by state — capturing the economic shock of the COVID-19 pandemic

Formatting enhancements were applied to improve readability of dense state-level labels and grid layouts.

🔍 Key Insights

Unemployment spiked dramatically across nearly all states in April 2020, reflecting severe pandemic-related shutdowns.

Some states experienced significantly higher unemployment peaks than others, revealing regional vulnerabilities.

Long-term patterns show cyclical economic behavior, but the 2020 spike remains historically exceptional.

🛠️ Tools & Technologies

Programming Language: Python

Libraries Used:

pandas

matplotlib

seaborn

Skills Demonstrated:

API integration

Time-series data cleaning

Handling missing values

Comparative state-level analysis

Visual communication of economic trends

✅ Project Outcome

This project delivers a clean, reproducible workflow for analyzing real-world economic data. It demonstrates proficiency in:

Automated data extraction

Dataset preparation

Time-series analysis

Creating meaningful visual insights

The resulting notebook serves as a strong example of data-driven research, particularly in labor market and economic studies.
