🐍 ## Snake Game 
This repository contains a Python implementation of the classic Snake Game, where the snake is trained using Reinforcement Learning with the Deep Q-Learning algorithm. The project showcases how artificial intelligence can learn to navigate and optimize its gameplay using neural networks and a reward-based learning framework.

🎯 ## Project Description
The goal of this project is to train an AI agent to play the Snake game efficiently by:

Maximizing the score by eating food.
Avoiding collisions with walls or its own body.
The AI agent uses Deep Q-Learning, a model-free Reinforcement Learning algorithm, to make decisions. Through training, the agent learns from its past actions using a neural network that approximates the optimal Q-values for the game state-action pairs.

This project demonstrates:

The application of reinforcement learning to a real-world sequential decision-making problem.
The importance of reward engineering in reinforcement learning.
How Deep Q-Learning works in a grid-based environment like Snake.
⚙️ Features
Custom Snake Game Environment: Built using Python and Pygame, the game provides a simple yet robust environment for training the RL agent.
Deep Q-Learning Implementation: Includes a neural network to approximate Q-values, a replay memory buffer, and an epsilon-greedy policy for exploration.
Training and Evaluation: The agent is trained over multiple episodes, and its performance is evaluated in terms of game score and survivability.
Video Demo: See the trained AI in action below.
🧠 ## Algorithm
Deep Q-Learning
Deep Q-Learning (DQL) is a reinforcement learning algorithm that combines Q-Learning with deep neural networks. The agent learns to predict the Q-value of state-action pairs using experience replay and target networks.

Workflow:
State Representation:

The state includes information about the snake's position, the location of the food, and the relative positions of obstacles (walls and the snake's own body).
Reward Function:

Positive reward: Eating food.
Negative reward: Colliding with a wall or itself.
Small negative reward: Each step taken without eating food to encourage efficient gameplay.
Neural Network Architecture:

Input: Current state representation (e.g., snake's position, food location).
Hidden Layers: Fully connected layers with ReLU activation.
Output: Q-values for all possible actions (e.g., move up, down, left, right).
Replay Memory:

Stores past experiences (state, action, reward, next_state, done) to train the neural network with randomly sampled batches.
Target Network:

A separate neural network periodically updated to stabilize training.
Training Loop:
📹 Demo


