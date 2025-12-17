Starter code and data for traveling salesman problem


Files in this directory:

* datareader.cpp : example code to read in the data files (use Makefile)
* datareader.py  : example code to read in the data files
* cities23.dat : list of coordinates for 23 cities in North America
* cities150.dat : 150 cities in North America
* cities1k.dat : 1207 cities in North America
* cities2k.dat : 2063 cities around the world
* routeplot.py : code to plot the globe and salesman's path<br>
usage:<br>
python routeplot.py cities.dat [cities2.dat] -r [="NA"],"World"'<br>
NA = North America, World = Mercator projection of the whole earth
* earth.C : (just for fun) plotting the globe in ROOT


INSTRUCTIONS FOR STUDENT RESPONSE
=================================

* All work was done in "the_plan.ipynb". As a fair warning, I spent some time debugging, so there's a number of validation functions floating around. Unless you want to follow my code exactly, all you need to see from the file are the annealing schedule plots at the bottom.
* cities150     327790.70 km     48627.37 km     9.38 s
* cities1k     2781799.58 km    102989.05 km     15.1 s
* cities2k    12040267.00 km    312940.95 km     18.2 s
* To test out trial configurations, I decided on swapping the path between two cities and calculating the new total distance. This has the advantage of untangling unnecessary loops. Obviously, I explored the phase space of this problem using the metropolis algorithm and simulated annealing.