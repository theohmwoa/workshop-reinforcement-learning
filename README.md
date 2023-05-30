---
module:	B-INN-000
title:	Reinforcement Learning and Custom Gridworld Gym Environment
subtitle:	Develop a Q-Learning agent and create a custom Gym environment for a Gridworld game
binary: 	rl_custom_gym.py
repository: 	NA
language:	python
compilation:	NA
build:		no need here
version:	1
---

# Reinforcement Learning and Custom Gridworld Gym Environment

## Tâche 0 : Installation des bibliothèques nécessaires

Install the necessary libraries - Gym, Numpy, and Matplotlib.

```bash
python3 -m pip install gym numpy matplotlib
```

# Tâche 1 : Understand the Basics forcement Learning

Understand the key concepts of Reinforcement Learning (RL) - agent, environment, action, state, and reward. Use the Gym library to explore an existing environment such as "CartPole-v0".

## Tâche 2 : Create a Custom Gym Environment for a Gridworld Game

Design a simple 2D Gridworld game where an agent can move up, down, left, or right, with some cells acting as obstacles. The game ends when the agent reaches a goal cell. Each movement action gets a small negative reward, reaching the goal gets a large positive reward, and hitting an obstacle gets a large negative reward.

Create a new class for your environment, Gridworld, that inherits from gym.Env. Define the following methods:

- __init__: To initialize the state space, action space, and the grid.
- step: To perform an action and return the new state, reward, done (whether the episode is finished), and additional information.
- reset: To reset the environment to the initial state.
- render: To provide a textual or graphical representation of the environment.

## Tâche 3 : Test the Custom Gridworld Environment

Test the Gridworld environment by creating a random agent that moves randomly. Verify that the environment's reactions (state transitions, rewards, etc.) are as expected.

## Tâche 4 : Understand Q-Learning

Cf. Présentation.

## Tâche 5 : Implement a Q-Learning Agent

Create a class for a Q-Learning agent. The agent should maintain a Q-table and choose actions based on it using an epsilon-greedy strategy. It should also be able to update the Q-table based on observed rewards and new states.

## Tâche 6 : Train the Q-Learning Agent on the Gridworld Environment

Implement a training loop where the agent repeatedly interacts with the environment and updates its Q-function. After each episode, evaluate the agent's performance and visualize its improvement over time.

> **Hint:** To evaluate the agent's performance, you can let it interact with the environment without updating its Q-function and calculate the total reward it collects.

## Tâche 7 : Evaluate the Q-Learning Agent's Performance

Evaluate the agent's performance by calculating the average reward over several episodes after the Q-Learning agent has been trained. Compare the performance of the Q-Learning agent with that of the random agent.

## Pour aller plus loin

### Bonus 1 : Vary Parameters

Experiment with different parameter settings for the Q-Learning agent, such as the learning rate, discount factor, and epsilon decay rate, and evaluate.


