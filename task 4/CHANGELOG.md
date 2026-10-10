# Changelog

## Week 4 — Market-Basket Analysis & Association Rules

- Prepared transaction data for market-basket analysis.
- Examined service frequencies and applied a minimum item-support threshold.
- Compared FP-Growth results at 1%, 2%, and 5% minimum support.
- Filtered association rules using lift and confidence thresholds and removed trivial or redundant rules.
- Evaluated rule stability across different months and validated selected rules on a separate time period.
- Developed cross-selling recommendations based on the selected association rules.
- Estimated potential additional revenue under conservative (5%), moderate (10%), and optimistic (20%) conversion-uplift scenarios, using the documented discount assumption.
- Documented the limitations of simulated data and scenario-based revenue estimates.
- Exported filtered association rules, one-to-one rules, and recommended bundles to CSV files.

## Final Verification — To Complete

- Record the actual number of frequent itemsets or rules found at each minimum-support level.
- Record the actual second-period validation results, including rules that remained strong and those that weakened.
- Document any errors discovered, corrections made, and final testing outcomes.
- Confirm that the notebook runs successfully from beginning to end and that all required outputs are saved.
