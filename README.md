# Cafe Sales Data Audit & Revenue Analysis

## Executive Summary

Audited 10,000 raw cafe transaction records from the Kaggle Cafe Sales dataset and identified widespread missing values (including 502 unrecorded `Total Spent` entries, 919 missing `Item` labels, and 3,757 missing `Location` records), placeholder text errors (`ERROR`, `UNKNOWN`), and unverified outlier anomalies. Standardized the ledger by stripping invalid placeholder strings into proper null formats, verifying mathematical consistency across unit prices and quantities, and applying outlier screening (`Outlier_Flag = "No"`) across all 10,000 records to ensure 100% calculation accuracy. After cleaning and standardizing the dataset ($84,763.50 in total recorded revenue), food staples led by **Salad** ($16,605.00), **Sandwich** ($12,956.00), and **Smoothie** ($12,556.00) accounted for **49.7%** of total revenue (and **55.0%** of revenue among identified items), with **In-Store** ($25,906.00) and **Takeaway** ($25,229.50) performing nearly evenly across known service channels.

---

## Key Metrics Snapshot

* **Total Records Audited:** 10,000 (0 flagged outliers excluded)
* **Total Recorded Revenue (`Total Spent`):** $84,763.50 (across 9,498 valid spend records)
* **Top Revenue Driver:** Salad ($16,605.00 total; $5,405.00 In-Store / $4,835.00 Takeaway / $6,365.00 Unassigned Location)
* **Channel Split (Known Locations):** In-Store ($25,906.00) vs. Takeaway ($25,229.50)