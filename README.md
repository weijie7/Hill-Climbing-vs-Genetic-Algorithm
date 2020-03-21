# Hill-Climbing-vs-Genetic-Algorithm
See how Hill Climbing and Genetic Algorithm can search from random string to find their way to "Hello, World!" strings!

### Hill Climbing:

In this example, we are going to have a set of strings or sentences as goal. And we are going to initialize our first solution from random strings from string.printable. Solutions will be evaluated to see how "far" are they from our goal. Solution with score would mean further away from goal.

Random mutation will be introduced. This approach is also known as Hill climbing by mutation and random choice appraoch. If the new found solution is better solution than the previous one, it will discard the previous one and take the current solution. Mutation will repeat until it reaches goal. Number of mutation will be recorded, trend of fitness converging to 0 will also be shown in the end.

Finally this will be compared to Genetic Algorithm approach to understand the difference in this case.

### Genetic Algorithm:

For Genetic Algorithm (GA), instead of single solution being mutated over and over, GA approach is evolution of entire population. To simuate this, we will need to initialize a population of solution.

Same thing, we will randomly initialize solution for a population size that we define. We also define our Surviving Rate (known as elite size in this example, where the fittest of the fittest in the population get retained over and over generation).

Next is Selection process, where we use Roulette Wheel / Wheel of Fortune to select a few of fitter solutions to replace the weaker solutions (by probability) in that population. From the selected population, we select a few solutions for crossover, based on crossover rate. Elite solutions will not be replaced or changed to keep the gene in the pool. Next is Mutation of single character in solutions, according to mutation rate. Again, elite solution will not be mutated. The result of these series of process will produce a new generation.

This entire process is looped until stop criteria is reached i.e. number of generation defined. Fitness trend will be plot against generations. Different mutation rate and crossover rate are also trialed to study the correlation to ultimate fitness of population.
