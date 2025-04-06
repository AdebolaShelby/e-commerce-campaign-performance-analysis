# E-commerce Campaign Performance: Time Series and Correlation Analysis

## Overview
This project combines time series and correlation analysis to evaluate e-commerce campaign performance metrics from September 2024 to March 2025. The analysis focuses on temporal trends and relationships between key performance indicators including Average Order Value (AOV), Return on Ad Spend (ROAS), and conversion rates.

### Analysis Types
1. Time Series Analysis
   - Temporal trends in AOV and ROAS
   - Before/after performance comparisons
   - Monthly metric tracking
   - Trend visualization

2. Correlation Analysis
   - Relationships between key metrics
   - Performance indicator dependencies
   - Multi-variable correlation matrix
   - Statistical significance testing

## Features
- AOV trend analysis and visualization
- Statistical comparison of pre/post December 2024 performance
- Correlation analysis between key metrics
- Comprehensive campaign performance summary

## Dependencies
- pandas
- matplotlib
- seaborn
- scipy

## Data Source
The analysis uses campaign performance data from `Resources/Campaign performance - Campaign performance.csv` containing the following metrics:
- Year and Month
- Cost
- Impressions
- Clicks
- CTR (Click-Through Rate)
- Conversions
- Conversion Value
- ROAS (Return on Ad Spend)

## Key Findings

### AOV (Average Order Value) Analysis
- Campaign Period: September 2024 to March 2025
- Highest AOV: $652.94 (November 2024)
- Lowest AOV: $563.37 (December 2024)
- Average AOV across period: $597.82
- Pre-December vs Post-December comparison shows a decrease of $89.57 in AOV

### ROAS (Return on Ad Spend) Performance
- Average ROAS: 10.43x
- Highest ROAS: 12.83x (September 2024)
- Declining trend observed from September 2024 (12.83x) to March 2025 (8.19x)

### Conversion Metrics
- Average Conversion Rate: 1.19%
- Best performing month: September 2024 (1.58%)
- Lowest performing month: November/December 2024 (1.03%)

### Correlation Analysis Highlights
Strong correlations identified between:
- AOV and ROAS (positive correlation)
- Clicks and Cost (positive correlation)
- Conversions and Cost (positive correlation)

### Campaign Performance Trends
- Overall declining trend in ROAS
- Consistent CTR averaging 1.76%
- Cost per conversion increased from $29.41 to $49.77

### Recommendations
1. Investigate December 2024 performance drop
2. Focus on improving conversion rates to counter declining ROAS
3. Optimize cost per conversion which has shown an upward trend
4. Consider adjusting strategy to improve AOV in post-December period

## Key Analyses

### 1. AOV Analysis
- Tracks Average Order Value trends over time
- Performs statistical t-test comparison before/after December 2024
- Visualizes AOV trends with line plots

### 2. Correlation Analysis
Examines relationships between:
- AOV (Average Order Value)
- CTR (Click-Through Rate)
- Cost
- Clicks
- Conversions
- ROAS

### 3. Performance Metrics
- Campaign period analysis
- ROAS tracking
- Conversion rate analysis

## File Structure
```
project/
│
├── template.ipynb          # Main analysis notebook
│
└── Resources/
    └── Campaign performance - Campaign performance.csv    # Source data
```

## Usage
1. Ensure all dependencies are installed:
```bash
pip install pandas matplotlib seaborn scipy
```

2. Update the file path in `template.ipynb` to match your local data location
3. Run the notebook cells sequentially

## Output
The analysis generates:
- Visualizations of AOV trends
- Statistical test results
- Correlation heatmap
- Comprehensive performance summary





