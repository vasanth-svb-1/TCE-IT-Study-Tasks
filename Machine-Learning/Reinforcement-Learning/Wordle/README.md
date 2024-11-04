# Wordle Game Reinforcement Learning

This project demonstrates a Q-learning agent trained to play a Wordle-inspired game. The agent aims to guess a five-letter target word within six attempts by receiving feedback on each guess. The feedback consists of positional hints, marked as:
- **G**: Correct letter in the correct position
- **Y**: Correct letter in the wrong position
- **X**: Incorrect letter

## Table of Contents
- [Project Overview](#project-overview)
- [Game Mechanics](#game-mechanics)
- [Agent Details](#agent-details)
- [Running the Project](#running-the-project)

## Project Overview
The program comprises:
1. **Game Environment** (`WordleGame`): Provides feedback on guesses.
2. **Q-Learning Agent** (`QLearningAgent`): Learns optimal guesses based on feedback.
3. **Visualization**: Tracks attempts per episode and Q-value heatmaps for state-action pairs.

## Game Mechanics
The `WordleGame` class simulates a simplified Wordle game:
- **State**: Feedback from the last guess.
- **Action**: Five-letter word guesses.
- **Reward**: Positive for correct guesses, negative for incorrect ones.
- **Feedback**: Letters are marked as G (correct), Y (misplaced), or X (incorrect).

## Agent Details
The Q-learning agent:
- Uses an epsilon-greedy policy for exploration vs. exploitation.
- Updates Q-values based on feedback and rewards, improving its strategy over episodes.

## Running the Project
1. Install dependencies through requirements.txt.
   ```bash
   pip install -r requirements.txt
2. Run the script to initiate training:
   ```bash
   python RL-Wordle.py
