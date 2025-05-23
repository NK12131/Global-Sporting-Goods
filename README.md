# 🛍️ Global Sporting Goods Market Analysis & Optimization

**Team Members**  
- Nithin Kumar Hadhge Girish Kumar ([NK12131](https://github.com/NK12131))  
- Resham Deepak Bahira ([Reshamm13](https://github.com/Reshamm13))  
- Sudhanshu Gopalrao Pawar ([Psudhanshu](https://github.com/Psudhanshu))

---
## 📌 Introduction
This project performs a comprehensive analysis of a global sporting goods retailer's transactional dataset to uncover insights in three key areas: international market segmentation, discount optimization, and delivery risk prediction. The goal was to support better decision-making across pricing, promotions, and supply chain logistics.

## 🎯 Objectives

### 1. **Competitive Market Analysis by Country**
- Segment countries by product preferences and pricing behaviors.
- Identify premium vs. price-sensitive markets using clustering and average pricing.

### 2. **Discount Effectiveness Analysis**
- Determine optimal discount rates to maximize profitability.
- Analyze sales volume, revenue impact, and regional discount patterns.

### 3. **Supply Chain Risk Modeling**
- Predict late delivery risks using logistic regression.
- Recommend actionable improvements in shipping strategies.


## 📊 Visualizations
- Treemaps for category-wise sales by country
- Bar charts for average product price comparisons
- Cluster maps for regional segmentation
- Logistic regression coefficient plots for delivery risk factors

---

## 🧪 Methodology

### Data Processing
- Cleaned and transformed using **PySpark** for scalable processing
- Handled missing data, one-hot encoding, and high-cardinality features (e.g., ZIP codes)

### Modeling Techniques
- Regression: Random Forest, XGBoost, Ridge Regression
- Classification: Logistic Regression
- Clustering: KMeans for country segmentation
- Evaluation: RMSE, R², Precision, Recall, F1-Score, ROC-AUC


## 📊 Results

### 🔹 Market Segmentation & Clustering
- **KMeans clustering** segmented **35+ countries** into 4 market types:
  - **Premium Markets**: Western Europe, Oceania
  - **Mid-Tier Regions**: Central America, Southeast Asia
  - **Price-Sensitive Markets**: Eastern Europe, Africa, USCA
- Enabled targeted pricing and inventory strategies.
- Resulted in **15% increase in ROI** from region-specific promotions.

### 🔹 Sales Forecasting
- **Models Used**: Random Forest, XGBoost
- **XGBoost Performance**:
  - RMSE: `0.43`
  - R²: `0.60`
- Improved forecasting accuracy by **33%** over baseline models.
- Informed more accurate pricing and supply planning strategies.

### 🔹 Discount Optimization
- Identified optimal discount thresholds (10%–25%) for maximum profitability.
- Found that **standardized discounts alone had weak correlation with sales**, suggesting the need for smarter, region-tailored strategies.
- Resulted in strategic discount adjustments that enhanced campaign performance and protected profit margins.

### 🔹 Late Delivery Risk Modeling
- **Model Used**: Logistic Regression
- **Performance Metrics**:
  - Accuracy: `93.29%`
  - Precision: `90.37%`
  - Recall: `94.37%`
  - ROC-AUC: `98.38%`
- High recall ensured timely identification of risky shipments.
- Guided logistics planning and reduced customer dissatisfaction due to delayed deliveries.

---

## 🚧 Limitations

- **Data Imbalance**: Some geographic regions and product categories had sparse data, which made model generalization challenging.
- **High Cardinality Features**: ZIP codes and customer regions needed encoding and careful feature selection to avoid overfitting.
- **Overfitting Risks**: Advanced models like XGBoost required tuning to prevent high variance, especially in small or imbalanced segments.
- **Limited Operational Data**: Real-time tracking metrics (like warehouse inventory or carrier reliability) were not included.

---

## 🔮 Future Work

- **Integrate Real-Time Logistics Metrics**: Include warehouse, vendor, and courier performance data for more accurate delivery risk modeling.
- **Deploy Interactive Dashboard**: Visualize regional segmentation, discount simulations, and delivery predictions for stakeholders.
- **Dynamic Discounting System**: Build an automated model that adjusts discounts by region, category, and time to maximize conversions.
- **Customer Segmentation**: Add behavior-based customer clustering to align marketing strategies and increase customer lifetime value.
- **Expand to Deep Learning Models**: Use LSTM or transformer-based approaches for more sophisticated temporal modeling in sales forecasting.

---

## 📈 Business Impact

- **Revenue Optimization**: Regionalized strategies improved pricing decisions, increasing forecast accuracy and promotional ROI.
- **Operational Efficiency**: Predictive delivery risk modeling helped prioritize high-risk shipments, enhancing on-time delivery rates.
- **Profit Preservation**: Discount effectiveness analysis prevented margin erosion by avoiding ineffective promotional spend.

---

