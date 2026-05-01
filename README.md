# LunarLander Reinforcement Learning Agent using PPO

This project trains a reinforcement learning agent using Proximal Policy Optimization (PPO) to solve the LunarLander-v3 environment from Gymnasium.

The agent learns optimal landing behaviour through trial-and-error interaction with the environment, receiving rewards for stable landing and penalties for crashing or inefficient movement.

## Technologies Used

- Python
- Gymnasium
- Stable-Baselines3
- PPO (Proximal Policy Optimization)
- Matplotlib
- NumPy
- ImageIO
- Google Colab

## Results

The agent was trained for 1,000,000 timesteps.

Training performance improved significantly over time, with rewards increasing from highly negative values during random exploration to stable positive rewards after learning.

The trained agent successfully learns to land between the flags consistently.

<img width="1500" height="600" alt="reward_curve" src="https://github.com/user-attachments/assets/ab290560-a3a8-454e-9b20-e847adb92d97" />

<img width="600" height="400" alt="trained_agent" src="https://github.com/user-attachments/assets/21cb7d77-1efc-44db-98d0-282ece247520" />

<img width="600" height="400" alt="random_agent" src="https://github.com/user-attachments/assets/fe4458c0-201a-42b9-9001-8e86c2cf9d26" />
