# E-commerce Sales & Customer Segmentation Dashboard

[**▶ View the Live Interactive Dashboard**](https://public.tableau.com/app/profile/vaibhaw.verma/viz/E-commerceSalesCustomerSegmentationDashboard/Dashboard1)

## Project Overview
This project demonstrates an **end-to-end business analysis workflow**, starting from a large e-commerce transactional dataset and culminating in a fully interactive **business intelligence dashboard**.

The goal is to:
- Uncover sales trends  
- Track key performance indicators (KPIs)  
- Segment customers to enable targeted marketing strategies  

<!-- ![Dashboard Screenshot](PASTE_IMGUR_LINK_HERE) -->

---

## Key Features
- **Sales Performance Tracking** – Monitor total revenue, sales volume, and seasonal trends over time.  
- **Geographical Analysis** – Visualize sales performance by country on an interactive map.  
- **Customer Segmentation (RFM Analysis)** – Classify customers into segments like _Champions_, _At Risk_, and _Lost_ based on Recency, Frequency, and Monetary value.  
- **Interactive Filtering** – Drill down into specific countries or customer segments for deeper insights.  

---

## Technologies Used
- **Data Manipulation & Analysis:** Python (Pandas)  
- **Data Visualization & Dashboarding:** Tableau Public  

---

## Process / Methodology
1. **Data Collection**  
   - Used the [Online Retail II UCI](https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci) dataset from Kaggle (over 500,000 transactions).

2. **Data Cleaning & Preparation**  
   - Loaded the data using Python.  
   - Removed missing values (especially `CustomerID`), duplicates, and invalid entries (e.g., returns with negative quantities).  
   - Engineered new features such as `TotalPrice` and extracted date components (Year, Month).  

3. **RFM Analysis**  
   - Calculated Recency, Frequency, and Monetary values for each customer.  
   - Categorized customers into distinct segments based on their RFM scores.  

4. **Data Visualization**  
   - Loaded cleaned data and RFM segments into Tableau.  
   - Created worksheets for sales trends, geographical sales, and RFM segment distribution.  
   - Combined all visuals into a single interactive dashboard.  

---

## Key Insights
- **Seasonality:** Sales spike in **November** → holiday shopping season opportunity for inventory & marketing.  
- **Customer Value:** _Champions_ segment generates most revenue → focus on retention.  
- **Market Dominance:** UK leads in sales, but **Germany** & **France** show strong growth potential.  
- **Customer Risk:** Many customers in _At Risk_ and _Lost_ segments → need re-engagement campaigns.  

---

## How to Run This Project Locally
1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/ecommerce-dashboard.git
   cd ecommerce-dashboard

2. Install dependencies:
   ```bash
   pip install pandas

3. Download the dataset from Kaggle and place it in the project folder.
   
4. Run data cleaning:
   ```bash
   python data_cleaning.py

5. Run RFM analysis:
   ```bash
   python rfm_analysis.py

6. Open the `.twbx` file in Tableau Public.
