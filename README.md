# A GENETIC ALGORITHM IMPLEMENTATION WITH PYTHON

Genetic algorithms are a family of optimization algorithms that are inspired by the Theory of Evolution, introducing concepts such as mutation or crossover, simulating evolutionary processes where those most adapted to the environment are those that survive and reproduce, but how can this adaptation to the environment be measured in a digital world? Let's see how it works in more detail.

The genetic algorithm begins with a set of possible solutions (non-optimal usually)

Now, we must evaluate which are the most optimal to reproduce. For this, a function is applied that validates those that are more optimal or less optimal based on a rating. The best will be the ones who continue the process. That is, natural selection.

Once the ranking with the results has been generated, those best positioned on the natural scale are crossed or mutated. This process can be done in different ways:

### RECOMBINATION

-	***Recombination at a point:*** A point of each vector is selected, where the array is divided. The different divided parts are crossed to give the children:

 ![alt text](https://github.com/qgvidal/geneticAlgorithms/blob/main/images/ga1.jpg)

-	***Recombination in two points:*** Two points are selected in each vector, where the array is divided. The different divided parts are crossed to give the children:

 ![alt text](https://github.com/qgvidal/geneticAlgorithms/blob/main/images/ga2.jpg)

-	***Cut and splice:*** The vectors are divided by a random point, generating two new children with also random length:

 ![alt text](https://github.com/qgvidal/geneticAlgorithms/blob/main/images/ga3.jpg) 

### MUTATION

Mutation means switching two positions in the array as you can see in the image above, where two bits have been exchanged.

 ![alt text](https://github.com/qgvidal/geneticAlgorithms/blob/main/images/ga4.jpg)  

Once the best have been recombined or mutated, the solutions (descendants) are taken and re-evaluated in the optimization function, seeing now, again, which ones are the best. This process will be repeated N times.

The iterative algorithm will terminate for several reasons:

**A)**	Reach the number of iterations.

**B)**	You get an optimal result

One of the advantages of these algorithms is that they are capable of handling a large volume of data and parameters, which makes it possible to assess many possible solutions and casuistry. However, the evaluation function must be perfectly defined to provide optimal solutions.

The result may not be the best solution but it is an optimal solution. These algorithms are widely used in countless computationally complex problems to solve such as: airport optimization and optimization of container ships or in cybersecurity, for example.

