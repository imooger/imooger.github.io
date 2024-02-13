---
layout: page
title: Get themes
subtitle: Themes
menubar: docs_menu
toc: false
show_sidebar: false
redirect_from:
  - /page-5/
---

# Configs.get_theme

---

<!-- #### Configs`.get_theme`(current=False) -->

##### Configs<span style="color:purple">.get_theme</span>( _current=<span style="color:grey">False</span>_ )

<!-- To view all available themes, execute the following code:





current : _bool, default False_ -->



<div style="display: flex; justify-content: left; margin-left: 50px;">
    <div>
        <p>
        This function returns the list of avaliable themes or dictionary detailing the customizable elements.
        </p>

        <p><b>Parameters:</b></p>
        <ul>
            <li><b>
            current :
            </b>
            <b><i>
            bool, default False
            </i></b></li>
            <p>
            If True, returns details about the current theme,
            including customizable elements and their corresponding color values.
            If False (default), returns a list of available themes.
            </p>
        </ul>
        <p><b>Returns:</b></p>
        <ul>
            <li><b>
            list or dict:
            </b>
            <b><i>

            </i></b></li>
            <p>
            list or dict: If current is False, returns a list of available themes.
            If current is True, returns a dictionary detailing the customizable elements
            and their corresponding color values within the current theme.
            </p>
            <p>

            </p>
        </ul>
    </div>
</div>


##### Examples


```python
#To get a list of available themes:
>>> ix.Configs.get_theme()
...
['Theme1', 'Theme2', 'Theme3']
```

```python
#To get details about the current theme:
>>> ix.Configs.get_theme(current=True)
...
{'dash_donuts_color': '#FFCBA5',
 'dash_bars_color': '#FF9899',
 'dash_bars_text_color': '#525252',
 'label_color': '#FF9899',
 'mini_hist_color': '#FFCBA5',
 'hist_color': '#FFCBA5',
 'hist_kde_color': '#FF9899',
 'bar_color': 'light:#FF9899',
 'bar_font_color': '#525252',
 'hover_color': '#FF9899'}
```




<!-- ## Getting themes

### get_theme()

To view all available themes, execute the following code:

```python
# return a list of all avaliable Themes
ix.Configs.get_theme()
```

### get_theme(current=True)

If `current` is set to `True`,  this function returns a dictionary detailing the customizable elements along with their corresponding color values within the current theme.

```python
# returns all customizable values
ix.Configs.get_theme(current=True)
```

![Atributes avaliable](/img/get_current_theme.png) -->
