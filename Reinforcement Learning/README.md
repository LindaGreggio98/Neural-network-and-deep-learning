# Deep Q-Learning — CartPole and MountainCar

This repository contains the implementation and analysis of **Deep Q-Networks (DQN)** applied to classic **Reinforcement Learning** environments from OpenAI Gym.

The main goal of this project is to study how deep neural networks can approximate the **action–value (Q) function** and learn optimal control policies through interaction with an environment. We investigate:

- Q-function approximation with deep neural networks  
- Stable training via **target networks** and **experience replay**  
- The impact of **reward shaping** on learning behavior and policy quality  

## Features
- Deep Q-Network (DQN) implementation  
- Target network with periodic updates  
- Experience replay buffer  
- Huber loss optimized with Adam  
- Discretization of continuous action spaces  

## Environments

### CartPole-v1
- Discrete action space  
- Reward for maintaining pole balance  
- Reward shaping to improve learning stability  

### MountainCarContinuous-v0
- Continuous action space (discretized)  
- Momentum-based control task  
- Analysis of unintended behaviors induced by reward shaping  

## Experiments
The following analyses are included:

- Training dynamics and convergence of DQN policies  
- Comparison of different reward shaping strategies  
- Evaluation of learned policies across environments  
