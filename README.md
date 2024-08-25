# Reinforcement Learning Algorithms for Taxi-v3 Environment

## Project Overview

This project implements and compares three reinforcement learning algorithms (Q-Learning, SARSA, and Deep Q-Network) on the OpenAI Gym Taxi-v3 environment. The goal is to train an agent to efficiently pick up and drop off passengers in a 5x5 grid world.

## Algorithms Implemented

1. SARSA (State-Action-Reward-State-Action)
2. Q-Learning
3. Deep Q-Network (DQN)

## Key Features

- Implementation of both on-policy (SARSA) and off-policy (Q-Learning, DQN) algorithms
- Comparison of tabular methods (SARSA, Q-Learning) vs neural network approach (DQN)
- Exploration of various hyperparameters including learning rate, discount factor, and epsilon values
- Performance evaluation using average rewards over episodes

## Results

| Algorithm | Best Average Reward (Training) | Best Average Reward (Testing) |
|-----------|--------------------------------|-------------------------------|
| Q-Learning (Variable ε) | 8.85 | 7.38 |
| Q-Learning (Constant ε) | 8.72 | 7.91 |
| SARSA (Variable ε) | 8.47 | 7.9 |
| SARSA (Constant ε) | 8.28 | 8.61 |
| DQN | 7.5 | 7.69 |



### Conclusion
The algorithms demonstrated similar performance, with Q-Learning (variable epsilon) slightly outperforming the others in terms of convergence speed and average rewards. Deep Q-Network did not yield significant improvements over simpler methods like Q-Learning and SARSA, especially in the Taxi-v3 environment. Simpler approaches may be more efficient for such grid-world problems.

## License

[MIT](https://choosealicense.com/licenses/mit/)

## Acknowledgements

- OpenAI Gym for the Taxi-v3 environment
- PyTorch and TensorFlow documentation for DQN implementation guidance
- **Sutton, R. S., & Barto, A. G. (2018).** *Reinforcement Learning: An Introduction* (2nd ed.). The MIT Press.

