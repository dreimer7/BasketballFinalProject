# 🏀 Predicting Star-Level Contracts in the NBA
This project analyzes how well an NBA player’s first two seasons predict their long-term financial value. Using statistical modeling and scraped salary data, the project examines which early-career performance metrics are most associated with reaching a “star-level” contract.

## 🔢 Table of Contents
1. Research Question
2. Data Sources
3. How to Run
4. Definitions
5. Key Finding
6. Contact

## ❓ Research Question
Which early-career performance factors lead to a star-level contract during a player’s career?

## 📊 Data Sources
- Player statistics sourced from Basketball-Reference  
- Salary data scraped from team-season pages (1991–2024)  
- Player statistics scraped using Gabriel Pastorello's [BRScraper](https://github.com/GabrielPastorello/BRScraper)

## ▶️ How to Run

This project is designed to run in **Google Colab**, and all required packages are installed within the notebook.
1. Open the notebook in Google Colab:
   - Upload the `.ipynb` file or open it directly from GitHub
2. Run all cells in order:
   - Runtime → Run All
3. Data will be loaded directly from GitHub, so no manual uploads are required

**🔗 Open in Colab**
- You can run the project directly using this link: [Open in Colab](https://colab.research.google.com/drive/1SPJzIR_zsC8CPpQZCf0zYlt4P2GVpMlN#scrollTo=NwG7U_0d5i47)

**⚠️ Notes**
- No local setup is required  
- A pre-collected dataset is included for faster execution  

## 📖 Definitions:
- **"Star-level" contract**: A contract that is greater than 20% of the salary cap for the given year
- **Player**: Player's name
- **Pick**: The draft pick # the player was selected with
- **DraftYear**: The year the player was drafted
- **PeakSalary**: the player's highest single-season salary during their career
- **PeakSalaryPercent**: the percentage of the salary cap that the player's peak salary occupied
- **StarContract**: A binary variable with 1 = star contract and 0 = not a star contract
- **max_salary_year**: the year the player achieved their highest single-season salary
- **MP_pg**: Minutes played per game on average
- **PTS**: Points per game
- **TRB**: Total Rebounds per game / TRB% = The percentage of available rebounds the player grabbed while they were on the court
- **AST**: Assists per game / AST% = The percentage of team field goals that the player assisted on while they were on the court
- **STL**: Steals per game / STL% = The percentage of opponent possessions that ended in a steal by the player while they were on the court
- **BLK**: Blocks per game / BLK% = The percentage of opponent two-point field goal attempts blocked by the player while they were on the court
- **TOV**: Turnovers per game
- **PER**: A measure of per-minute production standardized such that the league average is 15
- **BPM**: A box score estimate of the points per 100 possessions a player contributed above a league-average player, translated to an average team
- **VORP**: A box score estimate of the points per 100 TEAM possessions that a player contributed above a replacement-level (-2.0) player, translated to an average team and prorated to an 82-game season
- **WS**: An estimate of the number of wins contributed by a player.
- **WS/48**: An estimate of the number of wins contributed by a player per 48 minutes (league average is approximately .100)
- **FG%**: Field Goal Percentage
- **3P%**: 3-Point Field Goal Percentage
- **FT%**: Free Throw Percentage
- **eFG%**: This statistic adjusts for the fact that a 3-point field goal is worth one more point than a 2-point field goal
- **TS%**: A measure of shooting efficiency that takes into account 2-point field goals, 3-point field goals, and free throws
- **USG%**: An estimate of the percentage of team plays used by a player while they were on the floor.
- **"_Y1"**: Variables ending in "_Y1" correspond to the player's first year in the NBA (ex: PTS_Y1)
- **"_Y2"**: Variables ending in "_Y2" correspond to the player's second year in the NBA (ex: VORP_Y2)
- **"_jump_1_2"**: Variables ending in "_jump_1_2" are the difference between the player's first and second year (ex: USG%_jump_1_2 = USG%_Y2 - USG%_Y1)

## 🔎 Key Finding
Second-year performance and overall production (e.g., points, minutes, impact metrics) are stronger predictors of future salary than efficiency or short-term improvement.

## 📞 Contact
- 📧 Email: milowessel@icloud.com
- 🌐 LinkedIn: https://www.linkedin.com/in/milo-wessel
