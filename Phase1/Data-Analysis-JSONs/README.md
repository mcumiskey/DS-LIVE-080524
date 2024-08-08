# Data Analysis with JSONs

Materials:
- [Jupyter Notebook: Data Analysis with JSONs](DataAnalysis-JSON.ipynb)

## Learning Goals

Perform a complete data analysis by...
- Loading and exploring a .json file in Python
- Creating a clean data structure from a .json file
- Conducting descriptive analysis
- Visualizing the results

## Lesson Plan - 1 hour 15 minutes

### Introduction (5 minutes)

Spend a few minutes highlighting the importance of being able to deal with several different file types. JSONs have highly articulated structures, so the lessons from before on accessing data from highly nested structures will be relevant.

### Exploring JSON Schemas - Spotify Data (20 minutes)

Walk through the spotify object, moving level by level and discussing how to move between pieces. Stress the importance of being aware of data types at each level.

### Move to Plant Data and Explore Plant Families (20 minutes)

Read in the next dataset, of plants, and walk through the Plant Families section as a group. Note that this section currently uses a `defaultdict` from the `collections` module - you may need to spend extra time discussing why that's used here and how it's different from a base python dictionary.

### Explore Plant Synonyms (10 minutes)

Showcase where students can find the sysnonyms data and build the visualization, then let students find the plant with so many synonyms (might move students into breakout rooms for 5 minutes to work in groups).

### Explore Plant Bibliographies (15 minutes)

Showcase what the biliography part of the object looks like, and how to parse out and explore to find "Linnaeus". Then showcase how to find records from a specific book.

Give students 5 minutes (potentially in groups in breakout rooms) to change records within this dictionary.

### Conclusion (5 minutes)

Teaser of `pandas` lessons to come the following day.
