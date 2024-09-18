# Gradient Descent

## Learning Goals

- explain and use the concept of a gradient;
- explain the algorithm of gradient descent;
- describe the effect of the "learning rate" in the algorithm.

## Lecture Materials

[Jupyter Notebook: Gradient Descent](gradient_descent.ipynb)

## Lesson Plan

### Introduction (5 Mins)

The game plan here is to experiment with and visualize different guesses as to the optimal parameters for a linear regression problem. This will illustrate the idea of improving one's guess based on the value of the last one (which is the substance of the gradient descent algorithm).

### Building a Function to Plot Different Regression Lines (15 Mins)

*We* are going to use our eyeballs on the line plots to judge regression lines. The computer cannot of course do that, but it can calculate some metric like RMSE.

### Visualizing the Loss Function (10 Mins)

The loss function for linear regression forms a paraboloid, and so we get the idea of the minimum loss corresponding to the **bottom of the hill**.

### Gradient Descent Algorithm (15 Mins)

The **gradient** is the higher-dimensional analogue of a derivative. Just like the derivative of a 1-d function provides the slope at any point, so the gradient provides the *direction* of greatest increase in a higher-dimensional space. Thus, we simply need to nudge our guesses in the opposite direction.

### Step Size (5 Mins)

The question of *how far* to nudge our guesses is answered by making our step proportional to the magnitude of the gradient at our last guess. This works because the gradient shrinks smoothly as we approach the optimal values, and so the gradient will be near 0 when we're close and far from 0 when we're far. The step size is further moderated by the learning rate, which is our tunable constant of proportionality.

### In Code (10 Mins)

The code walks through a version of gradient descent for a simple linear regression problem.