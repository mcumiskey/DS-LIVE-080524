# Pandas DataFrames

The overarching goal here is to introduce students to `pandas` as our go-to way of working with data.

Materials:
- [Jupyter Notebook: Pandas DataFrames](pandas_dataframes.ipynb)

## Learning Goals

- use `pandas` to read in .csv files
- interact with and manipulate Series and DataFrames
- identify and deal with N/A values

## Lesson Plan - 1 hour 30 minutes

### Introduction (5 minutes)

Brief discussion of what `pandas` is and of its importance for us: This library will be one we use from here on out!

### Basic `pandas` Syntax: Methods and Attributes of DataFrames (15 minutes)

This first section uses the small heart dataset to start exploring common df/series methods like `.head()` or `.info()`, attributes like `shape` or `dtypes`, etc. Encourage the bracket-notation (`df['column']`) for grabbing columns of a df since it better handles column names with spaces or other strange characters. This also includes a brief run through of how to calculate simple statistics on columns or dataframes.

### Move to Bigger Data (15 minutes)

Showcase a live, publicly available dataset ([the Austin Animal Center Intakes data](https://data.austintexas.gov/Health-and-Community-Services/Austin-Animal-Center-Intakes/wter-evkm/)), including how to access it using `read_csv` from an API endpoint. Discuss some limitations of endpoints (here, it only lets you access the first 1000 rows by default). 

The version of the data in the `data` folder has been lightly cleaned to facilitate later exploration - namely, the Year column (the only numeric column) has been extracted from the date. This eliminates the need to dig into `.dt` attributes too early, but still allows us to do some numeric exploration later.

From here - after reading in the larger CSV, showcase doing the same methods/attributes from the earlier section on this new dataframe.

### Adding Rows and Columns to DataFrames (10 minutes)

Should point out that this method of adding rows is a bit rocky, but it's because this isn't typically how new data is added, that would typically happen at the database level - but, goes ahead and introduces `.concat`

### Filtering Exercises (15 minutes)

Introduce filtering using `loc` and `iloc`, but the emphasis is definitely on `loc`. Discuss how to set up the conditions that are passed into `loc` statements, the way that square brackets indicates location in a way, and expplain that they need to pass the exact location of columns instead of just column names inside the square brackets. Showcase using multiple conditions to segment down.

There are two exercises here, which can be run as group exercises in breakout rooms, or skipped and students can answer later if you're tight on time.

### Series Methods: `.value_counts()` and `.sort_values()` (10 minutes)

Introduce the power of value counts - a type of groupby before they even learn groupbys! Showcase how the results of a value count are just series objects themselves, so they can be segmented down (easy way to access the top ten of a series). Also showcase `normalize=True` to access percentages instead of whole counts. You might want to note how `.value_counts` does not capture how much of the column is null.

Discuss how sorting can happpen on a series or on a whole dataframe, but they require different arguments depending. Also discuss how sorting on an object column or something non-numeric can be weird (if you still have a non-datetime object column that captures dates, you can showcase how it doesn't magically sort that column correctly, unless it's a date time and it knows to treat the column as a date!)

### Conclusion (5 Mins)

Remind them that `pandas` will be an ultra-important library, and so there will be more lectures exploring more of its functionality.

## Tips

- I (Victor) find it useful to go over some alternative ways of doing the same thing to emphasize that there isn't only one way to do something (in Pandas).
- I usually spend a minute on the link to the Anaconda docs, illustrating that many packages are included with that Python installation (and that others are not).
- The heart dataset is from [kaggle](https://www.kaggle.com/ronitf/heart-disease-uci), and it's worth clicking on this link as not all the column names of the dataset are straightforwardly interpretable.

