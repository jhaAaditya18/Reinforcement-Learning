Q-Learning in a GridWorld

Overview
This project demonstrates Q-learning, a reinforcement learning (RL) algorithm, in a 4x4 grid environment.
The agent starts at (0, 0) and aims to reach the goal at (3, 3).
The agent receives a +10 reward for reaching the goal and a -1 penalty for every move.

Key Concepts of Q-Learning
Actions: The agent can move Up (U), Down (D), Left (L), or Right (R).
Reward Function: The agent receives a +10 reward for reaching the goal and -1 for every move.
Q-Table: A table that stores the expected value for each state-action pair.
Exploration vs. Exploitation: The agent explores new actions (randomly) with probability ε and exploits the best-known actions with probability 1-ε.


Hyperparameters
Learning Rate (α): 0.1
Discount Factor (γ): 0.9
Exploration Rate (ε): 0.2
Episodes: 500 training episodes

Reinforcement Learning Overview
Reinforcement learning is a type of machine learning where an agent learns to make decisions by interacting with its environment.
The goal is to maximize the cumulative reward over time.
Q-learning is an off-policy RL algorithm that updates the Q-values for state-action pairs using the following formula:
Q(s,a)←Q(s,a)+α[R+γmaxQ(s',a)-Q(s,a)]
