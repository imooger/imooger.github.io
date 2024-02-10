---
layout: page
title: Configuration
subtitle: Getting Started
menubar: docs_menu
show_sidebar: false
toc: true
---

## General Configuration

Recognizing that data preparation consumes significant time, the primary focus of ADIX is to streamline the analysis process for users. Consequently, extensive configuration options are intentionally kept to a minimum to avoid impeding the workflow.

However, users still have the flexibility to customize certain aspects, such as the color theme palette. Furthermore, options to disable the cache or the dashboard panel are available for those seeking additional control over their experience.

## Themes

Easily adjust the visualization theme to match your preferences. You can either select from pre-prepared theme plates by calling two functions `.get_theme()` & `.set_theme()` or customize ADIX with your own color palettes. Check out the documentation/Themes section for detailed instructions:

```python
ix.Configs.get_theme()
# Explore available themes and set your preferred one
ix.Configs.set_theme('FOREST')
```

![Theme Change](/img/change_c.png)

## Cache

ADIX employs caching as its default mechanism for a simple reason: it significantly accelerates the reloading of dataframes and visualizations, up to `10x times` faster! The system is intelligent enough to detect changes in dataframes and adapt accordingly. It's highly recommended to keep caching active primarily for performance reasons. However, you can disable it easily by entering:

```python
# Disable cache
ix.Configs.use_eda_cache = false
```

## Dashboard

The Dashboard serves as a swift initial insight into the dataset. By default, it appears when loading the entire dataset and is disabled when accessing individual variables or employing bivariate relations. As previously mentioned, since the entire dataframe is cached, attempting to deactivate it for time-saving purposes is computationally inefficient. Nonetheless, you can still disable it by entering:

```python
# Disable dashboard
ix.eda(df,wrap=False)
```
