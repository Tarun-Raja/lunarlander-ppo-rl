# LunarLander Reinforcement Learning Agent using PPO

This project trains a reinforcement learning agent using Proximal Policy Optimization (PPO) to solve the LunarLander-v3 environment from Gymnasium.

The agent learns optimal landing behaviour through trial-and-error interaction with the environment, receiving rewards for stable landing and penalties for crashing or inefficient movement.

## Reinforcement Learning Concept

This project demonstrates policy-based reinforcement learning using PPO (Proximal Policy Optimization).

PPO updates the policy gradually to ensure stable learning while enabling the agent to improve through repeated interaction with the environment.

## Technologies Used

- Python
- Gymnasium
- Stable-Baselines3
- PPO (Proximal Policy Optimization)
- Matplotlib
- NumPy
- ImageIO
- Google Colab

## Reinforcement Learning Setup

### Agent

The Lunar Lander spacecraft.

### Environment

`LunarLander-v3` from Gymnasium.

### Actions

The agent can perform four discrete actions:

1. Do nothing
2. Fire left engine
3. Fire main engine
4. Fire right engine

### Reward System

Positive rewards are given for:

* Safe landing
* Stable orientation
* Low landing velocity

Negative rewards are given for:

* Crashing
* Drifting away from the landing zone
* Excessive fuel usage

### Goal

The objective is to maximize cumulative reward by learning an optimal landing strategy.

---

## PPO (Proximal Policy Optimization)

This project uses PPO, a policy-based Reinforcement Learning algorithm.

PPO improves learning stability by preventing excessively large policy updates during training.

Instead of learning fixed rules, the agent continuously interacts with the environment, receives rewards, and gradually improves its policy through iterative optimization.

### PPO Training Workflow

1. Interact with the environment
2. Collect experiences
3. Compute rewards
4. Update policy network
5. Repeat until performance improves

## Random Agent (Before Training)
The untrained agent takes random actions and crashes frequently.

<img width="600" height="400" alt="random_agent" src="https://github.com/user-attachments/assets/549fb18f-d05f-4182-bacd-0b7f683df4c4" />

## Training Performance
The graph below shows the improvement in rewards during training.

- Light blue: raw episode rewards
- Dark blue: smoothed reward trend
- Green dashed line: solved threshold

<img width="1500" height="600" alt="reward_curve" src="https://github.com/user-attachments/assets/96664e16-f2fb-4c2d-896b-6dd2e3d7b183" />

## Trained Agent (After Training)
After training for 1,000,000 timesteps, the agent learns to land successfully between the flags consistently.

<img width="600" height="400" alt="trained_agent" src="https://github.com/user-attachments/assets/31a344ff-7085-4246-88fa-03ba3e40751b" />

## Results
The agent was trained for 1,000,000 timesteps.

Training performance improved significantly over time, with rewards increasing from highly negative values during random exploration to stable positive rewards after learning.

The trained agent successfully learns to land between the flags consistently.

- Initial performance: highly negative rewards
- Final performance: stable positive rewards
- Mean evaluation reward improved significantly after training
- Agent successfully learned stable landing behaviour

## Key Learning

This project demonstrates how reinforcement learning agents can learn complex control behaviour through interaction and reward feedback without explicitly programmed rules.
