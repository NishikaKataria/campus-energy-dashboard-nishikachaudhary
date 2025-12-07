# campus-energy-dashboard-nishikachaudhary
A simple Python project that loads multiple building energy CSV files, cleans the data, calculates daily and weekly usage, creates visual charts, and produces a summary report. This project is part of my Capstone Assignment for Programming in Python.
Campus Energy Dashboard – Capstone Project

This project is my Capstone Assignment for Programming for Problem Solving using Python.
It is a complete pipeline where I read energy-use data from different buildings, clean the data, analyze it, and create visual charts to understand electricity consumption on campus.
📌 Project Objectives

Read multiple CSV files of building electricity usage.

Combine them into one clean dataset.

Calculate useful insights like daily and weekly consumption.

Build simple Python classes for buildings and readings.

Create a dashboard with multiple charts.

Generate summary reports and export cleaned data.

📂 Folder Structure
campus-energy-dashboard/
│
├── data/                    # CSV files for each building
├── energy_dashboard.py      # Main Python script
├── dashboard.png            # Saved figure with 3 charts
├── cleaned_energy_data.csv  # Cleaned and merged dataset
├── building_summary.csv     # Summary table (per building)
├── summary.txt              # Text summary of findings
└── README.md

🛠 Technologies Used

Python

pandas

matplotlib

pathlib

Object-Oriented Programming (OOP)

🧩 What the Program Does (Simple Explanation)
Task 1 – Data Loading

The program reads all .csv files from the data folder using pathlib.
If a file is missing or corrupted, it skips it safely.
All files are combined into one big DataFrame.

Task 2 – Aggregation / Calculations

The program calculates:

Daily energy usage

Weekly energy usage

Building-wise statistics (mean, min, max, total)

Functions like:

calculate_daily_totals(df)
calculate_weekly_aggregates(df)
building_wise_summary(df)


are used for clean and simple logic.

Task 3 – OOP Model

I created three classes:

✔ MeterReading

Stores timestamp and kWh.

✔ Building

Stores building name and list of readings.

✔ BuildingManager

Loads all data and manages all buildings together.

This helps organize the project and follow OOP concepts.

Task 4 – Visualization

The program generates 3 charts:

Daily consumption line graph

Weekly usage bar chart

Scatter plot for peak-hour or reading comparison

All charts are combined into one image called dashboard.png.

Task 5 – Data Export & Summary

The program creates:

cleaned_energy_data.csv

building_summary.csv

summary.txt

Total energy consumed

Highest consuming building

Peak load

Weekly & daily insights

▶️ How to Run

Install libraries:

pip install pandas matplotlib


Place all .csv files inside the data folder.

Run the script:

python energy_dashboard.py


Check the output files:

dashboard.png

summary.txt

cleaned_energy_data.csv

📊 Example of Dataset Format
timestamp,kwh
2024-01-01 00:00,120
2024-01-01 01:00,110
...
📚 Assignment Context (in simple words)

This project helps understand how the campus uses electricity and which buildings consume the most.
By creating charts and summaries, the campus team can plan ways to save energy and reduce bills.

🙋‍♀️ Created By

Nishika Chaudhary
BTECH CSE (Data Science)
Programming for Problem Solving using Python
Capstone Project
