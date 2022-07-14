# reinforcement_learning
Implements an RL agent via Q-Learning in the tabular and function approximation settings.

In the CartPole environment, there is a pole standing up on top of a cart. The goal is to balance this pole by moving the cart from side to side to keep the pole balanced upright. A reward of +1 is provided for every timestep that the pole remains upright, and the episode ends when the pole is more than 15 degrees from vertical, or the cart moves more than 2.4 units from the center.

### Requirements

`pip3 install gym`

`pip3 install tqdm`

### Algorithm

1. Initialize Model

2. Rollout trajectories using current model and store it into the replay memory

3. Sample data from the replay memory to update the model's Q-value estimates

4. Repeat steps 2-4 until convergence

### Run

For tabular Q learning, `python mp6.py --model tabular.npy --episodes 8 --epsilon 0` should yield 200+ score.

