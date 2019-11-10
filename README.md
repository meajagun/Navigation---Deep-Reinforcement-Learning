[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif "Trained Agent"

# Project 1: Navigation

![Trained Agent][image1]

Source: Udacity

### Project Overview

This project involves using Deep Reinforcement Learning (DRL) to train an agent how to navigate an environment and collect bananas.

DRL uses Deep Networks and Reinforcement Learning principles in creating algorithms. The algorithms through the use of an agent, evaluates the current state of the environment, takes appropriate actions, receives a reward for its action and evaluates the reward it gets (positive - did well and negative - failed). From several trials, the agent learns how to complete the task without making mistakes to achieve the goal and receive the maximum rewards

### Environment

The goal of this project is to use Deep Reinformcement Algorithms in this case Deep Q-Learning Network (DQN) to train the agent how to collect yellow bananas from an environment, while being able to differenciate between yellow and blue banana, avoiding blue bananas in the process.

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana.  Thus, the goal of the agent is to collect as many yellow bananas as possible while avoiding blue bananas.  

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.  Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

The task is episodic, and in order to solve the environment, the agent must get an average score of +13 over 100 consecutive episodes.

### Repository Contents
This repository contains the files listed below which were successfully used to train the agent to collect yellow bananas.
1. ***Navigation.ipynb:*** This file contains the starter code from Udacity's Repository and the implementation of the DQN Function used to train the agent.
2. ***dqn_agent.py:*** This file contains the DQN Agent class.
3. ***model.py:*** This file contains defined QNetwork architecture.
4. ***checkpoint.pth:*** This file contains the trained and saved QNetwork weights.
5. ***README.md:*** This file contains the overview of this project and how to understand its contents and implement one of your own.
6. ***report.md:*** This file contains a detailed report of the learning algorithm used in this project.

### Instructions

Follow the instructions in `Navigation.ipynb` to get started with training your own agent!

### Dependencies

The following are requirments to setup and run the code of this repository:
* ***python 3***
* ***numpy***
* ***PyTorch:*** Installation instructions [click here](https://pytorch.org/get-started/locally/)
* ***Unity ML-Agents:*** Installation instructions [click here](https://github.com/reinforcement-learning-kr/pg_travel/wiki/Installing-Unity-ml-agents-on-Windows)
* ***NVIDIA drivers on local machine***

### Getting Started

To get started on your own system and train an agent of your own similar to what is done here, follow the instructions below:
1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux_NoVis.zip) to obtain the environment.

2. Place the file in the DRLND GitHub repository, in the `p1_navigation/` folder, and unzip (or decompress) the file. 

### Original Udacity Code

To try out your own implementation, the original Udacity repository for this project can be found [here](https://github.com/udacity/deep-reinforcement-learning/tree/master/p1_navigation).