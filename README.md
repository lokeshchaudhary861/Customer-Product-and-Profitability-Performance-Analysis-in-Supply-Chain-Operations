# 📊 APL Logistics Financial Performance Dashboard

An end-to-end data pipeline and dynamic business intelligence web application built for **APL Logistics** to isolate global revenue leaks, track regional profit concentration, and simulate promotional margin recovery.

---

## ⚙️ Core Architecture & Features

*   **Data Engine (`Google Colab`):** Cleans, type-validates, and optimizes raw data (`APL_Logistics_2.csv`) using byte-resilient `latin1` parsing to output a high-performance production dataset while protecting ML workflows from target leakage.
*   **Interactive Canvas (`Streamlit`):** A lightweight, single-page scroll-down layout equipped with multi-layered global cross-filters (Market, Region, Customer Segment, Categories, Products, and Discount Rates) that eliminates UI latency.
*   **Analytical Modules:**
    1.  *Financial Performance:* Macro KPI monitoring and Regional Revenue vs. Net Profit mapping.
    2.  *Customer Value Dashboard:* Side-by-side analysis of the top 10 most profitable vs. bottom 10 loss-making accounts based on a custom *Customer Value Index* ($CVI$).
    3.  *Product Portfolio Performance:* Margin-to-revenue density heatmaps and low-margin product risk watchlists.
    4.  *Strategic "What-If" Simulator:* Interactive slider enabling stakeholders to reduce active discount rates ($0\text{--}100\%$) to instantly project simulated profit lift and margin recovery.

---

## 💻 Tech Stack & Deployment

*   **Tools:** Python, Pandas, NumPy, Scikit-Learn, Streamlit, Plotly

```bash
# Install dependencies
pip install streamlit pandas numpy plotly

# Deploy application locally
streamlit run app.py
