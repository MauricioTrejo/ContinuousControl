# Continuous Control

Moving robotic arms with Reinforcement Learning.

## Index

1. [Project](#project)
2. [Requirements](#requirements)
3. [Installation](#installation)
4. [Files](#files)
5. [Acknowledgement](#acknowledgement)

<a name="project"></a>
## Project

In this project we try to move a double-jointed arm to target locations with a reward of +0.1 for each step that the agent's hand is in the goal location.

![IMAGE ALT TEXT](reacher.gif)

The space consists of 33 variables corresponding to position, rotation, velocity and angular velocities of the arm. Every entry in the action vector should be a number between -1 and 1.

The goal of each agent is to keep its position at the target location for as many time steps as possible.

There are 2 versions of the environment, the first has 1 agent and the second has 20 agents. To solve the environment in the first version you must reach an average score of +30 while for the second version, the average score of the 20 agents must be +30 over 100 episodes.

<a name="requirements"></a>
## Requirements

Packages needed for this project:

tensorflow 1.7.1 and [torch 0.4.0](https://pytorch.org/get-started/previous-versions/)

<a name="installation"></a>
## Installation

In order to run this project is important to set a python environment, you can follow the instructions [here](https://github.com/udacity/deep-reinforcement-learning#dependencies). 
  - There are 2 ways to install tensorflow 1.7.1 in your environment, one is with conda and the other is with pip (which is the one we recommend since conda installer has problems with this version of tensorflow)
  - Also, is important to note that the installation of torch has to be from [here](https://pytorch.org/get-started/previous-versions/), otherwise, neither pip nor conda will find the version.

<a name="files"></a>
## Files

- [agent](https://github.com/MauricioTrejo/ContinuousControl/blob/master/agent.py) is the py file containing the agent.
- [model](https://github.com/MauricioTrejo/ContinuousControl/blob/master/model.py) is the py file containing the neural networks of actor and critic.
- [actor weights](https://github.com/MauricioTrejo/ContinuousControl/blob/master/checkpoint_actor.pth) contains the weights of the trained actor.
- [critic weights](https://github.com/MauricioTrejo/ContinuousControl/blob/master/checkpoint_critic.pth) contains the weights of the trained critic.
- [Report](https://github.com/MauricioTrejo/ContinuousControl/blob/master/Report.ipynb) contains the report of the agent training.
- [data/](https://github.com/MauricioTrejo/ContinuousControl/tree/master/data) is Unity's environment for 1 and 20 agents.
- [python/](https://github.com/MauricioTrejo/ContinuousControl/tree/master/python) has necessary files for Unity's environment.
- [reacher](https://github.com/MauricioTrejo/ContinuousControl/blob/master/reacher.gif) is a gif with the environment of the project.

<a name="acknowledgement"></a>
## Acknowledgement

We want to thank [Unity](https://unity.com/) and [Udacity](https://www.udacity.com/) for the environment and training to solve this project.

