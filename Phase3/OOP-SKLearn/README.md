# OOP With Scikit-Learn

Use the familiarity of OOP to show how to extend Scikit-Learn objects with the API via inheritance and duck typing.

## Learning Goals

- Understand the concept of object-oriented inheritance
- Understand the main object types of the Scikit-Learn API
- Extend and create custom Scikit-Learn Estimators

## Lecture Materials

[Jupyter Notebook: OOP with SKLearn](oop_with_scikit_learn.ipynb)

## Lesson Plan

### Inheritance (10m)

Walk through inheritance from the class being explored throughout the lecture. Build the new class to show the benefits from inheritance (avoid boilerplate code).

### Duck Typing (5m)

Introduce duck typing concept and explain it used in Scikit-Learn API.

### Scikit-Learn's API (15m)

Explain Scikit-Learn's API, specifically what defines Estimators, Transformers, and Predictors. Emphasis on the key methods associated with each.

Take some time (if available) to observe source code for `StandardScaler`.

### Creating a Scikit-Learn Transformer (15m)

Go step-by-step in creating a custom Scikit-Learn Transformer by creating `fit()` and `transformer()` methods. Point out the relevant inheritance and duck typing.

### Exercise: Create Your Own Transformer (15m)

Take time for students to build their own Transformer emulating `StandardScaler` from Scikit-Learn. Take some time walking through the testing code that was already written.
