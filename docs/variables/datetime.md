---
layout: page
title: DateTime
subtitle: variables
menubar: docs_menu
show_sidebar: false
toc: true
redirect_from:
    - /page-with-notification/
---

## _main

Variables can be accessed either as part of a dataset, by their dtype, or individually.

```python

# To access the entire dataset:
ix.eda(ufo)

# Alternatively, to access specific variables by their dtype:
ix.eda(ufo, val='datetime')

# Alternatively, to access the 'Pclass' variable individually:
ix.eda(ufo, 'Time')
```

![Pairwise sample](/img/time_main.png)

Statistical Information on the Variable

|-----------------------|-----------------------------|
| VALID | _Percentage of valid observations in the variable_ |
| MISSING | _Percentage of missing observations in the variable_ |
| UNIQUE | _Percentage of unique observations in the variable_ |

The mini bar chart shows the variable value distribution (it uses log-scale making variations more apparent)


## Stats



![Pairwise sample](/img/time_stats.png)

The "Stats" tab provides users with basic set of statistics

Additionally, the tab includes a histogram paired with a Kernel Density Estimation (KDE) plot, providing a comprehensive visualization of the variable's distribution.

|-----------------------|-----------------------------|
| VALUES | Number of valid values in the variable |
| MISSING | Number of missing observations in the variable |
| DISTINCT | Number of unique observations in the variable |
| | |
| MEMORY | Memory size of the variable |
| DTYPE | Pandas datatype |
| | |
| MAX | Last chronological value |
| MIN | First chronological value |


## Value Table

![Pairwise sample](/img/cat_val.png)

The value table organizes data by sorting values according to their frequency of occurrence, enabling quick identification of the most common values (up to 10) within the dataset.

And additionaly displaying the top three and bottom three values for quick reference and analysis.
