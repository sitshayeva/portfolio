# A/B Test Dashboard – E-Commerce - Landing Page

[<img src="https://github.com/sitshayeva/portfolio/blob/main/images/60.png" width="400" height="250">](https://huggingface.co/spaces/lenaras/ab_test_analysis_ecommerce_landing_page)


**Streamlit Application:** https://huggingface.co/spaces/lenaras/ab_test_analysis_ecommerce_landing_page

## 🧠 Key Questions

- Does the **new landing page** significantly increase conversion?
- Are **conversion rates different by country**?
- Are there **time-based trends** in user conversions?
- Can we build **predictive models** to anticipate conversions?
- Can **multi-armed bandits** outperform traditional A/B testing?

---

## 🧹 Steps Performed

### ✅ 1. Data Cleaning
- Removed mismatched group/page assignments.
- Deduplicated `user_id`s.

### 📊 2. Conversion Analysis
- Calculated group-wise conversion rates.
- Constructed confidence intervals.
- Performed Z-tests and logistic regression.

### ⏱️ 3. Time-Based Trends
- Hourly, daily, and weekday conversion patterns visualized.

### 🗺️ 4. Geo-Based Analysis
- Country-level conversion comparisons with heatmaps and bar charts.
- Country-specific Z-tests and interaction modeling.

### 🧪 5. Multi-Armed Bandit Simulation
- Simulated Thompson Sampling vs. traditional A/B testing.
- Analyzed regret over time.

### 🤖 6. Predictive Modeling
- Trained RandomForest, LightGBM, and XGBoost models.
- Engineered features from group, page, time, and country.
- Evaluated models using AUC, F1-score, and SHAP values.

---

## 📈 Results Summary

- **Observed Difference:** ~0.0016
- **95% Confidence Interval:** (-0.0039, 0.00078)
- **Test Power:** ~26%
- **Conclusion:** No statistically significant impact of the new page at α = 0.05.

---

## 🧭 Recommendations

1. **Increase Sample Size**  
   - Power was only ~26%. Use power calculators to plan future tests.

2. **Segment Users**  
   - Analyze by country, time of day, traffic source, or device.

3. **Improve Sensitivity**  
   - Use CUPED or covariate adjustment.
   - Track continuous metrics like revenue/time on page.

4. **Try More Impactful Variants**  
   - Test changes to layout, content, or personalization.

5. **Consider Bayesian or Sequential Testing**  
   - Allows early stopping and more adaptive decision-making.

