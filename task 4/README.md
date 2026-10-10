# Wedding Planner Market-Basket Analysis & Association Rules

## Project Overview

This project uses market-basket analysis to identify wedding-planning services that are frequently purchased together. The objective is to develop data-driven cross-selling recommendations that could help an emerging wedding planner increase add-on sales and identify potential revenue opportunities.

The analysis applies the FP-Growth algorithm and association rules to discover relationships between services such as decoration, catering, photography, videography, floral design, lighting, and stage and backdrop services.

**Dataset note:** The transaction dataset used in this project is simulated for educational and analytical purposes. The results demonstrate a market-basket analysis workflow and should not be interpreted as verified purchasing behaviour from a real wedding-planning business.

## Project Objectives

- Analyse wedding service purchasing patterns.
- Identify frequently occurring combinations of services.
- Apply FP-Growth using different minimum-support thresholds.
- Evaluate association rules using support, confidence, and lift.
- Validate selected rules across separate time periods.
- Recommend actionable cross-selling bundles.
- Estimate potential additional revenue under different conversion scenarios.

## Tools and Technologies

- **Python** — analysis and calculations
- **Pandas and NumPy** — data preparation and manipulation
- **mlxtend** — FP-Growth and association-rule mining
- **Matplotlib and Seaborn** — data visualisation
- **Jupyter Notebook** — analysis workflow and documentation
- **GitHub** — project version control and portfolio presentation

## Methodology

### 1. Data Preparation
The transaction dataset was loaded and inspected. Services were organised into a basket representation, where each row represents a transaction and each service column indicates whether that service was included.

### 2. Service Frequency Analysis
Service frequencies were examined to understand which services appeared most often. A minimum item-support threshold was applied to reduce the influence of very rare services.

### 3. Frequent Itemset Mining
The FP-Growth algorithm was used to identify frequent service combinations. Three minimum-support thresholds were compared:

- 1% minimum support
- 2% minimum support
- 5% minimum support

This comparison helps demonstrate how the support threshold affects the number of frequent combinations discovered.

### 4. Association-Rule Generation
Association rules were generated from the frequent itemsets. Support, confidence, and lift were used to assess the frequency and strength of relationships between services.

Rules were filtered using the project's documented criteria, including lift greater than 1.2 and confidence of at least 0.30. Trivial, redundant, or unsuitable rules were excluded where appropriate.

### 5. Temporal Validation
Selected association rules were evaluated across different time periods, including January–June and July–December 2025. This helped assess whether the identified relationships remained useful beyond the initial mining period.

### 6. Cross-Selling Recommendations
The selected rules were converted into practical service recommendations. For example, customers booking decoration may be offered stage and backdrop services when the corresponding association is supported by the analysis.

### 7. Revenue Estimation
Potential additional revenue was estimated using three assumed conversion-uplift scenarios:

- **Conservative:** 5%
- **Moderate:** 10%
- **Optimistic:** 20%

These scenarios are estimates rather than measured campaign results. Revenue calculations depend on the assumptions and formula used in the notebook.

## Results

The final numerical results should be taken directly from the successfully executed notebook.

Key results to report include:

- Number of unique transaction baskets analysed
- Number of services analysed
- Frequent itemset counts at each minimum-support threshold
- Number of association rules retained after filtering
- Number of selected rules that passed the validation criteria
- Number of recommended cross-selling bundles
- Estimated additional revenue under the three conversion scenarios

The repository includes exported association-rule tables and recommended bundles to support verification of the findings.

## Revenue Assumptions

Revenue estimates use assumed add-on conversion uplifts of 5%, 10%, and 20%. They represent possible outcomes under different scenarios, not guaranteed increases in revenue.

The estimates should be interpreted cautiously because actual results may depend on customer behaviour, service pricing, discounts, profit margins, overlapping recommendations, and other business factors.

## Limitations

- The dataset is simulated and may not represent real customer purchasing behaviour.
- Association rules identify relationships between services but do not establish causation.
- Estimated revenue depends on assumptions rather than measured campaign performance.
- Patterns identified in the dataset may not generalise to a real business.
- Temporal validation can help assess stability, but it does not guarantee future performance.

## Future Improvements

With access to real booking data, this analysis could be improved by validating the discovered patterns against actual customer transactions, testing cross-selling recommendations through controlled experiments, incorporating service profit margins, and accounting more precisely for overlapping offers.

## Project Structure

```text
wedding-planner-market-basket-analysis/
│
├── Market_Basket_Analysis_Wedding_Planner_Reviewed.ipynb
├── wedding_planner_transactions.csv
├── README.md
├── SUMMARY.md
├── CHANGELOG.md
│
└── outputs/
    ├── association_rules.csv
    ├── association_rules_one_to_one.csv
    └── recommended_bundles.csv
```

*The file structure above describes the intended organisation. Confirm that each listed file exists in the repository before submission.*

## Conclusion

This project demonstrates how market-basket analysis can transform transaction data into practical cross-selling recommendations. By combining FP-Growth, association-rule metrics, temporal validation, and scenario-based revenue estimation, the analysis provides a structured way to identify service combinations that may be useful to an emerging wedding-planning business.