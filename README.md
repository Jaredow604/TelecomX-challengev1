📌 Executive Summary
This Data Science initiative focuses on analyzing the customer base of a telecommunications provider to uncover the primary drivers behind service cancellations (Churn). Through rigorous data cleaning, feature engineering, and visual analysis, this project identifies critical behavioral patterns, delivering strategic recommendations to improve user retention and maximize customer lifetime value.

🛠️ Methodology & Data Pipeline
The core notebook documents an end-to-end data processing workflow:

1. Extraction, Transform, Load (ETL)
Ingestion: Consumed raw transactional and demographic data in JSON format.

Flattening: Unpacked and structured nested JSON columns into a tabular format.

Standardization: Converted categorical boolean values (e.g., "Yes/No" to "1/0") and corrected numerical data types to enable mathematical processing and correlation scaling.

2. Feature Engineering
Custom Metrics: Calculated a new Daily_Charges variable to granularly analyze the psychological and financial impact of daily costs on customer retention.

3. Exploratory Data Analysis (EDA)
Deployed advanced statistical visualizations to cross-reference demographic and financial variables against the target variable (Churn rate).

🚀 Key Findings & Business Insights
Our visual and statistical analysis revealed three critical churn drivers:

The Critical Window: The highest volume of cancellations occurs during the first few months of service, indicating a potential flaw in the initial user experience or onboarding process.

The Monthly Contract Risk: Users on a "month-to-month" payment plan exhibit the highest flight risk compared to those on long-term contracts.

Price Sensitivity: Counterintuitively, customers paying the highest monthly premiums are abandoning the service at the fastest rate, suggesting a misalignment between cost and perceived value.

💻 Tech Stack
To ensure reproducibility, this project was built using standard industry libraries:

Language: Python 3.x

Data Manipulation: Pandas (ETL and feature engineering)

Base Visualization: Matplotlib (Structural plotting)

Advanced Statistics: Seaborn (Heatmaps, boxplots, and distribution analysis)

Environment: Jupyter Notebook / Google Colab

⚙️ Quick Start Guide
To clone this repository and run the analysis locally, follow these steps:

Clone the repository to your local machine:

Bash
git clone https://github.com/JociasOrt/telecom-customer-churn-analysis.git
Environment Setup: Ensure you have Python 3.x installed alongside a notebook environment (Jupyter).

Install Dependencies:

Bash
pip install pandas matplotlib seaborn
Execute: Open the main .ipynb notebook and run the cells in sequential order. The raw data will be automatically loaded, cleaned, and visualized.
