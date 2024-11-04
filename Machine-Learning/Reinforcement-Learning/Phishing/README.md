# Phishing Detection with Reinforcement Learning

This project applies reinforcement learning to detect phishing websites, using a simplified Q-learning approach. The program simulates a basic environment where a Q-learning agent learns to classify URLs as "phishing" or "not phishing" based on rewards and penalties. The model’s performance is tracked and visualized over time.

## Table of Contents
- [Project Overview](#project-overview)
- [Environment Setup](#environment-setup)
- [Agent](#agent)
- [Running the Project](#running-the-project)

## Project Overview
In this simulation:
1. The agent interacts with a custom `PhishingEnv` environment.
2. The agent learns to classify phishing URLs through trial and error, using Q-learning.
3. Performance is tracked across episodes to monitor correct classifications and Q-value convergence.

## Environment Setup
The environment includes:
- **State Space**: Placeholder states, representing phishing and not phishing URLs.
- **Action Space**: Actions to classify URLs as "phishing" or "not phishing."
- **Rewards**: Correct classifications receive positive rewards, while incorrect classifications receive penalties.

## Agent
The Q-learning agent uses an epsilon-greedy policy to balance exploration and exploitation, with Q-values updated at each step. Q-value convergence is tracked to monitor learning progress.

## Running the Project
1. Ensure you have all dependencies installed (refer requirements.txt).
2. Run the script to start training the agent:
   ```bash
   python phishing_rl.py

