## Project 1: Titanic Survival Exploration
GOAL: In 1912, the ship RMS Titanic struck an iceberg on its maiden voyage and sank, resulting in the deaths of most of its passengers and crew. We would look into RMS Titanic passenger manifest to determine WHICH features best predict whether someone survived or did not survive.

## Software Requirements
- [Python 2.7](https://www.python.org/download/releases/2.7/)
- [NumPy](http://www.numpy.org/)
- [pandas](http://pandas.pydata.org/)
- [matplotlib](http://matplotlib.org/)
- Jupyter Notebook

### Data
The modified Titanic data contains 11 features:

**Features**
- `pclass` : Passenger Class (1 = 1st; 2 = 2nd; 3 = 3rd)
- `name` : Name
- `sex` : Sex
- `age` : Age
- `sibsp` : Number of Siblings/Spouses Aboard
- `parch` : Number of Parents/Children Aboard
- `ticket` : Ticket Number
- `fare` : Passenger Fare
- `cabin` : Cabin
- `embarked` : Port of Embarkation (C = Cherbourg; Q = Queenstown; S = Southampton)
- `survival` : Survival (0 = No; 1 = Yes)

This project contains three files:
- `titanic_survival_exploration.ipynb`: main file
- `titanic_data.csv`: dataset
- `visuals.py`: supplementary file to help visualize (graph) and filter by features using 'survival_stats' method

### What's Next?
Using the full dataset try to redo the project applying `Decision Trees`!