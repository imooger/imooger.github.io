---
layout: page
title: Set Themes
subtitle: Themes
menubar: docs_menu
toc: false
show_sidebar: false
redirect_from:
  - /page-3/
---

# Configs.set_theme

---

##### Configs<span style="color:purple">.set_theme</span>( _theme_name:<span style="color:grey"> str</span>_ )

<div style="display: flex; justify-content: left; margin-left: 50px;">
    <div>
        <p>
        This function sets a new theme for visualization.
        </p>

        <p><b>Parameters:</b></p>
        <ul>
            <li><b>
            theme_name :
            </b>
            <b><i>
            str
            </i></b></li>
            <p>
            The name of the theme to be set. Use a theme name obtained
      from Configs.get_theme().
            </p>
        </ul>
        <p><b>Returns:</b></p>
        <ul>
            <li><b>
            None
            </b>
            <b><i>

            </i></b></li>
            <p>

            </p>
            <p>

            </p>
        </ul>
    </div>
</div>

##### Examples


```python
#To set a new theme:
>>> ix.Configs.set_theme('PEACH')
```



<!--
### set_theme('theme_name')

To set a new theme, first call `.get_theme()` to see all available themes and use the name of the theme as an argument for the function.

```python
# set a new theme
ix.Configs.set_theme('PEACH')
``` -->
