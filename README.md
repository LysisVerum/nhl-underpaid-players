# NHL Underpaid Players: Value vs Salary Analysis

## Objective
Use publicly available salary and performance data to identify NHL players who are significantly underpaid relative to their on-ice contributions.

## Key Questions
- Which players deliver the highest value per $1M of salary?
- How can teams identify undervalued contributors using data?
- What player archetypes tend to be underpaid?

## Project Structure
- `data/`: salary, performance (WAR, xGoals), merged dataset
- `notebooks/`: cleaning, analysis, modeling
- `visuals/`: plots and final insights

## Metrics Used
- WAR (Wins Above Replacement)
- xGoals, RAPM, Points
- Salary Cap Hit (AAV)
- Efficiency metrics: WAR/$1M, Points/$1M, Residuals from salary regression

## Tools
- Python (Pandas, Seaborn, Scikit-Learn)
- Jupyter/Colab
- Tableau (optional)
- GitHub for version control

## Future Plans
- Add clustering to detect undervalued player types
- Expand to include contract length or age curves
