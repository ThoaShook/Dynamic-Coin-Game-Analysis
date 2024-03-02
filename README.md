#### Dynamic-Coin-Game-Analysis

  * This Jupyter-notebook contains Python code for simulating a two-palyer game and analyzing the outcomes using the Monte Carlo method. The game involves two players, A and B, and is played with a six-sided die.
  * **Game Rules**
      * At the beginning of the game, each player starts with 4 coins, and there are 2 coins in the pot.Players take turns in a cycle (A,B, A,B,...). During their turn, players roll the die to perform certain actions:
     * On a roll of 1: Do nothing
     *  On a roll of 2: Take all coins in the pot
     *  On a roll of 3: Take half coins in the pot (round down)
     *  On a roll of 4,5, or 6: Put a coin in the pot
  * A player loses the game if they have 0 coins and need to place another coin in the pot. The last completed cycle is still counted even if a player goes out during the game.

* **Files**
    1. 'play_coin_game.ipynb': Contains the Python code for simulating the game and generating the 'cycle_counts' data for analysis
    2. 'analyze_outcomes.ipynb': Contains functions for analyzing the outcomes of the game, including calculating the expected value, standard deviation, and cofidence intervals for the number of cycles.
    3. 'hypothesis_testing.ipynb': Contains functions that test for normality of the outcomes
* **Usage**
    * Run 'play_coin_game.ipynb' to simulate the game and generate the 'cycle_counts' data. Adjust the 'num_games' variable to control the number of game simulations
    * Run 'analyze_outcomes.ipynb 'to analyze the generated 'cycle_counts' data. The functions in this file provide various statistical measures for the outcomes.
    * Run 'hypothesis_testing.ipynb' to test for normality of the outcomes and to estimate the sampling distribution and confidence intervals of the statistic of interest(e.g.,mean)
* **How to run**
    * Make sure your have Python (version 3.x) and Anaconda installed
    * Navigate to the folder containing the download files
    * Run 'play_coin_game.ipynb' to perform the game simulation and generate the 'cycle_counts' data.
    * Run 'analyze_outcomes.ipynb' to calculate the expected value, standard deviation, and confidence intervals based on the 'cycle_counts' data.
    * Run 'hypothesis_testing.ipynb' to test for normality
* **Dependencies**
    * numpy==1.26.0
    * scipy==1.11.4
    * matplotlib==3.7.2
    * seaborn==0.13.0
* Ensure you have these libraries installed before runing the code
* **Notes**
    * Adjust the 'num_games' variable in 'play_coin_game.ipynb' for different number of game simulatiion. A larger "num_games' values yields more accurate estimates but may increase computation time.
    * The game simulation is based on the rules specified in the problem statement. You may modify the game rules in the 'play_coin_game.ipynb' file as needed.
    * The statistical analysis assumes certain properties of the data and may require additional assumptions based on the specific context.
