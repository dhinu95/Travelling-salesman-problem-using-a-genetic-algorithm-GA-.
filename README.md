# Travelling salesman problem using a genetic algorithm(GA)
### Condition: Shortest possible route that visits each city once and return origin.
**Greedy algorithm:** Algorithmic strategy that makes the best optimal choice at each small stage with the goal of this eventually leading to a globally optimum solution. This means that the algorithm picks the best solution at the moment without regard for consequences.

City has been visited that city is not eligible to be travelled to again, the size of the search space stands as n! possible **permutations**.

**Fitness function** calculates the total distance between each city in the chromosome’s permutation.

**Selection** Probability to create bias in choosing fitter chromosomes to serve as the parents.

**Mutation action** is modified to avoid creating repetition of cities visited

we rank the routes in the current generation using **rankRoutes**. We then determine our potential parents by running the **selection function**, which allows us to create the mating pool using the **matingPool function**. Finally, we then create our new generation using the **breedPopulation** function and then applying mutation using the **mutatePopulation function**.
