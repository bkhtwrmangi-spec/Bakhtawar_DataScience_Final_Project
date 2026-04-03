# Bakhtawar_DataScience_Final_Project

📊 Sales Data Analysis Dashboard

Overview

This project was developed as my Final Internship Project at SoftGrowTech.
It is a complete Sales Data Analysis Dashboard built with Python and Streamlit, designed to provide actionable insights into product performance, revenue distribution, and monthly sales trends.

🔧 Tech Stack
Python (Pandas, NumPy, Matplotlib, Seaborn)

Streamlit (for interactive dashboard)

Dataset: sales_data_sample.csv (Kaggle)

🚀 Features
Data loading, cleaning, and preprocessing

Exploratory Data Analysis (EDA) with insights

Feature extraction for monthly sales trends

Visualizations:

Top selling products (bar chart)

Monthly sales trend (line chart)

Revenue distribution (pie chart)

Streamlit dashboard with:

KPIs (Total Revenue, Top Product)

Interactive charts

🛠 How I Built This Project
Data Loading

Used Pandas to read sales_data_sample.csv.

Faced encoding issues (UnicodeDecodeError) → solved by using latin1 and ISO-8859-1 fallback.

Data Cleaning & Preprocessing

Renamed Kaggle dataset columns (ORDERDATE → Date, PRODUCTLINE → Product, etc.).

Converted dates to datetime format.

Ensured numeric columns (Quantity, Price, Revenue) were properly cast.

Feature Extraction

Created a Month column using Date.

Aggregated monthly revenue for trend analysis.

Exploratory Data Analysis (EDA)

Built bar chart for top products.

Line chart for monthly revenue trends.

Pie chart for revenue distribution.

Added insights after each visualization.

Streamlit Dashboard

Designed KPIs (Total Revenue, Top Product).

Integrated interactive charts (st.bar_chart, st.line_chart, st.pyplot).

Finalized a clean, production-ready dashboard.

⚡ Challenges Faced & Solutions
Encoding Errors:

Problem: CSV file threw UnicodeDecodeError.

Solution: Added encoding fallback (latin1, ISO-8859-1).

Column Name Mismatch:

Problem: Kaggle dataset columns didn’t match my code assumptions.

Solution: Renamed columns in clean_data() to standard names (Date, Product, Quantity, Price, Revenue).

KeyError: 'Date':

Problem: Functions failed because Date column wasn’t recognized.

Solution: Explicitly mapped ORDERDATE → Date during preprocessing.

Dashboard Integration:

Problem: Streamlit charts initially didn’t align with Pandas groupings.

Solution: Reset index and ensured proper aggregation before plotting.

📈 Insights
Revenue is concentrated among a few product lines.

🙌 Acknowledgments
Special thanks to SoftGrowTech for providing mentorship and guidance during my internship. This project helped me strengthen my skills in data science, visualization, and dashboard development.

Seasonal peaks are visible in monthly sales trends.

Top products contribute disproportionately to overall revenue.
