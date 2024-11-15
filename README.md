# Otello
## Project Overview

This project is focused on implementing the α-β pruning algorithm for game tree resolution, specifically applied to the game of Otello (also known as Reversi). The objective is to understand and implement the algorithm, devise game heuristics, and compare their performance against each other.

## Game Rules

Otello is played on an 8x8 board with two players, Alice and Bob, who use black and white tokens, respectively. The game starts with four tokens placed in the center of the board. Players take turns placing tokens, with the requirement that each token placed must flip at least one of the opponent's tokens. The game ends when the board is full or neither player can make a legal move. The winner is determined by who has the most tokens on the board at the end of the game.

## Files Included

pr2_eng.pdf: Detailed description of the project requirements, including game rules, algorithm implementation guidelines, and the class interface for the Board.
Alfabeta.h/cpp: Implementation of the α-β pruning algorithm based on the provided Minimax algorithm.
Minimax.h/cpp: Original implementation of the Minimax algorithm.
heuristic.h/cpp: Contains the heuristic functions used to evaluate the game state. A non-informative heuristic is provided, and additional heuristics must be implemented for comparison.
## Implementation Instructions

Compile the Code: Follow the instructions in the explanation.txt file to compile the code. Ensure that you have a C++ compiler installed.
Run the Game: Execute the main program to start playing Otello using the implemented algorithms and heuristics. You can test the α-β algorithm against the Minimax algorithm or between different heuristics.
Heuristic Development: Implement at least two different heuristics in the heuristic.h/cpp files. The heuristics should evaluate the board state and provide scores for potential moves.
Testing: After implementing the heuristics, run tests to see how they perform against each other and document the results.
## Submission Requirements

A fully commented implementation of the α-β algorithm.
At least two heuristics with their respective implementations.
A file named explanation.txt containing compilation instructions and results obtained from testing the heuristics.
Source code must be sufficiently commented for clarity.
License
