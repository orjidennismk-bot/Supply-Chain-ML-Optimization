# Supply-Chain-ML-Optimization
An automated Python  data pipeline that cleans, transforms, and analyzes logistics data to optimize inventory levels and reduce supply chain bottlenecks.
# Supply-Chain-ML-Optimization

## Project Overview
This project demonstrates a dual-track Machine Learning lifecycle aligned with the PACE framework, developed to optimize both financial performance and operational reliability in global supply chains. By cleaning and engineering over 180,000 historical records, raw data was transformed into two distinct predictive engines.

## Track 1: Revenue Forecasting (Regression)
A Random Forest Regressor was engineered to provide deep visibility into the financial drivers of the business. 
* **Algorithm:** `RandomForestRegressor` optimized via `GridSearchCV`
* **Performance:** R² Score of 0.7423 with a Mean Absolute Error of $42.69.
* **Business Insight:** Feature importance analysis mathematically proved that Product Category (specifically Computers and Fishing) dominates order value. This empowers strategic allocation of warehouse space and marketing budgets.

## Track 2: Risk Mitigation (Classification)
To balance revenue with customer satisfaction, an early-warning radar was built to classify logistical vulnerabilities.
* **Algorithm:** `RandomForestClassifier` with class-weight balancing.
* **Performance:** 84% Precision in identifying high-risk orders.
* **Business Insight:** The model successfully identified over 11,000 destined-to-be-late orders in unseen test data, allowing supply chain managers to proactively reroute packages.

## How to Run This Project
1. Clone this repository to your local machine.
2. Install the required dependencies: `pip install -r requirements.txt`
3. Run the Jupyter Notebook `supply chain.ipynb`. 
   *Note: Due to file size, the trained model artifact is generated locally upon execution of the notebook.*

## Tech Stack
* **Languages:** Python
* **Libraries:** Scikit-Learn, Pandas, NumPy, Matplotlib, Seaborn
* **Techniques:** Data imputation, One-Hot Encoding, Pipeline construction, Grid Search cross-validation, Feature Importance extraction.
