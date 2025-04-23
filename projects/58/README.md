
**A/B Testing Campaign Analysis – Execution Report**

**Streamlit Application:**  https://huggingface.co/spaces/lenaras/ab_testing_campaign_analysis

**Objective:**  
Evaluate two campaign strategies (Control and Test) based on key marketing metrics to determine which yields higher returns, better conversions, and more efficient user engagement.

---

**1. Data Summary & Cleaning**
- Datasets from both campaigns were cleaned by removing missing values.
- Metrics like `Conversion Rate` and `ROAS` (Return on Ad Spend) were calculated:
  - **Conversion Rate = Purchases / Website Clicks**
  - **ROAS = Purchases / Spend**

---

**2. Summary Statistics**
| Metric           | Group    | Mean     | Std Dev  | Sample Size |
|------------------|----------|----------|----------|--------------|
| Conversion Rate  | Control  | 11.48%   | 6.84%    | 29           |
|                  | Test     | 9.23%    | 4.45%    | 30           |
| ROAS             | Control  | 0.232    | 0.091    | 29           |
|                  | Test     | 0.207    | 0.088    | 30           |

---

**3. Statistical Testing**
- **T-Test p-values:**
  - Conversion Rate: **0.143** (not significant)
  - ROAS: **0.280** (not significant)
- **Interpretation:**
  - Differences between Control and Test groups are not statistically significant (p > 0.05).

---

**4. Confidence Intervals (95%)**
| Metric           | Group    | CI Lower | CI Upper |
|------------------|----------|----------|----------|
| Conversion Rate  | Control  | 8.88%    | 14.08%   |
|                  | Test     | 7.57%    | 10.89%   |
| ROAS             | Control  | 0.197    | 0.267    |
|                  | Test     | 0.174    | 0.239    |
- **Overlap of intervals** reinforces lack of statistical significance.

---

**5. Funnel Efficiency**
Control group outperformed Test group across the full conversion funnel:
- CTR, Search Rate, Content View Rate, Add-to-Cart Rate, Final Purchase Rate.

---

**6. Daily Performance Stability**
| Group   | Conversion Rate Std | CTR Std | ROAS Std |
|---------|----------------------|---------|----------|
| Control | 6.84%                | 2.05%   | 9.13%    |
| Test    | 4.45%                | 6.77%   | 8.80%    |
- Test group showed more CTR fluctuation, suggesting less stable performance.

---

**7. Spend Efficiency**
**Correlation Matrix Highlights:**
- ROAS vs Spend: **-0.35** → Higher spend may lead to diminishing returns.
- ROAS vs Purchases: **+0.91** → ROAS is highly dependent on number of purchases.

---

**8. Predictive Modeling**
Top predictors for Purchases (Linear Regression Coefficients):
1. **# of Add to Cart** → 0.22
2. **# of Searches** → 0.06
3. **Spend** → 0.05

Negative or negligible influence:
- Impressions, Reach, View Content, Website Clicks

---

**9. Clustering & Ad Fatigue**
- **3 performance clusters** revealed:
  - High-performing days (often Control)
  - Medium and low-performing days (Test-heavy)
- **Rolling CTR and ROAS** showed mild **decline over time**, suggesting ad fatigue.

---

**10. Visual Insights Analysis**

**Funnel Efficiency (output.png):**
- Test group has higher CTR, but Control outperforms in all other stages.
- Indicates better guidance through the funnel by the Control group.

**Purchase Efficiency (output2.png):**
- Test group occasionally spikes in Purchase per Impression and Reach.
- Lacks consistency compared to Control.

**Cumulative Trends (output3.png):**
- Test spends more and gets more volume.
- However, spend efficiency does not clearly surpass the Control.

**Daily Metrics (output4.png):**
- Control is more consistent in Conversion and ROAS.
- Test group shows more volatility.

**Zoomed Cumulative View (output5.png):**
- Reaffirms volume advantage of Test, but questions cost-effectiveness.

**Clustering Analysis (output6.png):**
- Control dominates high-performance clusters.
- Test group appears mostly in low-efficiency clusters.

**ROAS vs Spend (output7.png):**
- Negative trend: more spend, lower ROAS.
- Test campaign often below trend line.

**Confidence Intervals (output1.png):**
- Overlapping CIs confirm no significant advantage.
- Control group estimates are slightly better and more stable.

---

**Conclusion & Recommendation**
- **Control Campaign performs more efficiently and consistently.**
- **Test Campaign** does not significantly outperform in conversions or ROI.

**Recommendation:**
- Continue with **Control strategy**.
- Improve Test Campaign design (creative, targeting, budget pacing).
- Explore segmented A/B testing for further granularity.

---

**Next Steps**
- Deploy creative and audience segment testing.
- Automate performance monitoring.
- Implement predictive metrics into dashboard tracking.
