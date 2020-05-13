# Udacity-DRL-Navigation-Project
Implementation of an agent to solve the Unity Banana Collection task.

## Task
There are two different type of bananas: yellow and blue. The goal is to collect as 
many yellow bananas in one episode as possible (each collected yellow banana yields a 
reward of +1) while avoiding any blue ones (collecting one of those will result in 
a reward of -1). The bananas are arranged on a plane and the agent can move in this 
two-dimensional space. The task is completed if the agent manages to collect an average
reward of 13 or more in 100 consecutive episodes.

## States
A 37 dimensional vector that includes information about the agent velocity and its 
field of vision in the forward direction (ray-based).

## Actions
There are four different possible actions the agent can chose from to navigate along
the two axis of the world:
- forward (encoded as 0)
- backward (1)
- left (2)
- right (3)

## Getting Started
This repository includes three main pieces of code:
- `Navigation.inpynb` - a Jupyter Notebook which takes care of the actual training
- `model.py` - a Python class which defines the architecture of the PyTorch Deep Neural Net
- `dqn_agent.py` - a Python class for the implementations of the actual agent and a ReplayBuffer

There is no installation of Unity needed to run the code, you are however required to download
the built of the environment and change the path in the first cell of the Notebook to the location
of it. There are some further Python packages need of which most (if not all) should be automatically
installed by running `!pip -q install ./python` in the first cell of the Notebook.
If this should fail, please install the listed packages manually from your terminal.

## Training the Agent
To train the agent, simply run the Jupyter Notebook. If you wanna tweak details of the model and / or
the agent, look into the two Python classes.


