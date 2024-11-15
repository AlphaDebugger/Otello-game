# Otello
The first objective of this exercise, to be developed in two sessions, is to understand and implement the α − β algorithm for resolution of game trees. The algorithm should be implemented as generally as possible, but it will be tested applying it to the game of Otello. In addition you must devise several game heuristics and make them compete against each other, either between those made by the components of the same group or against those made by other groups.
The rules of Otello are: we have a square board made by 64 squares (8 rows and 8 columns). 64 tokens exist with the shape of a coin and with different colors or symbols on each side (as in real coins). In our case, let’s say one face white and the other black.
Each player is associated with a color (face) of the tokens. Starting with the player who plays with black, each player places a token in any of the free squares with a restriction: when doing so, at least one token of the opponent’s color should be reversed. A token must be reverted if it is aligned horizontally, vertically, or diagonally between two of the opposite color, and also the whole line between them is continuously occupied (without holes) by tokens of the same color. This means e.g. that from the starting position, the first move of black could only be either to E3 (then, flipping the white token at E4), to C5 (flipping D5), to F4 (flipping E4) or to D6 (flipping D5).
If a player cannot place any token of his color according to these rules, he must pass, and only in that case is he allowed to do so. The game ends when all the 64 tokens are on the board, or when none of the two players can put more tokens. The winner is the player whose color is displayed at that time in more tokens on the board, or the two players tie in case of equality in number of tokens.
The result you must submit is:
The implementation of the α − β algorithm and its test in the game.
The implementation of at least two heuristics and their test in the game playing one against the other.
A file explanation.txt in ASCII text with the compilation instructions and results obtained with each heuristic.
The source code SUFFICIENTLY COMMENTED will have to be submitted, too.
Some data type are defined and a class Board is provided to help with the implementation. The data types are:
Type Square: typedef pair<char,char>Square. It is a pair of two characters that represents a square of the board. To be valid, the first character must be ’1’,...,’8’ (the row), and the second, ’A’,...,’H’ (the column). Notice that digits are represented as characters, not as integers.
Type Sqlist: typedef list<Square>Sqlist. A list of squares.
Type Token: defined as an enumerated type enum Token {x,o,e }. Letter o represents a black square,
x represents a white one and the e an empty square.
