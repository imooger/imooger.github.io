---
title: ADIX
subtitle: Making Data Science Fun, One Color at a Time!

layout: page
hero_link: https://pypi.org/project/adix/
hero_link_text: latest release
hero_image: true
callouts: example_callouts
show_sidebar: true
---

![Pairwise sample](/img/main_fade1.gif)
# What is it?
**adix** (Automatic Data Inspection and eXploration) simplifies Exploratory Data Analysis (EDA) with a single command `ix.eda()`. Experience a streamlined approach to uncovering insights, empowering you to focus on your data without distraction.
**Color customization** is at your fingertips, allowing you to tailor your analysis to your exact needs. Explore your data with confidence and efficiency, knowing that **adix** has your back every step of the way.

# Data Insights
The dashboard at the top serves as a dynamic hub, offering a snapshot of critical insights derived from the dataframe. With its intuitive layout, it provides at-a-glance access to key metrics, trends, and patterns, empowering users to make informed decisions swiftly.

![Pairwise sample](/img/dash.gif)

# Quick start
The system is designed for rapid visualization of target values and dataset, facilitating quick analysis of target characteristics with just one function `ix.eda()`. Similar to pandas' df.describe() function, it provides extended analysis capabilities, accommodating time-series and text data for comprehensive insights.

```python
import adix as ix
from adix.datasets import load_dataset

titanic = load_dataset('titanic')
```

# Main Features

- **Customizable Themes**
  - Spruce up the **adix** environment with your own personal touch by playing with color schemes!    
- **Eficient Cache Utilization**
  - Experience faster load times through optimized caching mechanisms, enhancing overall system performance.  
- **Rapid Data Insight**
  - **adix** prioritizes swiftly showcasing crucial data insights, ensuring quick access to important information.  
- **Automatic Type Detection**
  - Detects numerical, categorical, and text features automatically, with the option for manual overrides when
  necessary.
- **Statistically Rich Summary Information:**
  - Unveil the intricate details of your data with a comprehensive summary, encompassing type identification, unique values, missing values, duplicate rows, the most frequent values and more.
  - Delve deeper into numerical data, exploring properties like min-max range, quartiles, average, median, standard deviation, variance, sum, kurtosis, skewness and more.
- **Univariate and Bivariate Statistics Unveiled**
    - Explore univariate and bivariate insights with adix's versatile visualization options. From bar charts to matrices, and box plots, uncover a multitude of ways to interpret and analyze your data effectively.

# Installation
The best way to install **adix** (other than from source) is to use pip:
```
pip install adix
```

**adix is still under development** If you encounter any data, compatibility, or installation issues, please don't hesitate to reach out!





<!-- # Bulma Clean Theme demo website

This website showcases the options for the Bulma Clean theme. The theme is available as a ruby gem or can be used with GitHub pages.

[![Gem Version](https://badge.fury.io/rb/bulma-clean-theme.svg)](https://badge.fury.io/rb/bulma-clean-theme)
![Gem](https://img.shields.io/gem/dt/bulma-clean-theme.svg)
![GitHub Repo stars](https://img.shields.io/github/stars/chrisrhymes/bulma-clean-theme?style=social)

## Ruby Gem

The ruby gem is available on the Ruby Gems website at the following location. [https://rubygems.org/gems/bulma-clean-theme](https://rubygems.org/gems/bulma-clean-theme).

## GitHub Pages

The theme can be used with GitHub Pages by setting the `remote_theme` in your Jekyll sites `_config.yml`

```yml
remote_theme: chrisrhymes/bulma-clean-theme
```

## Documentation

For full instructions, please see the [Documentation](/bulma-clean-theme/docs/)

## Page Layouts

This demo site showcases the available page layout options.

* Sidebar
* Menubar
* Tabs
* Footer
* Hero
* Contents
* Landing Page With Callouts
* Sponsors Page
* Image Gallery
* Recipe Page
* Blog
* Post

## Supported By JetBrains

JetBrains have kindly provided an Open Source licence to aid in the future development of Bulma Clean Theme.

[![JetBrains](img/jetbrains-variant-4.svg)](https://www.jetbrains.com/?from=bulma-clean-theme) -->
