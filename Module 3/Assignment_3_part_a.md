# Part A: Code
One of the most useful applications of Machine Learning is to detect different diseases. In this
assignment, a heart disease data set is going to be used.

The following attributes(**features**) are used:
1. #3 (age)
2. #4 (sex)
3. #9 (cp)
4. #10 (trestbps)
5. #12 (chol)
6. #16 (fbs)
7. #19 (restecg)
8. #32 (thalach)
9. #38 (exang)
10. #40 (oldpeak)
11. #41 (slope)
12. #44 (ca)
13. #51 (thal)

More information about the data set: https://archive.ics.uci.edu/ml/datasets/Heart+Disease

The classification algorithm to be used will be K Nearest Neighbours (K-NN), a supervised learning method, in order to detect the presence of a heart disease.

One of the issues with these type of data sets is that some information can be useless or even can make the classifier to obtain a worst performance. For this reason, feature selection is one of the most important steps in Machine Learning.

***What to do:*** Your assignment now is to apply random-restart hill climbing and random-restart
Variable neighbour search as feature selection methods for the given problem. You have to run each
algorithm 10 times and give the average performance. You need to present the code to the teacher.
(1 point)

**How to use the given code:**
- Reading the dataset and K-NN is given in Assignment_3.py
- You have to install sklearn: pip install sklearn
- Here you have to change your code.

```python
#TODO: Write your algorithm as a funciton. You can add input parameters if you want.

def yourAlgorithm():
FITNESS_CALCULATIONS_COUNTER = 0

#Every time that you calculate the fitness value of a solution/combination you have to add one to FITNESS_CALCULATIONS_COUNTER. Example
# fitness = calculateFitness(currentSolution)
# FITNESS_CALCULATIONS_COUNTER += 1

if currentSolutionFitness > bestSolutionFitness:
    bestSolution = currentSolution
    bestSolutionFitness = currentSolutionFitness
    print("Best solution fitness ( ",FITNESS_CALCULATIONS_COUNTER,"/",

MAX_FITNESS_CALCULATIONS,"):", bestSolutionFitness)
# Condition to stop the algorithm
if FITNESS_CALCULATIONS_COUNTER >= MAX_FITNESS_CALCULATIONS:
    return bestSolution, bestSolutionFitness

bestSolution, bestSolutionFitness = yourAlgorithm()
```
- Every time that a fitness evaluation is calculated, 1 has to be added to FITNESS_CALCULATIONS_COUNTER. One example can be found in the code:

```python
#Every time that you calculate the fitness value of a solution/combination you have to add one to FITNESS_CALCULATIONS_COUNTER. Example
# fitness = calculateFitness(currentSolution)
# FITNESS_CALCULATIONS_COUNTER += 1
```

- The function will stop when the FITNESS_CALCULATION_COUNTER is greater than MAX_FITNESS_CALCULATIONS (5000):

```python
# Condition to stop the algorithm
if FITNESS_CALCULATIONS_COUNTER >= MAX_FITNESS_CALCULATIONS:
    return bestSolution, bestSolutionFitness
```

- When running the algorithm, you should print something like this:
```bash
Best solution fitness ( 1 / 5000 ): 57.78
Best solution fitness ( 10 / 5000 ): 63.64
Best solution fitness ( 11 / 5000 ): 67.44
Best solution fitness ( 22 / 5000 ): 68.67
Best solution fitness ( 168 / 5000 ): 69.05
Best solution fitness ( 236 / 5000 ): 71.43
Best solution fitness ( 674 / 5000 ): 73.49
Best solution fitness ( 2060 / 5000 ): 73.91
Best solution: [1, 1, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0]  Fitness: 73.91
```

Use the code given in: “Assignment_3.py”

Before defending the code, you have to send the code by email to johan.hjorth@mdu.se or jonatan.tidare@mdu.se.

**I will not consider a submission without the following format:**

File names for the submission:

StudentName_StudentLastName_Assignment3_Code.zip (Only by email)

Email subject for the submission:

[DVA264] StudentName StudentLastName Assignment3 Code
