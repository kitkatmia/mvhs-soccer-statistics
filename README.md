# MVHS Soccer Statistics

## Project Overview

This project aims to analyze soccer game data to provide insights into the MVHS team's performance, with a specific focus on possession statistics. The goal is to identify areas where the team can improve and provide valuable information to the coaches for strategic decision-making.

## File Structure

The project is organized as follows:

MVHS_Soccer_Statistics/

├── data/

│ └── \*.csv (game data files, e.g., possession_data.csv, goal_scorers.csv)

├── snapshot_1/

│ └── analysis_1.py (data analysis for first 4 games)

└── snapshot_2/

└── analysis_2.py (data analysis for next 4 games)

## Data Analysis Approach

1. Data Collection:

#### See Data Explanation section for a more detailed overview.

- Team data is collected into CSV files in the data folder. It is based on data given by video analysis done by HUDL
- Specific data (ex: 8_games_goal_info.csv) is based on data I've gathered watching the videos

2. Snapshot Analysis:

Data is analyzed in chunks of 4 games within Python files in the snapshot_1, snapshot_2, etc folders.
Each snapshot focuses on identifying patterns and trends in play - specifically those that are harmful to the team (as judged by being correlated with being scored on more).

- The focus is especially on passing and possession

3. Python Libraries:
   pandas is used for data manipulation and cleaning.
   matplotlib is used for creating visualizations to aid in interpretation.

## Insights and Recommendations

{TBC}

## Future Work

{TBC}
