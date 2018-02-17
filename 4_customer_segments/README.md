## Project 4: Creating Customer Segments
GOAL: Using unsupervised learning techniques, find meaningful relationships hidden between customers of a wholesale distributor in Lisbon, Portugal. The wholesale distributor wants to make informed business decision of changing their delivery method from a morning delivery service five days a week to a cheaper evening delivery service three days a week. See if any similarities exist between customers, and how to best segment customers into distinct categories.

### Software Requirements
- [Python 2.7](https://www.python.org/download/releases/2.7/)
- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)
- Jupyter Notebook

## Data
The customer segments data contains 440 data points collected on data found from clients of a wholesale distributor in Lisbon, Portugal.

Note: (m.u.) = *monetary units*.

**Features**
1) `Fresh`: annual spending (m.u.) on fresh products (Continuous); 
2) `Milk`: annual spending (m.u.) on milk products (Continuous); 
3) `Grocery`: annual spending (m.u.) on grocery products (Continuous); 
4) `Frozen`: annual spending (m.u.) on frozen products (Continuous);
5) `Detergents_Paper`: annual spending (m.u.) on detergents and paper products (Continuous);
6) `Delicatessen`: annual spending (m.u.) on and delicatessen products (Continuous); 
7) `Channel`: {Hotel/Restaurant/Cafe - 1, Retail - 2} (Nominal)
8) `Region`: {Lisnon - 1, Oporto - 2, or Other - 3} (Nominal) 

This project contains three files:

- `customer_segments.ipynb`: main file
- `customers.csv`: dataset
- `visuals.py`: supplementary file to help visualize (graph)

### Key take aways:
- Explore feature scaling, outlier detection
- Learnt to interpret data points that's scaled, transformed or reduced using PCA
- Analyze PCA dimensions and construct a new feature space
- Finding meaningful way to get info out of clustered data 

### What's Next?
Using the full dataset (fromhttps://archive.ics.uci.edu/ml/datasets/Wholesale+customers) try to ....