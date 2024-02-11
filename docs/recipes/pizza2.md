---
layout: recipe
title: Recipes
subtitle: Recipes
menubar: docs_menu
show_sidebar: false
toc: true
---

## Recipe Page

You can make a single page using the recipe layout, or you can use it in your blog by specifying the `layout: recipe` instead of post.

You probably want to hide the sidebar, so the recipe takes up the whole page width. If you add any additional content to the page it will appear below the recipe details.

Create a list in the front matter for the ingredients, then the method steps and it will automatically be added to the page.

The front matter will also be added to the page as schema data that is used by search engines.

Please see the below example for all of the schema options available.

```yaml
layout: recipe
title: Best pizza
subtitle: pizza pizza
author: imooger
date: 2024-14-02
show_sidebar: false
image: /img/pizza.jpg
hero_image: /img/pizza.jpg

Sugo:
    - basil
    - 440g mutti polpa tomatoes
    - 1 tea spoons salt
    - 2 tea spoons olive oil
Poolish:
    - 300ml water
    - 300gr. flour
    - 5gr. dry yeast
    - 5gr. honey.

    - 24 hours in the fridge

Rest of the dough:
    - All poolish
    - 200ml. water
    - 475gr. 00 flour
    - 15 gr. salt
    - 15gr. olive oil.

method:
    - day before mix the poolish and set it sit it the fridge for 24 hours
    - second day put all the poolish into the kitchen aid, add water and run on speed 2
    - after poolish is blended with water add flower and salt and mix for 10 -15 minutes until the dough starts separating completely from the bowl
    - let it in the mixer for 15 minutes
    - run on high speed for 10 seconds and transfer the dough onthe kitchen counter and form a firm ball. Let it rest covered for 1 hour
    - devide the dough into 5 pieces and shape small balls, cover them and rest for 1 hour, prepare other ingredients (preheat oven on max)
    - form pizzas and bake them in a pizza oven or kitchen oven
prep_time: PT0H10M
cook_time: PT1H
total_time: PT5H10M
keywords: recipe,cooking
recipe_yield: 5
recipe_category: Main course
recipe_cuisine: Italian
calories: 500 calories
```

[View example Recipe page](/bulma-clean-theme/example-recipe)
