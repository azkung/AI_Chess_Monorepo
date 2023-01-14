# Chess AI Monorepo
#### by Alexander Kung

The following repository is a multi-year personal research/learning project. The repositories in this monorepo are some of the several chess AI agents that I have programmed over the years. All agents make use of various algorithmic and ML/DL concepts in order to play the complex game of chess.

## Version Summary

| Version | Description |
| ------ | ------ |
| 1.0-1.1 | The repository includes a fully programmed chess game and UI as well as an AI agent that makes use of the minimax algorithm, in order to make informed chess moves. This agent creates a decision tree, and traverses the tree using alpha beta pruning, in order to determine the move the agent must use to establish the optimal tree traversal. |
| 2.0-2.2 |Similar to version 1, version 2.0 includes the same chess agents and UI, however with optimizations to the chess engine itself, is able to improve upon the agent's performance. |
| 3.0 | Slight alterations to the chess engine, while including more chess agents capable of scoring boards in different unique ways. Agents are now able to prioritize styles that tend towards more aggressive moves or more control over middle board positions.  |
| 4.0 | A final optimization of the chess engine, including all of version 3.0 agents. |
| 5.0 | Discards the personally programmed chess engine in favor of the python-chess library. Making use of a DNN (Deep Neural Network), the chess agent is now capable of evaluating a board given its state. This DNN scoring system is then implemented into a minimax algorithm to choose ideal moves. The DNN itself is trained on millions of boards where the labelled scoring is determined by the outcome of the game. The dataset is skewed so that later game boards are more common, as the state of later game boards are clearer on the probable winner. |
| 5.1 | An expansion on version 5.0, version 5.1 uses an overhauled board input (a 6x8x8 tensor) while making use of a CNN (Convolutional Neural Network) in order to score the board. The logic behind the CNN is to identify and score trends between relative piece positions. The CNNs excel at identifying trends between adjacent data positions, hence the logic here is the CNN may be able to prioritize positions that keep pieces protected by one another. |
| 5.5 | Use of the previous CNN to improve the performance of minimax alpha-beta pruning. Also an additional implementation of a C++ chess engine for faster query and chess calculation | 
