---
layout: page
title: Add Themes
subtitle: Themes
menubar: docs_menu
toc: true
show_sidebar: false
---

# Configs.add_theme

---

<!-- #### Configs`.get_theme`(current=False) -->

##### Configs<span style="color:purple">.add_theme</span>( _theme_name=<span style="color:grey"> str</span>_, _theme_values=<span style="color:grey"> dict</span>_ )

<!-- To view all available themes, execute the following code:





current : _bool, default False_ -->



<div style="display: flex; justify-content: left; margin-left: 50px;">
    <div>
        <p>
        This function adds a new custom theme for visualization.
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
            The name of the custom theme to be added.
            </p>
            <li><b>
            theme_values :
            </b>
            <b><i>
            dict
            </i></b></li>
            <p>
            A dictionary containing the custom theme values.
      The dictionary should include key-value pairs representing the customizable
      elements and their corresponding color values.

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
# add your custom theme
>>> custom_theme = {
    'dash_donuts_color': '#a3b18a',
    'mini_hist_color': '#a3b18a',
    'hist_color': '#a3b18a',

    'label_color':'#bc6c25',
    'dash_bars_color': '#bc6c25',
    'hist_kde_color': '#bc6c25',
    'bar_color': 'light:#bc6c25',
    'hover_color': '#bc6c25',

    'dash_bars_text_color': '#525252',
    'bar_font_color': '#525252',
}

>>> ix.Configs.add_theme('CustomTheme', custom_theme)                 

```










## Adding themes

Unleash your creativity by choosing any color for the list of attributes inside the ADIX environment. Refer to the image below for reference:

![Atributes avaliable](/img/add_theme.jpg)

### add_theme('theme_name',dict)
The function accepts two arguments:

- Name of the Theme as a string.
- Dictionary containing all values to change.






```python
# add your custom theme
ix.Configs.add_theme('Ocean',                  
{
    'dash_donuts_color': '#a3b18a',
    'mini_hist_color': '#a3b18a',
    'hist_color': '#a3b18a',

    'label_color':'#bc6c25',
    'dash_bars_color': '#bc6c25',
    'hist_kde_color': '#bc6c25',
    'bar_color': 'light:#bc6c25',
    'hover_color': '#bc6c25',

    'dash_bars_text_color': '#525252',
    'bar_font_color': '#525252',
})
```


## How to add your custom color palette

To add your custom color palette, follow these steps:

- `**Disable Cache** - important!!!`
- **Retrieve Current Theme Values:** Use the get_theme(current=True) function to obtain the current theme's values.
- **Name Your Theme:** Choose a name for your custom theme.
- **Copy and Paste Values:** Copy the values from the output of the get_theme(current=True) function into a dictionary. Replace the color values with your preferred colors.
- **Check Theme Availability:** Verify if your custom theme appears in the list of available themes.
- **Set Your New Theme:** Use the set_theme('your_theme_name') function to apply your custom theme.
- `**Enable Cache** - important!!!`

By following these steps, you can seamlessly integrate your custom color palette into your application or environment.

{% include notification.html
message="TIP:
The simplest method is to invoke get_theme(current=True), which retrieves all the values. Then, you can effortlessly copy them into the dictionary, substituting them with your preferred color choices (as hexadecimal values—utilize your preferred color application).

After completing customization, execute the function. Upon omitting the current=True parameter in get_themes, you'll observe that your theme has been successfully incorporated.

Finally, execute set_theme, and presto! Your color theme is now established."
status="is-warning"
icon="fas fa-rocket"
%}
![Atributes avaliable](/img/new_theme.png)
