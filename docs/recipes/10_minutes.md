---
layout: page
title: Get started
subtitle: 10 minutes to ADIX
menubar: docs_menu
show_sidebar: false
toc: true
---

# Installation
The best way to install **adix** (other than from source) is to use pip:
```
pip install adix
```

**adix is still under development** If you encounter any data, compatibility, or installation issues, please don't hesitate to reach out!


# Quick start
The system is designed for rapid visualization of target values and dataset, facilitating quick analysis of target characteristics with just one function `ix.eda()`. Similar to pandas' df.describe() function, it provides extended analysis capabilities, accommodating time-series and text data for comprehensive insights.

```python
import adix as ix
from adix.datasets import load_dataset

titanic = load_dataset('titanic')
```

### 10 minutes to **adix**


#### 1. Rendering the whole dataframe
```python
ix.eda(titanic)
```
- using _forest color theme_
![Pairwise sample](/img/all_var.gif)

---
#### 2. Accesing variables of specific dtype
Render the DataFrame containing only categorical variables.

```python
ix.eda(titanic,val='categorical')
```
---
#### 3. Accesing individual variables
```python
ix.eda(titanic,'Age')
```
- using _forest color theme_

![Pairwise sample](/img/one_var.gif)

---
#### 4. Pandas .loc & .iloc
An easy way to render only a part of the DataFrame you are interested in.

```python
ix.eda(titanic.loc[:10:2,['Age','Pclass','Fare'])
```
---

#### 5. Changing theme colors
```python
ix.Configs.get_theme()
...
ix.Configs.set_theme('FOREST')
```
<div align="center"><img width="100%" src="/img/change_c.png"/></div>

---

#### 6. Bivariate relationships:  numerical & numerical
```python
ix.eda(titanic,'Age','Fare')

```
<div align="center"><img width="100%" src="/img/c_c.png"/></div>

---

#### 7. Bivariate relationships:  categorical & numerical
```python
ix.eda(titanic,'Sex','Age')


```
<div align="center"><img width="100%" src="/img/cat_c.png"/></div>

---

#### 8. Bivariate relationships:  categorical & categorical
```python
ix.eda(titanic,'Sex','Survived')

```
<div align="center"><img width="100%" src="/img/cat_cat.png"/></div>
