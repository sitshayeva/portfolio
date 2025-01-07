
# **Market Basket Analysis for Marketing**
## **Project Report**

### **1. Introduction**
Market Basket Analysis (MBA) is a cornerstone in understanding customer purchasing patterns and leveraging those insights for strategic marketing. This project uses transactional data from "The Bread Basket," a bakery in Edinburgh, to perform MBA. The analysis identifies product associations and purchasing trends using data visualization and the Apriori algorithm, providing actionable insights for product placement, promotional offers, and sales recommendations.

---

### **2. Project Objectives**
- Analyze transactional data to identify purchasing patterns.
- Generate association rules using the Apriori algorithm.
- Visualize results using classical data visualization techniques and dynamic association rule graphs.

---

### **3. Dataset Overview**
#### Source:
- Dataset from [Kaggle: The Bread Basket](https://www.kaggle.com/mittalvasu95/the-bread-basket)
- License: CC0: Public Domain

#### Structure:
- **Total Rows**: 20,507
- **Columns**: 5 (`Transaction`, `Item`, `date_time`, `period_day`, `weekday_weekend`)
- **Unique Transactions**: 9,465
- **Product Types**: 94

#### Column Details:
- `Transaction`: Unique identifier for each transaction.
- `Item`: Products purchased in each transaction.
- `date_time`: Date and time of purchase.
- `period_day`: Categorization into parts of the day (morning, afternoon, etc.).
- `weekday_weekend`: Indicates whether the purchase occurred on a weekday or weekend.

---

### **4. Data Preprocessing**
- **Date Conversion**: Converted `date_time` to `datetime` format for accurate time-series analysis.
- **Feature Engineering**:
  - Extracted new columns: `hour`, `month`, `month name`, `day`, `weekday`, and `weekday name`.
  - Aggregated data to create a structured format for transactional analysis.

---

### **5. Analysis and Visualizations**

#### **5.1. Popular Items**
- **Top Items**:
  - Coffee: 26.68%
  - Bread: 16.21%
  - Tea: 6.99%
- **Visuals**: Bar plot highlighting the top 20 purchased items.

#### **5.2. Temporal Trends**
- **Monthly Trends**:
  - Peak months: March and November.
  - Seasonal insight: Winter sees the highest activity, while summer is the least active.
- **Weekly Trends**:
  - Most purchases occur on Saturdays.
- **Daily Trends**:
  - Highest activity between 9 AM and 4 PM.
  - Afternoon purchases dominate.

#### **5.3. Weekday vs. Weekend**
- **Distribution**:
  - Weekday: 62%
  - Weekend: 37%
- **Visuals**:
  - Pie charts for overall distribution and top products.

---

### **6. Association Rule Mining**
#### **6.1. Methodology**
- **Frequent Itemsets**: Generated using the Apriori algorithm with a minimum support threshold of 1%.
- **Key Metrics**:
  - **Support**: Frequency of itemsets in transactions.
  - **Confidence**: Likelihood of consequent given antecedent.
  - **Lift**: Strength of association between antecedent and consequent.
  - **Conviction**: Dependence of consequent on antecedent.

#### **6.2. Key Rules**
- **Most Frequent Rules**:
  - {Coffee} → {Bread} (Support: 9%)
  - {Pastry, Bread, Coffee} → {Cake} (Support: 1%)
- **High Confidence Rules**:
  - {Toast} → {Coffee} (Confidence: 70%)
  - {Cake} → {Tea} (Confidence: 22%)

#### **6.3. Refined Insights**
- Excluded dominant rules involving Coffee to uncover less obvious associations.
- Examples:
  - {Cake} → {Tea} (Lift: 1.60)
  - {Pastry} → {Bread} (Confidence: 33%)

---

### **7. Visualization of Association Rules**
#### **7.1. Dynamic Graphs**
- Visualized association rules using the `pyvis` library.
- **Graph Features**:
  - Node size: Represents support.
  - Edge thickness: Represents confidence.
  - Interactive elements: Smooth edges, hover information.

#### **7.2. Interpretation**
- Enabled clear understanding of complex relationships.
- Highlighted strong associations and key insights visually.

---

### **8. Recommendations**
- **Product Placement**:
  - Coffee and Bread should be placed nearby due to their strong association.
  - Cake and Tea can be strategically positioned together for cross-selling.
- **Promotional Offers**:
  - Discounts on Coffee with Cake or Tea could drive sales.
- **Inventory Management**:
  - Focus on high-demand periods (afternoons, Saturdays, winter months).

---

### **9. Conclusion**
This analysis demonstrates how MBA transforms transactional data into actionable insights. Using visualizations and association rule mining, we identified purchasing patterns, strong associations, and optimal product recommendations. These insights can help "The Bread Basket" enhance its marketing strategy, optimize store layout, and increase sales.

---

### **10. Future Scope**
- Extend the analysis to incorporate seasonal promotions.
- Explore clustering techniques for customer segmentation.
- Analyze the impact of external factors (e.g., weather, holidays) on purchasing patterns.

---

