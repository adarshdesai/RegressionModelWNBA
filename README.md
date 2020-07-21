# RegressionModelWNBA

## Dataset:
The Dataset contains advanced statistics of teams and players of WNBA history. The two descriptive csv files (wnba-player-stats.csv and wnba-team-elo-ratings.csv) contains advanced statistics for Women NBA players by team for the 1997-2019 seasons, from Basketball-Reference.com. Where one file represents the Teams’ performance statistics and the other focuses on individual players’ performance.

Composite Rating is determined by the following formula (based on NBA player stats):

Rating = -5.237248 + 0.1741241*PER + 26.0059929*WS40

Individual ratings are then adjusted so the team's weighted average Composite Rating (times 4.064, a scalar to account for score effects) equals the team's Net Rating. Wins Generated are derived by divvying up the team's Net Rating-implied wins according to each player's contribution to the team's Net Rating.

### The Regression Model predicts the ‘Wins_Generated’ attribute of the player. 
