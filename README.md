📊 Customer Behavior Analysis | Data Analytics Portfolio Project
An end-to-end data analytics project exploring customer purchasing behavior using Python, Pandas, SQL, PostgreSQL, and Power BI. The project demonstrates a practical workflow for preparing customer shopping data, analyzing purchasing patterns, querying a relational database, and presenting business metrics through a dashboard.
🎯 Project Objectives
- Clean and prepare customer shopping data using Python and Pandas.
- Perform exploratory data analysis (EDA).
- Analyze purchasing behavior using SQL and PostgreSQL.
- Investigate customer spending, product ratings, discounts, shipping methods, and subscription behavior.
- Visualize customer behavior and business metrics using Power BI.
- Communicate evidence-based findings and recommendations.
🛠️ Technologies Used
Technology	Purpose
Python	Data analysis and preprocessing
Pandas and NumPy	Data manipulation and numerical operations
Jupyter Notebook	Interactive analysis
SQL	Business queries and aggregations
PostgreSQL	Relational database
SQLAlchemy and psycopg	Python-to-PostgreSQL connection
Power BI	Dashboard and data visualization
CSV	Source dataset
Git and GitHub	Version control and project hosting


📂 Repository Structure
customer_behavior_analysis/
├── README.md
├── customer_behavior.ipynb
├── customer_behavior.sql
├── customer_behavior_dashboard.pbix
└── customer_shopping_behavior.csv
🔄 Project Workflow
1. Data loading and understanding: Load the CSV, inspect columns and data types, and assess data quality.
2. Data cleaning: Investigate missing values, duplicates, inconsistent categories, and incorrect data types.
3. Exploratory data analysis: Explore purchasing patterns, customer characteristics, ratings, discounts, and shipping methods.
4. Database integration: Load the prepared dataset into PostgreSQL.
5. SQL analysis: Use aggregations, subqueries, CTEs, conditional logic, and window functions to answer business questions.
6. Power BI visualization: Explore key metrics and patterns in the dashboard.
7. Insights and recommendations: Document findings supported by the actual query results and dashboard.
🔍 Business Questions
The SQL analysis investigates these ten questions:
1. Revenue by gender: What is the total purchase revenue recorded for male and female customers?
2. Discounts and spending: Which discounted purchase records have an amount greater than the overall average purchase amount?
3. Product ratings: Which five products have the highest average review rating?
4. Shipping methods: How do average purchase amounts compare between Standard and Express Shipping?
5. Subscription behavior: How do average purchase amount and total recorded revenue compare between subscribers and non-subscribers?
6. Discount rates: Which five products have the highest percentage of purchase records with discounts applied?
7. Customer segments: How are records classified as New, Returning, and Loyal based on previous purchases?
8. Top products by category: What are the three most frequently recorded products within each category?
9. Repeat buyers and subscriptions: What is the subscription-status distribution among customers with more than five previous purchases, and how does it compare with other customers?
10. Revenue by age group: What is the total recorded purchase revenue for each age group?
Interpretation note: The dataset's row granularity matters. If a customer can appear in multiple rows, counts of rows are not the same as counts of unique customers. The SQL results should be interpreted accordingly. The repeat-buyer question should compare subscription rates for repeat and non-repeat groups before concluding that one group is more likely to subscribe.

📊 Key Metrics
Depending on the available data and dashboard configuration, the project examines:
- Total recorded purchase revenue
- Average purchase amount
- Purchase-record counts
- Average product review rating
- Discount rate by product
- Purchase amounts by shipping method
- Subscription-status distribution
- Product purchase frequency
- Revenue by age group
🚀 Getting Started on Windows
Prerequisites
Install the following tools as needed:
- Python 3.11 or 3.12
- Jupyter Notebook
- PostgreSQL
- Microsoft Power BI Desktop
- A SQL client such as pgAdmin or DBeaver (optional)
1. Clone the repository
Open PowerShell or Command Prompt and run:
git clone https://github.com/ShubhamB0107/customer_behavior_analysis.git
cd customer_behavior_analysis
2. Create and activate a virtual environment
python -m venv .venv
.\.venv\Scripts\Activate.ps1
If PowerShell blocks activation, you can use Command Prompt instead:
.venv\Scripts\activate.bat
Alternatively, run Python and pip through the environment without activating it:
.\.venv\Scripts\python.exe -m pip install --upgrade pip
3. Install Python dependencies
If a requirements.txt file is not present in the repository, install the main packages:
python -m pip install pandas numpy matplotlib seaborn jupyter sqlalchemy "psycopg[binary]" python-dotenv
4. Open the notebook
jupyter notebook
Open customer_behavior.ipynb in the browser and execute its cells in order. If the notebook uses a relative CSV path, ensure that the path matches the repository's actual file layout.
5. Configure PostgreSQL
Create the database if it does not already exist:
CREATE DATABASE customer_behavior;
Configure your local PostgreSQL connection in the notebook or through environment variables. Ensure that the database, table, column names, and data types match the SQL script.
To run the SQL analysis:
1. Open pgAdmin or another PostgreSQL client.
2. Connect to your local PostgreSQL server.
3. Select the customer_behavior database.
4. Open customer_behavior.sql.
5. Execute the queries after confirming the data has been loaded into the expected customer table.
Security: Do not commit passwords, .env files, private credentials, or sensitive customer data to GitHub.
6. Open the Power BI dashboard
Open customer_behavior_dashboard.pbix in Power BI Desktop. If the dashboard uses a local CSV path or PostgreSQL connection, update its data source settings and refresh the data as necessary.
📈 Findings and Recommendations
Record actual findings here after executing the SQL queries and reviewing the dashboard. Good findings should include:
- The metric or pattern observed.
- The result that supports the observation.
- Why the result may matter to the business.
- A recommendation, with limitations noted where appropriate.
Do not infer causation from a simple difference in revenue, ratings, or subscription status.
🔮 Possible Future Improvements
- Add RFM (Recency, Frequency, Monetary) customer segmentation if the data supports it.
- Compare subscription rates between repeat and non-repeat buyers.
- Analyze retention and repeat-purchase patterns where transaction history is available.
- Add a report summarizing the strongest findings.
- Improve dashboard KPIs and interactivity.
- Automate the data preparation and reporting workflow.
📚 Learning Outcomes
This project provides practical experience with:
- Data cleaning and preprocessing using Python.
- Exploratory data analysis and visualization.
- SQL aggregations, subqueries, CTEs, and window functions.
- PostgreSQL database integration.
- Dashboard-based communication of analytical results.
- Translating business questions into measurable queries.
- Documenting a reproducible analytics workflow.
📜 Dataset and License
This project is intended for educational and portfolio purposes. Check the original dataset's license and attribution requirements before redistributing the CSV. No project license is implied unless a license file is added to the repository.
👨‍💻 About the Author
Shubham Bendre
Aspiring Data Analyst | Python | SQL | PostgreSQL | Power BI
- GitHub: ShubhamB0107
- LinkedIn: Shubham Bendre
- Portfolio: Personal Portfolio
⭐ If you find this project useful, consider starring the repository.
Turning customer shopping data into meaningful business insights through data analytics.
