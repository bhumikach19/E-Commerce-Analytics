# UCI Retail Analytics Project

## Overview
This project performs comprehensive retail analytics on the UCI Online Retail II dataset, focusing on customer segmentation, revenue analysis, and business insights. The analysis includes data cleaning, RFM (Recency, Frequency, Monetary) analysis, customer clustering, and revenue trend analysis.

## 📊 Dataset
- **Source**: UCI Online Retail II Dataset
- **Size**: ~90MB (814,845 records)
- **Time Period**: December 2009 - August 2011
- **Features**: Invoice, StockCode, Description, Quantity, InvoiceDate, Price, Customer ID, Country

## 🗂️ Project Structure
```
UCI/
├── UCI.ipynb                    # Main Jupyter notebook with analysis
├── online_retail_II.csv         # Original dataset
├── cleaned_retail_data.csv      # Cleaned and processed data
├── customer_segments.csv        # Customer segmentation results
├── monthly_revenue.csv          # Monthly revenue analysis
├── Country revenue.csv          # Revenue by country
├── Stockcode description.csv    # Product descriptions
├── Analytics.pdf               # Detailed analytics report
└── README.md                   # This file
```

## 🔧 Data Processing Steps

### 1. Data Cleaning
- Removed rows with missing Customer ID
- Eliminated duplicate records
- Filtered out negative quantities (returns)
- Converted InvoiceDate to datetime format
- Created TotalPrice column (Quantity × Price)

### 2. Data Analysis
- **Monthly Revenue Analysis**: SQL-based aggregation of revenue by month
- **RFM Analysis**: Customer segmentation based on:
  - **Recency**: Days since last purchase
  - **Frequency**: Number of purchases
  - **Monetary**: Total amount spent
- **Customer Clustering**: K-means clustering (4 clusters) for customer segmentation
- **Geographic Analysis**: Revenue breakdown by country

## 📈 Key Insights

### Revenue Trends
- Peak revenue: November 2010 (£1,166,460)
- Seasonal patterns observed
- Overall growth trend from 2009 to 2011

### Customer Segments
- **4 distinct customer clusters** identified using K-means
- Segmentation based on RFM scores
- Enables targeted marketing strategies

### Geographic Distribution
- **United Kingdom**: Primary market (87% of revenue)
- **EIRE**: Second largest market
- **Netherlands, Germany, Denmark**: Emerging markets

## 🛠️ Technologies Used
- **Python**: Primary programming language
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computations
- **Scikit-learn**: Machine learning (K-means clustering)
- **SQLite**: Database operations
- **Jupyter Notebook**: Interactive development and documentation
- **Power BI**: Business intelligence dashboard creation and visualization

## 📋 Prerequisites
```bash
pip install pandas numpy scikit-learn jupyter sqlite3
```

**For Power BI Dashboard:**
- Microsoft Power BI Desktop (free version available)
- Power BI service account (for sharing and collaboration)

## 🚀 Usage

### Running the Analysis
1. Ensure all CSV files are in the project directory
2. Open `UCI.ipynb` in Jupyter Notebook
3. Run cells sequentially to reproduce the analysis

### Viewing the Dashboard
1. Open `Analytics.pdf` to view the Power BI dashboard
2. The dashboard contains interactive visualizations of all key metrics
3. For full interactivity, open the original Power BI file (.pbix) if available

### Key Outputs
- **cleaned_retail_data.csv**: Processed dataset ready for analysis
- **customer_segments.csv**: Customer clustering results with RFM scores
- **monthly_revenue.csv**: Monthly revenue trends
- **Country revenue.csv**: Geographic revenue distribution
- **Analytics.pdf**: Power BI dashboard with interactive visualizations

## 📊 Analysis Components

### 1. Data Exploration
- Dataset overview and statistics
- Data quality assessment
- Missing value analysis

### 2. Revenue Analysis
- Monthly revenue trends
- Seasonal patterns identification
- Growth rate calculations

### 3. Customer Segmentation
- RFM score calculation
- K-means clustering (k=4)
- Customer behavior analysis

### 4. Geographic Analysis
- Revenue by country
- Market concentration analysis

## 📈 Interactive Dashboard

### Power BI Analytics Dashboard
Our comprehensive business intelligence dashboard provides interactive visualizations of all key insights:

| Feature | Description |
|---------|-------------|
| 📊 **Revenue Trends** | Monthly revenue analysis with seasonal patterns |
| 👥 **Customer Segments** | RFM-based customer clustering visualization |
| 🌍 **Geographic Analysis** | Revenue distribution by country |
| 📈 **Performance Metrics** | Key performance indicators and trends |

**[📊 View Dashboard](Analytics.pdf)** | **[📥 Download PDF](Analytics.pdf)**


## 📈 Business Applications
- **Customer Retention**: Identify high-value customers
- **Marketing Strategy**: Target campaigns based on segments
- **Inventory Management**: Seasonal demand patterns
- **Market Expansion**: Geographic opportunity analysis

## 🔍 Future Enhancements
- Predictive analytics for customer churn
- Product recommendation systems
- Advanced time series analysis
- Interactive dashboards
