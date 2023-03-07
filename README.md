# Random-Search-Optimization-Techniques

## Genetic Algorithm
### Pseudo code:

1 - Calculate the distance matrix for data points

2 - Generate the initial population
	
	In this step, you can generate a random population or use other heuristic or meta-heuristic techniques to generate it

3- Start iterating n times:

	3.1 Elite the best solutions in the current population
  
	3.2 Perform crossover with a specified probability
  
	3.3 Mutate some solutions with a specified probability
  
	3.4 Form the new population
  
  
### Crossover:

1- Choose 2 parents with a tournament selection 'best fitness from a random sample'
3- In case of PMC crossover, add  result child to the next generation.


### PMC crossover:

1- Generate 2 random split points

2- Swap the genes within the generated range with one condition: there are no duplicate genes in the same chromosome. for more info: 


### Mutation:

There are many ways to perform mutation.

The one used here is generate random number swap chromosome genes



## Ant colony Algorithm
### Pseudo code:

1 - Calculate the distance matrix for data points

2 - Generate the initial population

In this step, you can generate a random population or use other heuristic or meta-heuristic techniques to generate it, I create that by random.

3- Generate the initial pheromone matrix then update it using the initial population. Note (initial pheromone using zeros add small number to aviod divide by zero)

3- Start iterating n times:

	3.1 Construct a new population

	3.2 Update the pheromone matrix with the new population
  

### Construction:

Construct n solution. To construct each one:

1- Choose a random point as a start

2- Calculate p value between this point and other unvisited points

3- Select the point with the max p value as the next destination

4- Add the selected point to the path 

5- Repeat until constructing the whole path

### Demo 


https://user-images.githubusercontent.com/55801427/223328256-0c75eb39-0f54-485d-8a7e-3ff1a461c672.mp4

