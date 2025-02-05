# Air-Quality-Analysis-for-Local-Government
Air Quality Analysis for Local Government (winter2024/2025)
Air Quality Analysis for Bradford

📊 Project Overview

This project focuses on analyzing air quality data from Bradford, with an emphasis on PM2.5 and PM10 levels across multiple monitoring sites. The goal was to clean, process, and analyze the data to provide meaningful insights for Bradford Council regarding air quality trends, exceedances, and potential health impacts.

⚙️ Key Features

Data Cleaning: Handled negative and missing values.

Air Quality Analysis: Identified exceedances and trends in PM2.5 and PM10.

Exposure Assessment: Classified exposure levels across different sites.

Regulatory Comparison: Compared results to current and future air quality standards.

Insights for Policymakers: Provided actionable insights for better air quality management.

🗂️ Project Structure

├── data/
│   └── bradford_air_quality_data.xlsx
├── notebooks/
│   └── air_quality_analysis.ipynb
├── presentation/
│   └── bradford_air_quality_report.pdf
├── src/
│   └── data_cleaning.py
│   └── analysis.py
├── README.md
└── requirements.txt

data/: Raw data files.

notebooks/: Jupyter Notebook with analysis steps.

presentation/: Final report or presentation slides.

src/: Python scripts for data cleaning and analysis.

requirements.txt: Python dependencies.

📥 Data Loading and Initial Exploration

Loaded air quality data into a Pandas DataFrame.

Performed an initial inspection to identify data types, missing values, and anomalies.

🧹 Data Cleaning

Handling Negative Values

Identified negative PM2.5 and PM10 values.

Replaced negative values with 0, as negative readings are physically impossible.

Investigated instances where PM2.5 > PM10 to identify measurement errors.

Handling Missing Values

Checked for missing data patterns.

Keighley: Used linear interpolation for imputation.

Tong Street: No imputation between December 29th and January 3rd (equipment removed).

Treadwell Mills: Adjusted dataset to account for the device becoming operational post-December 21st.

📊 Air Quality Analysis

PM10 Exceedances: Identified exceedances based on the 50 µg/m³ threshold.

PM2.5 Trends: Compared average concentrations against current (20 µg/m³) and future (12 µg/m³ by 2028) targets.

Exposure Categories: Defined as Low, Moderate, and High exposure levels.

Exposure Analysis: Calculated the percentage of time populations were exposed to each category.

📝 Key Findings

Data Quality Issues: Addressed negative and missing values.

Exceedances: Detected PM10 exceedances, especially on January 16th at Keighley and Treadwell Mills.

Site Comparisons: Identified differences in PM2.5 and PM10 levels across sites.

Exposure Insights: Quantified exposure levels for different monitoring locations.

🔍 Areas for Further Analysis

January 16th PM10 Spike:

Correlate with weather and traffic data.

Investigate local events or industrial activities.

Advanced Data Quality Checks:

Equipment calibration review.

Advanced imputation techniques (time series models).

Deeper Air Quality Analysis:

Time series forecasting.

Spatial analysis with additional monitoring sites.

Predictive Modeling:

Develop models to forecast PM2.5 and PM10 levels.

Interactive Dashboards:

Build visual tools for easier data exploration and stakeholder engagement.

🚀 How to Run

Clone the repository:

git clone https://github.com/your-username/bradford-air-quality-analysis.git
cd bradford-air-quality-analysis

Install dependencies:

pip install -r requirements.txt

Run the analysis notebook:
Open air_quality_analysis.ipynb in Jupyter Notebook.

📦 Dependencies

Python 3.8+

pandas

numpy

matplotlib

seaborn

scipy

statsmodels

Install all dependencies using:

pip install -r requirements.txt

🙌 Acknowledgments

Bradford Council for providing the data.

Contributors to the open-source libraries used in this project.

📬 Contact

Shaurya PalInformation Analyst Trainee | Data ScientistLinkedIn | Email

📢 License

This project is licensed under the MIT License. See the LICENSE file for more details.

Feel free to contribute to this project by submitting pull requests or reporting issues!

