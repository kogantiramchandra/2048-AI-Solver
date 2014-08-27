# 2048 AI - Using no hard-coded knowledge about the game.

Credit goes to ronzil/2048-AI for implementation of an AI solver that doesn't need a human's knowledge of the game. The AI solver has to find out for itself what the best possible move is at any point. This implementation does not use any heuristics such as smoothness or monotonicity. 

For each possible move, play it and then continue to play random moves until the game is finished. This is done many times and the move that returns the highest average score is chosen.

Each run of a particular move causes the updates the MCTS(Monte Carlo Tree Search) and thus helps in choosing a particular move over the author. Increasing the number of runs for each move causes a better aproximation towards the optimal move and hence is preferred. Keeping time constraints in mind, I am using 100 runs pper move.
