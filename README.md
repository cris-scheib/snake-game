## Snake Game 🐍🍏 - Reinforcement Learning

### Purpose
Using AI to learn how to play the Snake Game with Reinforcement Learning
The idea behind the project was to learn reinforcement learning methods, so this project was made from scratch

### The Game
The rules of the game are that the snake cannot hit itself, nor the walls and must catch as many apples as possible.

### Environment
The Environment was designed in a 5x5 size, the snake starts, the snake always starts in the same position at the beginning of the game and the apple is projected in a random position with each new game.
Each position of each element in the environment has a state, which is controlled by a Hash table, there are four possible states for each point on the board, being Snake's Head, Snake's Body, Empty or the Apple. The head and body are different as the states change according to the snake's direction.
The reward was initially set at 100 points for when it gets the apple, -200 for when it loses the game, 10 for each step toward and -5 further the apple.
There is a 0.9 reward discount factor, a learning rate of 0.99 and a probability of exploitation of 1 (100%) with 0.1 of decay;

### Agent
Using a Q list (as image below) it keeps track of action state, where it receives state, reward, where it checks the values between action state compared to previous actions states. It plays the game until it loses all the games by X episodes.
At the end it returns how many games it played and how many were its rewards.

![image](https://user-images.githubusercontent.com/61483993/181864165-9c02890f-d04a-4651-adac-0b9f39abec18.png)
