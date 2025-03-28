# NHL Value Forwards: Identifying Underpaid Players for Trade and Free Agency Targets

## Objective
Use NHL salary and performance data to identify **forwards who significantly outperform their contracts**, making them high-value targets for trades or free agency.

## Key Questions
- Which NHL forwards provide the most value per $1M of salary?
- How does play-driving (xGF%) relate to team success?
- What traits or metrics define an "undervalued" player?

##  Why It Matters
Teams constantly seek low-cost, high-impact players to build depth and stay under the cap. Identifying these players through data-driven analysis can give front offices a competitive edge.

## Project Structure
- `data/`: Raw and cleaned salary + performance data
- `notebooks/`: Data cleaning, metric creation, and visualizations
- `visuals/`: Value charts and scatter plots
- `README.md`: Summary of methodology and findings

## Metrics Used
- **Points per $1M AAV** → offensive efficiency
- **xGF% per $1M AAV** → play-driving efficiency
- **TOI/GP, GP** → minimum usage thresholds
- **R² = 0.53** → proven correlation between xGF% and Win%

## Tools
- Python (Pandas, Matplotlib)
- Google Colab
- GitHub for versioning

## Findings
- xGF% correlates strongly with team win% (R=0.728)
- Several players outperform their salary based on both production and play-driving
- Ideal trade/FA targets are often middle-six forwards under $4M

## Correlation of xGF% and Win%
![xGF% vs Win% Correlation](visuals/xgf_vs_win_correlation.png)

## Best Value Forwards based on points/per million dollars
![Best Value Forwards: Points Efficiency](visuals/points_per_million_plot.png)

## Best Value Forwards for xgf per million
![Best Value Forwards: Play Driving Efficiency](visuals/xgf_per_million_plot.png)

## Top 15 Underpaid Forwards (Combined Value Score)
![Value Score Bar Plot](visuals/value_score_bar_plot.png)


📂 Top 15 Based on Value Metric Data: [`data/top_15_value_targets.csv`](data/top_15_value_targets.csv)

This plot is based on players filtered by cap hit (≤ $4M), TOI/GP (≥ 8), and GP (≥ 30).  
📄 Source data: [`data/final_value_targets.csv`](data/final_value_targets.csv)

## Future Work
- Add clustering by player archetype
- Visualize team-level value capture
- Introduce contract length, age curves, or playoff performance




## Data Sources
- Thank you to Natural Stat Trick for the in game analytic stats
- Thank you to PuckPedia for the Salary Stats


🧠 Full analysis notebook: [`notebooks/nhl_value_forwards.ipynb`](notebooks/nhl_value_forwards.ipynb)
