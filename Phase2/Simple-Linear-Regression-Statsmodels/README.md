# Simple Linear Regression 

Two Parts (typically delivered across 2 one-hour blocks) - both use the same notebook.

# Part 1

## Learning Goals

- Explain and use the concepts of covariance and correlation

## Lecture Materials

- [Google Slides: Simple Linear Regression](https://docs.google.com/presentation/d/1DwCvkgzA0PmdwZJAqD82QJnwcR_AnGcFM74s5QxpDkQ/edit?usp=sharing)
- [Jupyter Notebook: Simple Linear Regression Lecture](Simple_Linear_Regression_Lecture.ipynb)

## Lesson Plan

### Introduction (5 Mins)

Centrality of LR:
- bridge between inferential / predictive stats
- bridge between statistics / ML
- fundamental modeling algorithm that will form the basis for other models

### Slides (40 Mins)

This time estimate includes the exercise of finding the best-fit line parameters, which should take 5-10 Mins.

### Correlation and Covariance (10 Mins)

### Conclusion (5 Mins)

Still need to implement Simple LR in code!

## Tips

The slides, including the exercise where I have students work on finding the LR parameters by hand, take me about 40 minutes. I aim for ending the lesson around the proof of the equations for the regression parameters, so that I start the second lesson with the interpretation and the assumptions of LR.


-----

# Part 2

This lecture is a demo of running and interpreting a regression model. It also introduces the idea of assumptions and their checks.

## Learning Goals

- Run simple linear regression in `statsmodels` and interpret the results
- Describe and check the assumptions of simple linear regression

## Lecture Materials

[Jupyter Notebook: Simple Linear Regression Lecture](Simple_Linear_Regression_Lecture.ipynb)

## Lesson Plan

### Introduction (5 Mins)

We're actually running our first model!! Hyyyyype!!!

### Statistical Learning Theory & Interpreting Coefficients (15 Mins)

Introduce the idea of errors/residuals and the desire to minimize them. Don't linger on proofs, just let them know that these estimates minimize error in ways that will make more sense when we talk about calc in Phase 3.

### `statsmodels` Demo Without & With Noise (20 Mins)

Unpack the syntax, talking about what the OLS object is and what it means to "fit" a model. Discuss the relevant parts of the results table (estimates, SEs, t/p values, R^2), with caveat that this is all wonky since we have a perfect model. Show differences in results once error is present. 

### Assumptions & Checks (15 Mins)

Talk about the assumptions, focus on interpreting residual plots and using them to identify problems. Let them know that they will get more practice with this in MLR.

### Conclusion (5 Mins)

Go forth and model!

