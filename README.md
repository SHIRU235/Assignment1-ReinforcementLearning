# Assignment1-ReinforcementLearning
This project contains solutions for Gridworld and Pick-and-Place Robot (MDP design) tasks as part of the Reinforcement Learning assignment.

## Project Structure

├── AssignmentRL.ipynb
├── requirements.txt     # Python dependencies
└── README.md            # Project documentation

## Problems Covered

1. 5x5 Gridworld
•	Implements a simple grid environment.
•	Demonstrates Off-policy Monte Carlo control to estimate value functions.
•	Example output includes the estimated value function across the grid.

2. Pick-and-Place Robot (MDP Design)
•	Formulated as a Markov Decision Process (MDP).
•	Components defined:
–	States: Joint angles, velocities, and end-effector pose.
–	Actions: Joint torques or position increments.
–	Transitions: Deterministic robot dynamics.
–	Rewards: Positive reward for successful placement, penalties for collisions or failures.
–	Discount Factor: Models long-term planning.

## Installation
1.	Clone this repository:
 	git clone https://github.com/SHIRU235/Assignment1-ReinforcementLearning.git .
cd rl-assignment
2.	Create a virtual environment (optional but recommended):
 	python -m venv venv
source venv/bin/activate   # On Linux/Mac
.venv\scripts\activate      # On Windows
3.	Install dependencies:
 	pip install -r requirements.txt

## Requirements
Dependencies are listed in requirements.txt:
numpy
Note: time module is part of Python’s standard library, no installation required.

## Example Gridworld Output
Estimated Value Function (V):
[-5.6953 -5.217  -4.6856 -4.0951 -7.439 ]
[-5.217  -4.6856 -4.0951 -3.439  -2.71  ]
[-4.6856 -4.0951 -7.439  -2.71   -1.    ]
...

## Future Improvements
•	Add visualization for Gridworld trajectories using matplotlib.
•	Implement Q-learning or SARSA for Gridworld.
•	Extend Pick-and-Place to a simulated robotics environment (e.g., PyBullet).

