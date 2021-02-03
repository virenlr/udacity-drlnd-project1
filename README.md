# udacity-drlnd-project1
This is the first project done as part of Udacity's Deep Reinforcement Learning Nanodegree.

## Project Details

This project uses the Banana Collector environment in Unity's ML toolkit. The goal is to navigate and collect bananas in the world.

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of the agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The GIF below was taken directly from Udacity's project page.

![Project Demo](https://raw.githubusercontent.com/virenlr/udacity-drlnd-project1/main/Demo.gif "Project Demo")

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:

`0` - Move Forward
`1` - Move Backward
`2` - Turn Left
`3` - Turn Right

The task is episodic, and in order to solve the environment, the agent must get an average score of +13 over 100 consecutive episodes.

## Getting Started

#### Step 1: Clone my repository

You will need the Report.ipynb file, as well as the Python files titled `dqn_agent.py` and `model.py`. Please ensure these are all placed in the same folder.

#### Step 2: Setup the required dependencies

1. Create (and activate) a new environment with Python 3.6.

Linux or Mac:

```
conda create --name drlnd python=3.6
source activate drlnd
```

Windows:

```
conda create --name drlnd python=3.6 
activate drlnd
```

2. Perform a minimal installation of OpenAI Gym

```
pip install gym
```

3. Clone the repository from [Udacity's GitHub page](https://github.com/udacity/deep-reinforcement-learning), and navigate to the python/ folder. Then, install several dependencies.

```
git clone https://github.com/udacity/deep-reinforcement-learning.git
cd deep-reinforcement-learning/python
pip install .
```

4. Create an IPython kernel for the `drlnd` environment.

```
python -m ipykernel install --user --name drlnd --display-name "drlnd"
```

5. You may have to install other dependencies with pip, like Unity ML and PyTorch. You will know when you start executing the cells in my notebook.

6. Before running the code in the notebook, change the kernel to match the drlnd environment by using the drop-down Kernel menu.

#### Step 3: Download the environment

Download the Unity environment corresponding to your operating system with the links provided by Udacity.

Linux: [Click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
Mac OSX: [Click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
Windows 32-bit: [Click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
Windows 64-bit: [Click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)

Then, place the file in the same folder as the other files you downloaded from my repo and unzip (or decompress) it.

## Instructions

With the environment set up, you can simply open and execute the cells of the Jupyter notebook, one by one. Feel free to take a look at the code in `dqn_agent.py` and `model.py` as well.
