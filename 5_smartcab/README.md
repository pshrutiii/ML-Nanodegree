## Project 5: Train a Smartcab How to Drive
GOAL: Apply reinforcement learning technique on a self-driving agent in a simplified world to aid it in effectively reaching its destinations in the allotted time. 

### Software Requirements
- [Python 2.7](https://www.python.org/download/releases/2.7/)
- [NumPy](http://www.numpy.org/)
- [pandas](http://pandas.pydata.org/)
- [matplotlib](http://matplotlib.org/)
- [Pygame](https://www.pygame.org/wiki/GettingStarted)
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

This project contains:

- `/logs/`: after you run simulations, files would be generated here
- `/images/`: if you turn on GUI, you can see traffic in action using pygame
- `/smartcab/`: has pythong files that create environment, GUI interface, simulation, and agents.
	- `agent.py`: main file
	- `environment.py`: creates environment
	- `planner.py`: high-level planner for the agent to follow towards a set goal
	- `simulation.py`: creates simulation and GUI 
- `smartcab.ipynb`: report
- `visuals.py`: supplementary file to help visualize (graph)

### Key take aways:
- Implement Q-Learning to guide the agent
- How to use Exploration-Exploitation factors

### What's Next?