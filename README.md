# Week1-InClass-Task1-Distance-Finder
finding the distance between two random points in a rectangle

Here's some pseudocode for this problem:

```{r}
#How many simulations to run?
NumberOfSims<-1000
#What is the size of the grid?
a<-10
b<-5
set.seed(123)  # set the seed for the random number generator - this makes sure the results are reproducible when we are debugging

#Declare a variable to keep track of the sum of the distances across all simulations
Distance<-0

for (i in 1:NumberOfSims){
  # generate z1 (so generate it's x and y coordinates)
  z1<-cbind(runif(1,0,a),runif(1,0,b))
  # generate z2 (likewise)


  # Use Pythagoras' theorem to find the distance between them

  # Add the distance to the variable Distance
}

# Divide Distance by NumberOfSims to calculate the average distance we observed across all sims
AverageDistance<-Distance/NumberOfSims

# report that number
cat("\nOur estimate of the expected distance between the two points is ",AverageDistance)

# Better still, keep each distance in a vector and then plot a histogram of its distribution? Is the distribution from a family you recognize? (e.g. Normal, Poisson, Exponential,...?)
```{r}
