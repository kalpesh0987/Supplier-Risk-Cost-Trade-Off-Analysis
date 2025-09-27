# Supplier Risk & Cost Trade-Off Analysis

This project analyzes suppliers based on cost, risk, reliability, and sustainability to support strategic sourcing decisions. It highlights the trade-off between choosing low-cost but high-risk suppliers versus more reliable but expensive ones.

---

## Project Overview
- **Objective**: Identify an optimal set of suppliers by balancing procurement cost and supplier risk.  
- **Approach**:  
  - Data exploration of supplier cost, risk, and performance metrics.  
  - Visualization of risk versus cost.  
  - Scoring model that integrates cost efficiency, risk exposure, and sustainability.  
- **Outcome**: A framework for supplier segmentation and selection.

---

## Dataset
The dataset `suppliers_risk.csv` contains synthetic supplier information:
- Supplier, Country  
- UnitCost (per unit)  
- RiskScore (0–100, higher = riskier)  
- Reliability (%)  
- Sustainability (%)  

---

## Methodology
1. Load and explore supplier data.  
2. Compare suppliers on cost and risk using scatterplots.  
3. Apply a weighted scoring model:  
   `Score = 0.6*(1/Cost) + 0.3*(1/Risk) + 0.1*(Sustainability)`  
4. Visualize reliability and sustainability to assess supplier balance.  

---

## Tech Stack
- Python  
- Libraries: `pandas`, `matplotlib`, `seaborn`  

---

## How to Run
```bash
# Clone repository
git clone https://github.com/yourusername/supplier-risk-analysis.git
cd supplier-risk-analysis

# Install dependencies
pip install pandas matplotlib seaborn jupyter

# Run the notebook
jupyter notebook supplier_risk_analysis.ipynb
