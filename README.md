# NBA-Statistical-Analysis-and-Player-Valuation-2019

The purpose of this project is to analyze different NBA statistics to better understand players' values. I downloaded my data from Basketball Reference and Kaggle at the links below. I filtered my data for 2010 to 2019, eliminated duplicates within each year that came from trades and salary changes, and merged my 2019 data with the current salaries of the NBA players. Additionally, I filtered for different positions, minutes, and salaries to look more closely at the numbers and better compare players.

Throughout the project, I adjusted my dataframes to only include players who played an average of at least 2 minutes per 84 game season. This is because I continuously saw that different players who played minimal minutes had extremely high usage rates and efficiency ratings if they happened to, for example, score a three pointer in 1 minute  played. I believe that this adjustment increases the reliability of my results by eliminating those skewed numbers. In analyzing player performances, I took into account the minutes played and salaries earned by each player to find those who may be undervalued or deserve more minutes. I discovered players who were most efficient with the minutes they were allocated, as well as those who gave the best return on their yearly salary. This information would help GMs and coaches make informed decisions on player personnel and usage.

In order to conduct my valuation, I first examined how different key statistics correlate with win shares. I used this stat because I believe that a player's value should be determined by how he influences his team and delivers them wins. However, strong talent within a team may disperse the win shares among the talented players, driving down each individual's statistic. Therefore, I used the correlation coefficients of key statistics over a 10 year period to determine the values of players, using the numbers to weigh the importance of each stat since win shares alone can be biased. While this is not a perfect fix for the potential dilemma, since other statistics are affected by strength of teammates, it helps diminish the flaw.

Finally, I created a valuation model by using the correlation coefficients and applying them to each player's stats. I multiplied each statistic by its coefficient, added them together, and divided the result by the number of stats used in order to average the win shares estimated for each player. This method proved to be effective, as the model showed 74% accuracy in predicting NBA all-stars over 5 years and identified potentially undervalued players. After discovering each player's value, I weighed the value of players in the top 50% of the league against their yearly salary. This analysis allowed me to discover players whose salaries are most valuable given their return. I also weighed the values against the minutes played to see which players perhaps deserve more time on the court. I repeated these methods, looking into the top performers at each position. I believe my findings would be useful to an NBA GM in deciding which players to target and carrying out different transactions.

While I believe this is a thorough analysis, I am always searching for new perspectives and ideas on how to improve my valuation. If you have any questions, comments, or concerns regarding my analysis, you may reach out to me via email at jeh606@stern.nyu.edu or phone at 610-509-1189. I am excited by any opportunity to enhance this model, so please do not hesitate to contact me if you find anything you believe I can improve.


Author: *James Haag*

Sources:
    
    https://www.basketball-reference.com/leagues/NBA_2019_advanced.html
    https://www.basketball-reference.com/leagues/NBA_2019_totals.html
    https://www.basketball-reference.com/contracts/players.html
    https://www.kaggle.com/drgilermo/nba-players-stats#Seasons_Stats.csv
