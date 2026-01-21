# 📦 Inventory Risk Control System (Excel)

## 🧩 Problem  
Raw inventory and supplier data contained duplicates, missing values, and inconsistent product records.  
Using this data directly would lead to incorrect stock levels, false shortage alerts, and wrong business decisions.

## 🎯 Objective  
Build a controlled pipeline that transforms messy inventory data into reliable, decision-ready outputs while preventing bad data from silently reaching reports.

## 🚨 Data Issues Identified  
- Duplicate product records  
- Missing stock values  
- Inconsistent product naming  
- Mismatched supplier entries  
- Totals not aligning across sheets  

## 🛠️ Approach  
1. Separated raw data from clean working sheets  
2. Standardized product and supplier fields  
3. Built validation layers to detect:  
   - Missing values  
   - Duplicate records  
   - Mismatched totals  
4. Designed repeatable formulas using Excel logic  
5. Created structured summaries for operational review  
6. Connected the clean layer to Power BI for reporting  

## 🛡️ Validation & Control Logic  
- Record count checks between raw and clean layers  
- Duplicate detection rules  
- Null-value flags for critical fields  
- Reconciliation totals to detect silent breakage  

Any failed check **stops the pipeline**.

## 📊 Output  
- Clean inventory dataset  
- Risk indicators for overstock and stock-out  
- Operational dashboard for decision-making  

## 💡 Why This Matters  
In real environments, data is never clean.  
This project is designed to behave like a production system:  
- It expects failure  
- It surfaces errors  
- It prevents silent corruption  
- It protects downstream users  

The goal is not visualization.  
The goal is **trust**.

## 🧰 Tools Used  
- **MS Excel** – Cleaning, Mapping, Validation, Reconciliation  
- **Power BI** – Data Modeling, Relationships, Risk Dashboard  
