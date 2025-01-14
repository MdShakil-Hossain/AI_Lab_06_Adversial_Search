# AI Lab 06 - Adversarial Search Report

## Introduction
This report documents the implementation of adversarial search algorithms to solve Pacman challenges. The task involved designing and testing agents using Reflex, Minimax, Alpha-Beta Pruning, Expectimax, and a custom evaluation function.

## Objectives
- To implement adversarial search algorithms for solving game challenges.
- To develop an evaluation function to improve decision-making.
- To meet performance benchmarks using the autograder.

## Implemented Algorithms
### Reflex Agent
The Reflex Agent evaluates game states based on:
- Distance to food.
- Proximity to ghosts.
- A heuristic function for immediate decisions.

### Minimax Agent
This agent:
- Implements the Minimax algorithm to find optimal moves.
- Considers adversarial behavior of ghosts.

### Alpha-Beta Pruning
Enhances Minimax by:
- Pruning branches that cannot affect the final decision.
- Improving efficiency without sacrificing accuracy.

### Expectimax Agent
Handles uncertainty by:
- Treating ghosts as stochastic agents.
- Using probability distributions for ghost actions.

### Better Evaluation Function
The evaluation function combines:
- Distance to the nearest food pellet.
- Penalty for proximity to ghosts.
- Game score to prioritize winning moves.

## Testing and Results
### Autograder
The implemented agents were tested using the autograder:
```bash
python autograder.py -q <question_number>
```
- The `<question_number>` corresponds to specific tasks:
  - `q1`: Tests Reflex Agent.
  - `q2`: Tests Minimax Agent.
  - `q3`: Tests Alpha-Beta Pruning.
  - `q4`: Tests Expectimax Agent.
  - `q5`: Tests Better Evaluation Function.

- All agents passed their respective tests successfully.

### Manual Testing
Manual testing was conducted on different layouts:
```bash
python pacman.py -p <AgentName> -l <Layout>
```
- Reflex Agent struggled in complex layouts.
- Minimax and Alpha-Beta Pruning performed efficiently.
- Expectimax handled randomness effectively.

## Observations
1. Reflex Agent is suitable for simple layouts but lacks depth.
2. Minimax ensures optimal decisions but is computationally expensive.
3. Alpha-Beta Pruning significantly reduces computational overhead.
4. Expectimax models ghost randomness realistically.
5. The Better Evaluation Function enhanced gameplay significantly.

## Conclusion
The project successfully implemented adversarial search algorithms to solve Pacman challenges. The Better Evaluation Function demonstrated substantial improvement, meeting all performance criteria.


## References
- UC Berkeley Pacman AI Projects: [http://ai.berkeley.edu](http://ai.berkeley.edu)
