# Mountain Car Control Using Deep Q-Network and Fuzzy Logic

## Videos


![Fuzzy-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/5e2edc59-5c7a-4224-b17a-353115d5bfa0)
![RL-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/6699c172-8acc-435c-8d8c-ec3466584491)





## Overview
This project explores the implementation of a **Deep Q-Network (DQN)** for solving the classic **Mountain Car problem** and subsequently designing a **Fuzzy Logic System (FLS)** based on the trained DQN model. The goal is to train an agent to control a car climbing a mountain efficiently by maximizing cumulative rewards.

## Authors
- **Mohammad Mehdi Moazedi**
- **Mohammad Reza Shirdoost**
- **Date**: February 2025

---

## Table of Contents
- [Introduction](#introduction)
- [Deep Q-Network (DQN)](#deep-q-network-dqn)
- [Fuzzy Logic System (FLS)](#fuzzy-logic-system-fls)
- [Implementation Details](#implementation-details)
- [Results & Analysis](#results--analysis)
- [Conclusion](#conclusion)

---

## Introduction
The **Mountain Car problem** is a well-known reinforcement learning challenge where a car with low power must learn to reach the goal by optimizing its movements through an uneven landscape. This project implements **DQN**, a deep reinforcement learning algorithm, and then translates its learned behavior into a **Fuzzy Logic System (FLS)** for alternative decision-making.

## Deep Q-Network (DQN)
### Key Concepts
- **Reinforcement Learning (RL)**: An agent interacts with an environment to maximize cumulative rewards.
- **Q-Learning**: A value-based RL algorithm that estimates action values (Q-values) for optimal decision-making.
- **Deep Q-Network (DQN)**: Combines deep learning with Q-learning to approximate Q-values using neural networks.

### Improvements in Training
- **Experience Replay**: Storing and replaying past experiences to stabilize learning.
- **Target Network**: A separate neural network to provide stable Q-value targets.
- **Reward Shaping**: Custom rewards to encourage effective exploration and learning.

## Fuzzy Logic System (FLS)
After successfully training the **DQN agent**, we used its data to design an **FLS** that mimics its learned behavior.

### Steps in FLS Design
1. **Data Extraction**: Collecting position, velocity, and action data from the trained RL model.
2. **Membership Functions**: Gaussian membership functions for state representation.
3. **Fuzzy Rules**: Defining rules based on RL agent behavior to control the car effectively.
4. **Inference & Defuzzification**: Computing actions based on fuzzy logic.

## Implementation Details
- **Programming Language**: Python
- **Libraries Used**:
  - TensorFlow / PyTorch (for DQN implementation)
  - OpenAI Gymnasium (for Mountain Car environment)
  - Skfuzzy (for fuzzy logic system)

## Results & Analysis
- **DQN Model** successfully learns an optimal strategy for solving the Mountain Car problem.
- **FLS-Based Controller** effectively mimics the trained RL agent's decision-making.
- **Performance Comparison**:
  - DQN achieves faster learning but requires extensive training.
  - FLS provides a rule-based, interpretable alternative with competitive results.

## Conclusion
This project demonstrates how a trained **DQN model** can be leveraged to design an **FLS-based controller** for solving the Mountain Car problem. The **hybrid approach** showcases the power of combining **reinforcement learning** with **fuzzy logic** for intelligent decision-making.

## Acknowledgments
- **Deep Q-Network (DQN)** was implemented based on OpenAI Gym and TensorFlow.
- **Fuzzy Logic System (FLS)** was designed using **skfuzzy** for rule-based decision-making.

---

Feel free to explore and contribute! 🚀

