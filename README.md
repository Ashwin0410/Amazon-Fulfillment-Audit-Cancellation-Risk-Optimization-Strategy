# Amazon-Fulfillment-Audit-Cancellation-Risk-Optimization-Strategy

This project is a deep-dive audit into **where Amazon orders are failing** — and how fulfillment method, product category, and location contribute to cancellations.

Rather than just exploring the data, we go further:  
We simulate **what would happen if we rerouted risky orders from Merchant to Amazon fulfillment** — and prove how that one small change could reduce cancellations and protect revenue.

---

## Key Business Questions Answered

1. **Which product categories have the highest cancellation rates?**  
   → Some top-selling items are also the most cancelled — that’s a problem.

2. **Which cities or states are most prone to failures?**  
   → Geo-level patterns show fulfillment performance varies heavily by region.

3. **Does fulfillment method (Amazon vs Merchant) affect reliability?**  
   → Yes. Merchant fulfillment has significantly higher cancellation rates in certain states.

4. **Are our best-selling products also at risk?**  
   → Revenue-generating categories like Sets and Kurtas are also major cancellation contributors.

5. **What happens if we change fulfillment logic in high-risk zones?**  
   → Simulation shows that rerouting Merchant orders in 12 states could prevent **~48% of failed orders**, recovering ₹16,525 in revenue.

---

## Dataset Overview
Link - http://kaggle.com/datasets/thedevastator/unlock-profits-with-e-commerce-sales-data

- Source: Amazon order-level sales export  
- Rows: 128,975 orders  
- Columns include:
  - Order details (ID, status, amount)
  - Product category & SKU
  - Fulfillment method (Amazon vs Merchant)
  - Shipping location (city, state, postal code)
  - Dates & timestamps

---

## Techniques Used

- Data Cleaning & Preprocessing (`pandas`, `numpy`)
- Feature Engineering:
  - `Is_Cancelled`, `Is_High_Value`, `Cancel_Rate (%)`, `Revenue_At_Risk (%)`
- Visualizations:
  - Bar charts, boxplots, trendlines, pie charts (via `matplotlib`, `seaborn`)
- Simulation:
  - Merchant → Amazon rerouting strategy
  - Cancel rate comparison + revenue recovery estimation
- Geo and Category segmentation
- Business commentary + strategy recommendations

---

## Key Takeaways

- **47.7% of failed orders** could have been saved with a better fulfillment strategy
- **High-value orders are getting cancelled more often under Merchant**
- Building a fulfillment decision model by state could meaningfully reduce customer churn and revenue loss

---

## Files Included

- `Amazon_Fulfillment_Audit_Cancellation_Risk_&_Optimization_Strategy.ipynb` – the full Jupyter notebook
- Visualizations & charts throughout
- Final conclusions and action-ready recommendations

---

## Author Notes

This project was built to reflect **real-world analytics consulting**:  
Not just charts, but **insights, impact, and a clear recommendation path**.

It’s designed to be decision-driven — and it simulates change, not just observes data.

---

## Tags

`EDA` `Data Analysis` `Fulfillment Strategy` `Amazon Orders` `Cancellations`  
`Pandas` `Seaborn` `Simulation` `Business Analytics` `Logistics Optimization`

