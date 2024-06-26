# 2048-PPO

As a fan of the game 2048, I decided to explore whether the PPO (Proximal Policy Optimization) algorithm could play the game as effectively as I do.

# Rules

The rules of 2048 are simple: each move collapses the tiles on the board. If two tiles with the same number collide, they merge into one with their sum. If they don’t match, they just shift positions. After every move, a new tile (either 2 or 4) appears randomly on the board. The objective of the game is to reach the 2048 tile.

<img width="502" alt="Screenshot 2024-05-20 at 15 27 11" src="https://github.com/lucca11235/2048-PPO/assets/91396656/a10ea7d9-6b25-44d0-b560-1e42c57a92c4">

# Results (as of now)
I have successfully implemented the game in Python and used the stable_baselines3 library to apply the PPO algorithm. The results show an upward trend in rewards across episodes, indicating some learning progress. However, the rewards are still quite unstable, which affects the algorithm’s performance. Further improvements are necessary to enhance the stability and efficiency of the gamepla, perhaps by increasing the size of the network or playing with hyperparameters using Optuna.

### Rewards across episodes
<img width="538" alt="Screenshot 2024-05-20 at 15 29 57" src="https://github.com/lucca11235/2048-PPO/assets/91396656/b8f09de9-3d52-49d2-92d3-297890068aae">

### Comparizon with random policy
Even though the model was not able to achieve an extremely good performance, it's clear that the model learned since the disbribution of best scores is slightly shifted to the right, meaning that on average the model is better then a random policy.

<img width="507" alt="Screenshot 2024-05-20 at 19 49 30" src="https://github.com/lucca11235/2048-PPO/assets/91396656/01636c32-7c5a-42c4-933e-3085cbb0e700">

