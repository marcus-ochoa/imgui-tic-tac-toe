# Tic Tac Toe Base Submission
### Notes
For the most part, I followed the comments and TODOs closely. I also used some implementations from class (such as the kWinningTriples).
I added const class variables for the spacing of squares on the board for consistency and a boolean for AI state which allows the AI to be toggled.
From class I have a very broken minimax implementation which I plan to fix for next submission.
For the time being it does play and make moves, although they are terrible moves.
I feel like I could have used the state string a little more to save some function calls that check bits.
Otherwise I feel my implementation was very straightforward thanks to the given starting comments.

Platform - Linux
### Changes
I changed line 69 in the given CMakeLists file to use the library named in the file which allowed by code to compile properly\
I changed line 43 in the given Sprite.cpp file to check for linux along with apple to get proper dependencies

# Negamax Submission
### Notes
The AI uses what I understand to be pretty standard negamax with standard alpha-beta pruning.
I used the code done in class and the pseudocode found here: [Wikipedia Link](https://en.wikipedia.org/wiki/Negamax).
Wins are 10 points which is rather abitrary and there is no evaluation of non-terminal states.
All moves (except those pruned) are explored until terminal states are reached.
I still use winning triples to check for wins and I check for full boards / draws by finding zeros in the state string.
Overall I believe the algorithm is working as intended and as far as I can tell the AI plays pretty much perfectly.
The alpha-beta pruning also significantly reduced the number of recursions occuring each turn.
