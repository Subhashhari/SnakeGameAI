#  Applying the concepts of Deep Q-learning to train a system agent to play the Snake game.

## Goal:
The aim was to successfully use the concepts of Deep Q-learning and train a system agent to play a custom version of the classic Snake Game.

## Tech Stack:
* Python
    * Pytorch
    * Pygame
    * Matplotlib
    * Ipython 
    * Random
    * Numpy
    * Collections
    * enum

## How to Run:
* Make sure all the files in the repository are downloaded into the same folder.
* Make sure all the necessary modules are already installed onto the system.
* Run the "agent.py" file as it controls the game and it imports the necessary other files and functions.
* Two windows will pop up, one showing the game and other a graph of current score and also a rolling average.
* Let the model learn for a while, upto about 150 games and be amazed by the results.

## Explanation
* Created an agent to interact with a custom built Snake game environment using the Pygame library.
* The agent observes the game state by encoding information like snake position, food location, and danger zones into a numerical vector, it also controls the choice of the next action
* The core of the agent is a Q-Network implemented with PyTorch. This network predicts the future reward for each possible action based on the current state. The agent learns by exploring different actions, receiving rewards (or penalties), and updating the Q-Network based on those experiences.
* To improve learning efficiency, the agent utilizes experience replay. It stores past experiences (state, action, reward, next state) in a memory buffer and randomly samples from it for training the Q-Network.
* The code employs a helper function to plot the training scores and their rolling average over time. This visualization provides a clear representation of the agent’s learning trajectory.

## Applications:
This project built an ML model that plays the Snake game, but it's more than just a game. The real strength is its flexibility. By changing the game's settings, how the model gets rewarded, and the complexity of the neural network, this system could be used for other games too. I started with the Snake game to build a strong foundation. In the future, this system could be used to solve puzzles, master different game types, or even learn to compete against itself. This project opens the door to exciting possibilities in machine learning and game AI.

## Further Improvements:
* Could have had a better UI for the game or even chosen a more complicated game.
* Could have added other elements like bonus points or score multipliers etc. to make the game more fun.
* Could have implemented the model such that it was more accurate by either adding more layers to the neural network or even optimising the reward function, could have also exploited the tradeoff between exploration and exploitation to try more random things at the start. 

## Conclusion
* This project successfully implemented a machine learning model capable of playing the Snake game. The model demonstrates the ability to learn and improve its performance over time, as evidenced by the increasing scores depicted in the progress graph. While the current implementation focuses on the core elements of the game, it lays a strong foundation for further development. Future iterations could explore incorporating more complex strategies, introducing obstacles, or even evolving the model to compete against itself or other AI players. Overall, this project serves as a valuable exploration of machine learning in a simple yet engaging environment.

## Demo Video:
* https://youtu.be/b_aoi2JPUTY
