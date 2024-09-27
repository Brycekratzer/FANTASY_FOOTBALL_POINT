# Fantasy Football Data Analysis Project

## Overview

This project analyzes fantasy football data from 2020 to 2023, focusing on player performance trends and correlations between early-season and full-season averages for different positions (WR, QB, RB).

## Data Sources

The project uses CSV files containing fantasy football points data (PPR format) from FantasyPros for the years 2020, 2021, 2022, and 2023.

## Dependencies

- pandas
- numpy
- matplotlib
- seaborn

## Data Preparation

1. Import CSV files for each year (2020-2023).
2. Remove unnecessary columns ('Player', 'Team', '#').
3. Concatenate data from multiple years for analysis.
4. Clean data for each position (RB, QB, WR):
   - Filter players with average points for full season >= 5.
   - Replace '-' and 'BYE' values with 0.
   - Convert data to float type.
   - Remove players with more than 5 zero-point games.

## Analysis

The project performs the following analyses for each position (WR, QB, RB):

1. Calculate 3-week averages for the beginning of the season.
2. Compare 3-week averages to full-season (18-game) averages.
3. Create scatter plots with regression lines to visualize the relationship.
4. Calculate correlation coefficients (R-values) between 3-week and season averages.

## Visualizations

The project generates scatter plots for each position, showing:
- X-axis: 3-week average fantasy points
- Y-axis: 18-game (full season) average fantasy points
- Regression line
- R-value in the plot title

## Key Findings

The R-values for each position indicate the strength of the correlation between early-season (3-week) performance and full-season performance:

- WR: [R-value .74]
- QB: [R-value .72]
- RB: [R-value .61]

These values can help in understanding how predictive early-season performance is for different positions in fantasy football.

## Additional Notes

- The project includes specific analysis for low-scoring WRs (6-8 points average).
- Performance differences between 3-week and season averages are calculated for QBs and RBs.

## Future Improvements

1. Extend the analysis to include more years of data.
2. Add analysis for other positions (TE, K, DEF).
3. Implement machine learning models for performance prediction.
4. Create interactive visualizations for easier data exploration.

## Running the Project

1. Ensure all dependencies are installed.
2. Place the CSV files in the same directory as the script.
3. Run the script to generate analyses and visualizations.

## Conclusion

This project provides insights into the relationship between early-season and full-season performance in fantasy football, which can be valuable for fantasy team management and player evaluation strategies.