# American Options Pricing with Q-learning

## Overview

This project implements Fitted Q Iteration, a Q-learning-based approach, to price American options. American options are financial derivatives that give the holder the right, but not the obligation, to buy or sell an underlying asset at a specified price before or at the expiration date (T).

This approach aims to learn an optimal pricing policy Q* for American options. In other words, we want to learn the optimal action (exercise or hold) to take at each state (financial market condition) to maximize the expected cumulative reward over time. We estimate the continuation value using Laguerre Basis functions and compare it to the return of exercising the option.

## Features

- **Monte Carlo Framework:** The project uses Monte Carlo simulation to generate thousands of paths of stock prices, which are used to train the model.

- **Q-learning Algorithm:** At the core of the project is the Q-learning algorithm, which trains a model to make optimal decisions for exercising or holding American options.
  
- **American Options Pricing:** The Q-learning model is applied to the specific problem of pricing American options. It learns from historical financial data and market conditions to determine the optimal pricing strategy.

- **Agent:** The entity that interacts with the environment, learning to exercise or hold the option to maximize the reward.

- **Data:** Two years of Apple stock data were utilized. Further details about the data, including format and preprocessing, can be found in the project documentation.


## Results

This algorithm provides very promising results, descovering good opportunities to excercise or hold the option for the right reasons, here we get

![Alt Text](results.png)
