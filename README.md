# Project_2

This repository is Project 2 Continuous Control Option 1 in Udacity Deep Reinforcement Learning. 

## Getting started

The framework is based on Pytorch and Python 3.6. 

My implementation is based on Windows 10 OS and did the following from the dependencies section of https://github.com/udacity/deep-reinforcement-learning:

conda create --name drlnd python=3.6

conda activate drlnd

pip install gym

pip install unityagents==0.4.0

pip install .

conda install pytorch=0.4.0 -c pytorch  # Some errors occurred when I ran the above line. My Undacity mentor suggested this line. 

Once the above steps are done, one needs to clone this repository to get the working code and saved model weights.

## Project environment

This environment simulates a double-jointed arm that can move to target locations. The state space is a 33-variable vector, representing position, rotation, velocity, and angular velocities of the arm. The action space is a 4-variable vector, representing torques applied to two joints. Each element in the action space ranges between -1 and 1. 

A reward of +0.1 is gained for each time step that the arm is in the goal position. The goal of the agent is to maintain its position at the target location for as long as possible. This environment is considered solved when the agent accumulates an average socre of 30.0 or more in 100 consecutive episodes. 

## How to run

Python code main.py in the repository contains all necessary code for this project. Ddpg() in main.py is the entry function to train a model. Meanwhile, the main body of code is a complete workflow for training. Running python main.py will start training automatically. The script will save intermediate model into checkpoint file. 

A set of pretrained models have been already saved in this repository as .pth files. 
