# gto

## Project Overview

This repository contains an implementation of Counterfactual Regret Minimization (CFR) for Kuhn Poker. CFR is an iterative algorithm used to approximate Nash equilibria in extensive-form games, such as poker.

## How It Works

The CFR algorithm works by simulating a large number of iterations of the game, during which it updates the regrets for each possible action at each decision point. The regrets represent the difference between the actual payoff and the payoff that would have been received if a different action had been taken. By averaging the strategies over many iterations, the algorithm converges to a Nash equilibrium, where no player can improve their expected payoff by unilaterally changing their strategy.

### Key Concepts

- **Regret Minimization**: The algorithm updates regrets for each action based on the difference between the actual payoff and the payoff that would have been received if a different action had been taken.
- **Strategy Convergence**: By averaging the strategies over many iterations, the algorithm converges to a Nash equilibrium.
- **Information Sets**: The algorithm uses information sets to represent the knowledge available to each player at each decision point.

## Usage Instructions

To run the CFR algorithm for Kuhn Poker, follow these steps:

1. Ensure you have Python installed on your system.
2. Install the required dependencies by running `pip install -r requirements.txt`.
3. Run the `kuhn.py` script using the command `python kuhn.py`.

The script will output the expected values for each player and the strategies they should use to achieve a Nash equilibrium.

### Interpreting Results

- **Expected Values**: The script will display the expected values for each player, representing their average payoff over many iterations.
- **Strategies**: The script will display the strategies for each player, showing the probability of taking each action at each decision point.

By following these instructions, you can run the CFR algorithm and analyze the results to understand the optimal strategies for Kuhn Poker.
