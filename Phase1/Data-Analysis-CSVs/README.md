# Data Analysis with CSVs

This session is students' first full, real-ish analysis with a raw data file. It goes through loading the file, cleaning it, analyzing it, and visualizing it.

Materials:
- [Jupyter Notebook: Data Analysis with CSVs](DataAnalysis-CSV.ipynb)

## Learning Goals

Perform a complete data analysis by...

- Creating a Python data structure from a .csv file
- Exploring and cleaning the data 
- Conducting descriptive analysis
- Visualizing the results

## Lesson Plan - 1 hour 15 minutes

### Introduction (5 minutes)

Motivate as their first end-to-end analysis with raw data

### Load the CSV (10 minutes)

Work first in the terminal, showcasing where the file is and how to capture the path, then saving that in the notebook as a string. Show also that you can explore the csv file directly inside the terminal.

Then move to the notebook for the rest of the lecture, opening the file both without and with the `csv` module and describing the `with open` syntax (you might consider adding a part comparing to what you would do without the `with` clause, as the differences between those syntaxes often confuse students).

### Data Prep (25 minutes)

Two data cleaning steps: cleaning the service size to be recognized as numeric, and cleaning the dates to access the month and year.

The first is set up so that you walk through the steps as the group, then the second you can use as an activity, sending students into breakout rooms for 5-10 minutes to work on the task before coming back together and showcasing a solution.

### Data Analysis (30 minutes)

Another area for activities! Here you can also split the group into breakout rooms to work on answering these questions for 10-15 minutes, then regrouping to review answers. Make sure to run the answer to Question 4 before proceeding to Data Viz.

### Data Viz (5 minutes)

Follows from Question 4, need to run the answer for that for the viz cell to run.

## Extras

Level Up: Counter
Level Up: datetime
