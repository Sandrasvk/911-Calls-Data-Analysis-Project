# 911 Calls - Data Analysis Project

## 📌 Project Overview
This project performs an Exploratory Data Analysis (EDA) on a dataset of 911 emergency calls. The analysis transforms raw call logs into structured insights, focusing on the categorization of emergency types and the timing of incidents to identify high-activity periods.

## 🛠️ Tech Stack
* *Language:* Python
* *Libraries:* Pandas, NumPy, Matplotlib, Seaborn
* *Environment:* Jupyter Notebook

## 🔍 Key Analysis & Steps

### 1. Data Exploration
* *Location Analysis:* Identified the top 5 zip codes and townships with the highest call volumes.
* *Volume Assessment:* Analyzed a dataset of approximately 99,000 call records to determine the most frequent emergency types.

### 2. Feature Engineering
* *Reason Categorization:* Created a new Reason column by extracting department prefixes (EMS, Fire, Traffic) from the title field using string manipulation and lambda functions.
* *DateTime Conversion:* Converted raw timestamp strings into Python DateTime objects to allow for precise time-based indexing.
* *Temporal Features:* Extracted *Hour, **Month, and **Day of Week* to enable deeper analysis of when emergencies occur.

### 3. Visualizing Trends
* *Categorical Distribution:* Produced countplots to visualize which emergency categories (e.g., EMS) are most prevalent.
* *Weekly Activity:* Generated clustered bar charts (Seaborn countplots) to compare the frequency of different emergency types across the days of the week.
* *Label Mapping:* Mapped numerical day values (0-6) to string format (Mon-Sun) for better readability in visualizations.

## 📈 Key Insights
* *Primary Reason:* EMS was found to be the leading cause of 911 calls.
* *Peak Areas:* Successfully ranked townships and zip codes by call density.
* *Temporal Patterns:* Identified how call volumes for Traffic, Fire, and EMS fluctuate between weekdays and weekends.

## 🚀 How to Run
1. Ensure you have Python installed.
2. Install dependencies: pip install pandas numpy matplotlib seaborn
3. Open the Jupyter Notebook and run the cells to generate the analysis and plots.
