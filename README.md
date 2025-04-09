# E-commerce Campaign Performance: Time Series and Correlation Analysis

## Overview
* This project combines time series and correlation analysis to evaluate e-commerce campaign performance metrics from September 2024 to March 2025. The analysis focuses on temporal trends and relationships between key performance indicators including Average Order Value (AOV), Return on Ad Spend (ROAS), and conversion rates.

### Analysis Types

1. Time Series Analysis
   
   What this means:
   - Analyzing how metrics change over time (e.g., how AOV changes month by month)
   - Comparing performance between different time periods (e.g., before and after holiday season)
   - Tracking monthly changes in key metrics and identifying seasonal patterns
   - Creating visual predictions with confidence ranges
   - Breaking down trends into long-term patterns and short-term fluctuations

   Why:
   - Identifies patterns and cycles in campaign performance
   - Enables accurate forecasting of future performance
   - Helps detect anomalies and performance issues early
   - Reveals seasonal impacts on campaign effectiveness

   Benefits:
   - Better budget allocation based on historical performance
   - Proactive campaign optimization
   - Improved ROI through timing optimization
   - Early warning system for performance degradation
   - Data-driven decision making for campaign scheduling

2. Correlation Analysis

   What this means:
   - Understanding how different metrics influence each other (e.g., how ad spend affects sales)
   - Identifying which metrics depend on others
   - Creating a comprehensive view of how all metrics relate to each other
   - Testing whether relationships between metrics are statistically valid
   - Measuring the strength and direction of relationships between metrics

   Why:
   - Uncovers hidden relationships between metrics
   - Identifies key drivers of performance
   - Validates or challenges assumed metric relationships
   - Helps prioritize optimization efforts

   Benefits:
   - More efficient budget allocation
   - Better targeting strategies
   - Improved campaign optimization focus
   - Risk mitigation through understanding metric dependencies
   - Enhanced reporting accuracy

3. Statistical Testing

   What this means:
   - Comparing different time periods to confirm real performance changes
   - Calculating ranges where true values likely fall
   - Verifying if changes in metrics are meaningful or just random
   - Understanding how metrics are distributed across their range

   Why:
   - Validates performance changes statistically
   - Ensures decisions are based on significant data
   - Reduces impact of random variations
   - Provides confidence levels for findings

   Benefits:
   - More reliable decision making
   - Reduced risk of false conclusions
   - Better justification for strategy changes
   - Quantifiable confidence in results

4. Performance Metrics Analysis

   What this means:
   - Deep dive into campaign results over specific time periods
   - Tracking return on advertising spend over time
   - Understanding how many clicks turn into actual sales
   - Measuring how efficiently money is being spent on advertising

   Why:
   - Provides comprehensive performance overview
   - Tracks ROI and efficiency metrics
   - Identifies areas for improvement
   - Enables performance benchmarking

   Benefits:
   - Clear performance accountability
   - Easy identification of optimization opportunities
   - Better stakeholder communication
   - Improved campaign strategy development

5. Trend Visualization

   What this means:
   - Creating clear visual representations of how average order value changes
   - Showing return on ad spend performance through graphs
   - Displaying relationships between metrics through color-coded maps
   - Plotting how metrics change over time in easy-to-understand charts

   Why:
   - Makes complex data relationships visible
   - Enables quick pattern recognition
   - Facilitates stakeholder communication
   - Supports intuitive decision making

   Benefits:
   - Faster insights discovery
   - Better presentation of findings
   - Improved stakeholder understanding
   - More effective reporting

### Business Impact

The combination of these analysis types delivers several key business advantages:

1. Strategic Benefits:
   - Data-driven decision making
   - Improved campaign planning
   - Better resource allocation
   - Enhanced performance prediction

2. Operational Benefits:
   - Real-time performance monitoring
   - Quick issue identification
   - Efficient optimization process
   - Better timing of campaign changes

3. Financial Benefits:
   - Improved ROI through better targeting
   - Reduced waste in ad spend
   - More efficient budget allocation
   - Better cost control

4. Organizational Benefits:
   - Clear performance communication
   - Better stakeholder alignment
   - Improved team coordination
   - Data-backed strategy discussions

## Technical Details

### Dependencies
- pandas (1.5.0+): Data manipulation and analysis
- matplotlib (3.5.0+): Basic plotting and visualization
- seaborn (0.12.0+): Advanced statistical visualizations
- scipy (1.9.0+): Statistical computations and testing

### Installation
```bash
# Create a virtual environment (recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install pandas matplotlib seaborn scipy
```

## Data Source Details
The analysis uses campaign performance data from `Resources/Campaign performance - Campaign performance.csv`

### Data Schema
| Column Name      | Description                              | Data Type |
|-----------------|------------------------------------------|-----------|
| Year            | Campaign year                            | Integer   |
| Month           | Campaign month                           | String    |
| Cost            | Total ad spend                           | Float     |
| Impr.           | Total impressions                        | Integer   |
| Clicks          | Total clicks received                    | Integer   |
| CTR             | Click-through rate                       | Percentage|
| Avg. CPC        | Average cost per click                   | Float     |
| Conversions     | Total conversions                        | Float     |
| Conv. value     | Total conversion value                   | Float     |
| Cost / conv.    | Cost per conversion                      | Float     |
| Conv. rate      | Conversion rate                          | Percentage|
| Conv. value/cost| Return on ad spend (ROAS)               | Float     |

## Detailed Findings

### AOV (Average Order Value) Analysis
- Campaign Period: September 2024 to March 2025
- Highest AOV: $652.94 (November 2024)
  - 9.2% above period average
  - Driven by holiday season shopping
- Lowest AOV: $563.37 (December 2024)
  - 5.8% below period average
  - Potential impact of holiday discounts
- Average AOV across period: $597.82
- Statistical Analysis:
  - Pre-December vs Post-December comparison
  - Significant decrease of $89.57 in AOV (p < 0.05)
  - 13.7% decline in average order value

### ROAS Performance Breakdown
- Average ROAS: 10.43x
- Monthly Performance:
  - September 2024: 12.83x (Peak)
  - October 2024: 10.31x
  - November 2024: 12.30x
  - December 2024: 9.49x
  - January 2025: 9.99x
  - February 2025: 9.88x
  - March 2025: 8.19x (Lowest)
- Overall decline: 36.2% from peak to lowest

### Detailed Conversion Metrics
- Average Conversion Rate: 1.19%
- Monthly Breakdown:
  - September 2024: 1.58% (Best)
  - October 2024: 1.25%
  - November 2024: 1.03%
  - December 2024: 1.03% (Tied Lowest)
  - January 2025: 1.21%
  - February 2025: 1.19%
  - March 2025: 1.07%

### Advanced Correlation Analysis
Correlation coefficients between key metrics:
- AOV & ROAS: +0.82 (Strong positive)
- Clicks & Cost: +0.91 (Very strong positive)
- Conversions & Cost: +0.88 (Strong positive)
- CTR & Conversion Rate: +0.45 (Moderate positive)

### Detailed Campaign Performance Trends
1. ROAS Decline Analysis:
   - 36.2% total decline (12.83x to 8.19x)
   - Average monthly decline: 6.03%
   - Steepest decline: December 2024 (-22.8%)

2. CTR Performance:
   - Average: 1.76%
   - Standard deviation: 0.06%
   - Range: 1.68% - 1.86%

3. Cost Efficiency Metrics:
   - Initial cost per conversion: $29.41
   - Final cost per conversion: $49.77
   - Total increase: 69.2%
   - Monthly average increase: 11.5%

## Implementation Guide

### Setup Instructions
1. Clone the repository:
```bash
git clone https://github.com/yourusername/e-commerce-campaign-analysis.git
cd e-commerce-campaign-analysis
```

2. Create and activate virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Configure data path:
   - Open `template.ipynb`
   - Update file_path variable to match your local setup

### Running the Analysis
1. Launch Jupyter Notebook:
```bash
jupyter notebook
```

2. Open `E-commerce Campaign Performance Analysis.ipynb`
3. Run all cells sequentially
4. Generated outputs will be saved in the project root directory

## Output Files
The analysis generates the following outputs:
1. Visualizations:
   - `AOV_trend_plot.png`: AOV trends over time
   - `ROAS_trend_plot.png`: ROAS performance visualization
   - `correlation_heatmap.png`: Metric correlations
   
2. Statistical Reports:
   - T-test results for AOV analysis
   - Correlation coefficients matrix
   - Monthly performance summaries

