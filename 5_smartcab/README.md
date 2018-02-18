## Project 5: Train a Smartcab How to Drive
GOAL: Apply reinforcement learning technique on a self-driving agent in a simplified world to aid it in effectively reaching its destinations in the allotted time. 

### Software Requirements
- [Python 2.7](https://www.python.org/download/releases/2.7/)
- [NumPy](http://www.numpy.org/)
- [pandas](http://pandas.pydata.org/)
- [matplotlib](http://matplotlib.org/)
- [Pygame] (https://www.pygame.org/wiki/GettingStarted)
- Jupyter Notebook

Double check if pygame was installed correctly
`python -m pygame.examples.aliens`

### Data
Here, we're not working with actually dataset (hence no features) therefore it's important to get an idea of how smartcab/agent.py works:
1) Environment: agent is operating in a grid-like city with roads going North-South and East-West directions. Assuming there are no pedestriants and traffic is controlled by traffic lights (with US right-of-way rules applied)
2) Input/ Output:
- `'waypoint'`, which is the direction the *Smartcab* should drive leading to the destination, relative to the *Smartcab*'s heading.
- `'inputs'`, which is the sensor data from the *Smartcab*. It includes 
  - `'light'`, the color of the light.
  - `'left'`, the intended direction of travel for a vehicle to the *Smartcab*'s left. Returns `None` if no vehicle is present.
  - `'right'`, the intended direction of travel for a vehicle to the *Smartcab*'s right. Returns `None` if no vehicle is present.
  - `'oncoming'`, the intended direction of travel for a vehicle across the intersection from the *Smartcab*. Returns `None` if no vehicle is present.
- `'deadline'`, which is the number of actions remaining for the *Smartcab* to reach the destination before running out of time.
3) Reward and goal: the agent would receive positive or negative reward based on the action it takes. It receives a small positive reward when making a good action, and a varying amount of negative reward dependenting on the severity of the traffic violation it would have committed. Based on rewards, agent would learn how to obey traffic rules, avoid accidents and get to destination on time.

This project contains three directories:

- `/logs/`: This folder will contain all log files that are given from the simulation when specific prerequisites are met.
- `/images/`: This folder contains various images of cars to be used in the graphical user interface. You will not need to modify or create any files in this directory.
- `/smartcab/`: This folder contains the Python scripts that create the environment, graphical user interface, the simulation, and the agents. You will not need to modify or create any files in this directory except for `agent.py`.

It also contains two files:
- `smartcab.ipynb`: This is the main file where you will answer questions and provide an analysis for your work.
-`visuals.py`: This Python script provides supplementary visualizations for the analysis. Do not modify.

Finally, in `/smartcab/` are the following four files:
- **Modify:**
  - `agent.py`: This is the main Python file where you will be performing your work on the project.
- **Do not modify:**
  - `environment.py`: This Python file will create the *smartcab* environment.
  - `planner.py`: This Python file creates a high-level planner for the agent to follow towards a set goal.
  - `simulation.py`: This Python file creates the simulation and graphical user interface. 
  
### Key take aways:
- Implement Q-Learning to guide the agent
- How to use Exploration-Exploitation factors

### What's Next?