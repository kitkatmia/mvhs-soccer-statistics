# MVHS Soccer Statistics

## Project Overview

This project aims to analyze soccer game data to provide insights into the MVHS team's performance, with a specific focus on possession statistics. The goal is to identify areas where the team can improve and provide valuable information to the coaches for strategic decision-making.

## Insights and Recommendations
Linked below are all of the analyses sent to the soccer coaches, copy and pasted from the emails sent to them (with minor edits for clarity / removal of personal details). The purpose and main subject of the analyses differ **because of the team's changing needs and coaches asks**
<br/>
Note: They are sorted from most recent - oldest order
<br/>
- [Los Altos Games Comparison](./insight_pdfs/los_altos_game_comparison.pdf)
- [Palo Alto Game](./insight_pdfs/palo_alto_game.pdf)
- [Los Altos Game 1](./insight_pdfs/los_altos_game.pdf)
- [Snapshot 2](./insight_pdfs/snapshot_2.pdf)
- [Snapshot 1](./insight_pdfs/snapshot_1.pdf)
  
## File Structure

The project is organized as follows:

MVHS_Soccer_Statistics/

├── data/

│ └── \*.csv (game data files, e.g., possession_data.csv, goal_scorers.csv)

├── insight_pdfs/

│ └── los_altos_game.pdf (pdf of insights emailed to coach with minor edits for privacy / clarity)
│ └── ...and so on

├── snapshot_1/

│ └── snapshot_1.ipynb (data analysis for first 4 games)

...and so on

## Data Analysis Approach

### 1. Data Collection:

- #### See Data Explanation section for a more detailed overview.
- Team data is collected into CSV files in the data folder. It is based on data given by video analysis done by HUDL
- Specific data (ex: 8_games_goal_info.csv) is based on data I've gathered watching the videos

### 2. Snapshot / Game Analysis:

Data is analyzed in chunks of 4 games within Python files in the snapshot_1, snapshot_2, etc folders.
Each snapshot focuses on identifying patterns and trends in play - specifically those that are harmful to the team (as judged by being correlated with being scored on more).

- The focus is especially on passing and possession
  
<br/>

NOTE: In recent weeks, the focus has shifted towards analyzing specific games and comparing them to our averages. As such, data is now analyzed on a game-by-game basis
- The focus depends on coaches asks (although passing and possession are always relevant statistics)
- Since data is analyzed in comparison to averages, their are extra datasets in the data folder that exist simply to compare game to past games

### 3. Python Libraries:

Pandas is used for data manipulation and cleaning.
<br/>
Matplotlib is used for creating visualizations to aid in interpretation.


## 4. Future Work

- Optimize data pipeline
- Compile all data; look for greatest predictive values of wins / goals as well as greatest predictive values for getting scored on
- Streamline most commonly used functions

  
## Data Explanation
- time_frame: what period of time the tracked event / statistic occured in (ex: 0-15 means it happened in the first 15 minutes of the game)
- goals_for_avg: average goals MVHS scored (NOTE: if this is just for a single game, this may be represented by just 'goals')
- goals_against_avg: averages goals opponents scored on MVHS
- shots_on_target_%: what percentage of the shots taken were on frame
- shots: how many shots were taken
- crosses: how many crosses were taken
- poss_%: percentage of time that MVHS had possession of the ball in a selected time frame
- pass_success_rate: percentage of successful passes
- num_pass_strings: number of pass strings, as defined by a series of 3+ passes
- avg_pass_string: average length of a pass string in a time frame
- 3_to_5_PS: number of pass strings that consisted of 3 to 5 passes
- 6_plus_PS: number of pass strings that consisted of 6+ passes
- atk_third_pass_success_%: what percentage of passes in the attacking third of the field were successful
- pass_attempts_atk: how many passes were attempted in the attacking third
- mid_third_pass_success_%: what percentage of passes in the middle third of the field were successful
- pass_attempts_mid: how many passes were attempted in the middle third
- def_third_pass_success_%: what percentage of passes in the defensive third of the field were successful
- pass_attempts_def: how many passes were attempted in the defensive third
