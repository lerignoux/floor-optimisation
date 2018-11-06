# floor-optimisation
Trying to help with floor plan seats assignation

## Description
We have a graph of nodes with a weight between each of the nodes (distance between nodes). This represent the seats available

We then have a second graph with some weights between people (the people).
The weight represent the interest of people being close to each other

We want to find the seat repartition to try to get the optimal placement so that people are as much as possible close to people they are related to.

## Algo
### Using MonteCarlo
We take a random filling.
We consider each permutation of two people
We apply the best permutation
We iterate until there is no positive permutation

This should ensure a local optimum, We take multiple samples and loop to find the best local optimum

### Proof of result
We need to ensure this converge towards the global best optimum
TODO
