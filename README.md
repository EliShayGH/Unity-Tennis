# Udacity Deep Reinforcement Learning Nanodegree

## Project 3: Collaboration and Competition

### Project details

In this project I solved the [Tennis](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#tennis) environment.

In this environment, two agents control rackets to bounce a ball over a net. If an agent hits the ball over the net, it receives a reward of +0.1. If an agent lets a ball hit the ground or hits the ball out of bounds, it receives a reward of -0.01. Thus, the goal of each agent is to keep the ball in play.

The observation space consists of 8 variables corresponding to the position and velocity of the ball and racket. Each agent receives its own, local observation. Two continuous actions are available, corresponding to movement toward (or away from) the net, and jumping.

### Solving the Environment

The task is episodic, and in order to solve the environment, your agents must get an average score of +0.5 (over 100 consecutive episodes, after taking the maximum over both agents). Specifically,

After each episode, we add up the rewards that each agent received (without discounting), to get a score for each agent. This yields 2 (potentially different) scores. We then take the maximum of these 2 scores.
This yields a single score for each episode.

### Getting Started

1. Clone and install dependences for the Udacity DeepRL Nanodegree found at [Udacity DeepRL](https://github.com/udacity/deep-reinforcement-learning#dependencies), which are required by this DDPG agent's implementation

2. This project requires `python 3.6` and a Unity virtual environment. You do not need to install Unity directly for this project. Instead, you can download a pre-build environment from one of the following links based on your operating system::<br>

<b>Version 1: One (1) Agent:<b><br>

- Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux.zip)
- Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis.app.zip)
- Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86.zip)
- Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86_64.zip)

3. Clone this GitHub repository and unzip the Unity Tennis environment into its root directory.

### Instructions

To train the agent run all the cells in [Tennis.ipynb](Tennis.ipynb) notebook.

Description of the implementation is provided in [report.md](report.md).
For technical details see the code in the notebook.

Agent's weights are stored in [checkpoint_actor.pth](checkpoint_actor.pth) and [checkpoint_critic.pth](checkpoint_critic.pth)
