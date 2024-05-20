# 2048-PPO
As a lover of the game 2048, I decided to test whether the PPO algorithm could solve play the game as good as I play

# Rules
The rules of the game a simple, every move you do will collapse the number onto each other, if they are equal they will be summed, if they are not, they will just move positions, with every move a random 2 or 4 will appear on the tile. The goal of the game: Reach 2048.

<img width="502" alt="Screenshot 2024-05-20 at 15 27 11" src="https://github.com/lucca11235/2048-PPO/assets/91396656/a10ea7d9-6b25-44d0-b560-1e42c57a92c4">

# Results
I have succesfully implemented the game in python in an environment. Using stable_baseline3 library, I implemented the PPO algorithm where I got an upward trend of rewards across episodes. However, the rewards are still very unstable, which causes the actual algorithm to not perform very well on the game and further improvements are needed.


<img width="538" alt="Screenshot 2024-05-20 at 15 29 57" src="https://github.com/lucca11235/2048-PPO/assets/91396656/b8f09de9-3d52-49d2-92d3-297890068aae">
