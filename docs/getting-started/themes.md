---
layout: page
title: Themes
subtitle: Getting Started
menubar: docs_menu
toc: true
show_sidebar: false
---


## Getting themes

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

![Atributes avaliable](/img/get_current_theme.png)

## Setting themes

### set_theme('theme_name')

To set a new theme, first call `.get_theme()` to see all available themes and use the name of the theme as an argument for the function.

```python
# set a new theme
ix.Configs.set_theme('PEACH')
```


## Adding themes

Here your creativity starts, you can choose any color for the list of attributes inside the ADIX environment. See the image below for reference:

![Atributes avaliable](/img/add_theme.jpg)

### add_theme('theme_name',dict)
the function accepts two arguments:
- name of the Theme as a str
- dict of all values to change






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

- `Disable Cache - important!!!`
- Retrieve Current Theme Values: Use the get_theme(current=True) function to obtain the current theme's values.
- Name Your Theme: Choose a name for your custom theme.
- Copy and Paste Values: Copy the values from the output of the get_theme(current=True) function into a dictionary. Replace the color values with your preferred colors.
- Check Theme Availability: Verify if your custom theme appears in the list of available themes.
- Set Your New Theme: Use the set_theme('your_theme_name') function to apply your custom theme.
- `Enable Cache - important!!!`
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
