# Ant Puzzle

This repo contains the Ant puzzle and solution for the Graduate Researcher Position at Optiver.
Below is the problem description and questions. The solution can be found in the Jupyter notebook ('ants_sim.ipynb').
The notebook contains a monte carlo simulator for bounded and spatially unbounded problems.
Spatially unbounded problems should have a time/simulation limit determined by the ants maximum lifespan ('max_lifespan'); unless you have a lot of time...

## Requirements:
- Python 3.9+
- Numpy 1.23
- Multiprocess 0.70

----------

## Problem:
An ant leaves its anthill in order to forage for food. 
It moves with the speed of 10cm per second, but it doesn't know where to go, 
therefore every second it moves randomly 10cm directly north, south, east or west with equal probability.

### Question 1:
If the food is located on east-west lines 20cm to the north and 20cm to the south, 
as well as on north-south lines 20cm to the east and 20cm to the west from the anthill, 
how long will it take the ant to reach it on average?

### Question 2:
What is the average time the ant will reach food if it is located only 
on a diagonal line passing through (10cm, 0cm) and (0cm, 10cm) points?

### Question 3:
Can you write a program that comes up with an estimate of average time to find food for any 
closed boundary around the anthill? 
What would be the answer if food is located outside an area defined by
((x – 2.5cm) / 30cm )2 + ( (y – 2.5cm) / 40cm )2 < 1 in coordinate system 
where the anthill is located at (x = 0cm, y = 0cm)? 
Provide us with a solution rounded to the nearest integer.