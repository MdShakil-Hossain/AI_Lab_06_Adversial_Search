# AI Lab 06 - Adversarial Search Report

This report outlines the implementation of adversarial search algorithms for solving Pacman challenges, including Reflex Agent, Minimax, Alpha-Beta Pruning, Expectimax, and a custom evaluation function.

## Objectives
- Implement adversarial search algorithms.
- Develop an optimized evaluation function.
- Pass autograder tests and meet task requirements.

## Project Overview

### Implemented Algorithms
- **Reflex Agent**: Evaluates game states based on food and ghost distances.
- **Minimax Agent**: Computes optimal moves considering adversarial ghosts.
- **Alpha-Beta Pruning**: Optimized Minimax to reduce computation time.
- **Expectimax Agent**: Handles stochastic ghost behavior.
- **Better Evaluation Function**: Combines heuristics for food, ghost distance, and game score.

### Testing and Results
- **Autograder**: Successfully passed all tests using:
  ```bash
  python autograder.py -q <question_number>
  ```
- **Manual Testing**: Tested agents on layouts using:
  ```bash
  python pacman.py -p <AgentName> -l <Layout>
  ```

## Observations
- Reflex Agent performs well in simple layouts.
- Minimax and Alpha-Beta handle adversarial scenarios efficiently.
- Expectimax models ghost randomness effectively.
- Better Evaluation Function balances food collection and ghost avoidance.

## Conclusion
The project successfully implemented and tested adversarial search algorithms, meeting all requirements. The Better Evaluation Function significantly improved performance.

## Future Work
- Incorporate additional factors like power pellets.
- Explore reinforcement learning for optimization.
