# Supply_Chain_Management_SkillCircle
## Project Objective
As a data analyst, your role is to verify if the charges levied by courier partners for each shipment made by Company X are correct, using internal order data, SKU weights, zone mappings, and courier invoice files.

---

## Project Structure
```
Cointab_Supply_Chain_Challenge/
├── Cointab_Supply_Chain_Challenge.ipynb   # Main notebook with full solution
├── requirements.txt                        # Python dependencies
├── README.md                               # Project overview and usage
├── Company X - Order Report.xlsx
├── Company X - SKU Master.xlsx
├── Company X - Pincode Zones.xlsx
├── Courier Company - Invoice.xlsx
├── Courier Company - Rates.xlsx
├── output/
│   ├── order_level_analysis.xlsx           # Per-order charge validation
│   └── summary_table.xlsx                  # Summary of overcharges, undercharges
```

---

## How to Run

1. Install required packages:
```bash
pip install -r requirements.txt
```

2. Place all dataset Excel files in the project root directory.
3. Open and run `Cointab_Supply_Chain_Challenge.ipynb`.
4. Check the `/output/` folder for generated results.

---

## Input Data
- Website Order Report: Product list per order
- SKU Master: Weight (g) per SKU
- Pincode Zones: Zone classification based on warehouse and customer pincodes
- Courier Invoice: Billed weights, charges, delivery zone
- Rate Card: Zone- and weight-based forward/RTO charge rates

---

## Output Files
- `order_level_analysis.xlsx`: All order-wise validation details
- `summary_table.xlsx`: Aggregated counts of charge correctness

---

## Key Features
- Accurate calculation of weight slabs in 0.5 KG intervals
- Zone mapping validation
- Expected charge computation using courier rate card
- Identification of overcharged and undercharged shipments
- Final business recommendations

---

## Summary Insights
- Helps identify courier inefficiencies
- Enables contract renegotiation backed by data
- Supports automation of invoice validation

---

## Recommendations
- Automate this script as a monthly audit pipeline
- Investigate high-RTO zones for root causes
- Flag and review partners with frequent overcharging
- Integrate this validation into finance/ERP system

---

## Dataset Source
[Google Drive Dataset](https://drive.google.com/file/d/1NjYY0t8ed4fcLEvgQl9DIqFluUkVL3GF/view)

---
