# Project Summary

The Wedding Planner Market-Basket Analysis project explores which wedding services tend to be purchased together and how those relationships can inform cross-selling decisions. The analysis uses Python, Pandas, Matplotlib, and MLxtend to prepare transaction baskets, apply FP-Growth, and generate association rules measured using support, confidence, and lift.

Three minimum-support thresholds are compared to understand how the threshold affects the number of rules discovered. Rules with lift above 1.2 are considered for further analysis, while trivial or redundant relationships are filtered according to the notebook's documented criteria. The main analysis uses January–June 2025, with July–December 2025 used for out-of-time validation.

The final recommendations identify service combinations that could be offered as bundles or add-ons. Their potential revenue is estimated using 5%, 10%, and 20% conversion scenarios and an assumed 10% discount. These figures are hypothetical projections rather than measured business outcomes.

The main limitation is that the dataset is simulated. Real booking records and controlled experiments would be needed to confirm the associations and estimate actual incremental revenue. This project demonstrates a market-basket analysis workflow and translates its findings into practical business recommendations.