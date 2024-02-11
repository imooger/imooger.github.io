---
layout: page
title: Get dtypes
subtitle: dtpes
menubar: docs_menu
toc: true
show_sidebar: false
---

# Configs.get_dtypes

---

<!-- #### Configs`.get_theme`(current=False) -->

##### Configs<span style="color:purple">.get_dtypes</span>( _<span style="color:grey">dataframe</span>_ )

<!-- To view all available themes, execute the following code:





current : _bool, default False_ -->



<div style="display: flex; justify-content: left; margin-left: 50px;">
    <div>
        <p>
        This function gets suggested data types for each variable in the provided DataFrame.
        </p>

        <p><b>Parameters:</b></p>
        <ul>
            <li><b>
            dataframe:
            </b>
            <b><i>
            pandas df
            </i></b></li>
            <p>
            The DataFrame for which data types are to be determined.
            </p>
        </ul>
        <p><b>Returns:</b></p>
        <ul>
            <li><b>
            dict:
            </b>
            <b><i>

            </i></b></li>
            <p>
            A dictionary containing suggested data types for each variable.
      Keys are variable names, and values are the suggested data types.
            </p>
            <p>

            </p>
        </ul>
    </div>
</div>


##### Examples


```python
#To get suggested data types for variables in the Titanic dataset:
>>> ix.Configs.get_dtypes(titanic)
...

{'PassengerId': 'continuous',
 'Survived': 'categorical',
 'Pclass': 'categorical',
 'Name': 'text',
 'Sex': 'categorical',
 'Age': 'continuous',
 'SibSp': 'categorical',
 'Parch': 'categorical',
 'Ticket': 'text',
 'Fare': 'continuous',
 'Cabin': 'text',
 'Embarked': 'categorical'}
```















{% include notification.html
message="TIP:
Setting dtypes inside the ADIX environment will NOT change the data types of the pandas dataframe. They are used internally for a more precise description of the variables."
status="is-warning"
icon="fas fa-rocket"
%}
<!--

## Getting Dtypes

### get_dtype(dataframe)

The function returns a dictionary containing suggested data types for each variable based on an automated analysis of the dataset's characteristics and values.

```python
# Returns a dictionary of suggested dtypes for each variable
ix.Configs.get_dtypes(titanic)
```
```python
# output
{'PassengerId': 'continuous',
 'Survived': 'categorical',
 'Pclass': 'categorical',
 'Name': 'text',
 'Sex': 'categorical',
 'Age': 'continuous',
 'SibSp': 'categorical',
 'Parch': 'categorical',
 'Ticket': 'text',
 'Fare': 'continuous',
 'Cabin': 'text',
 'Embarked': 'categorical'}
 ``` -->
