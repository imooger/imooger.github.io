---
layout: page
title: Set Dtypes
subtitle: dtypes
menubar: docs_menu
toc: true
show_sidebar: false
redirect_from:
    - /page-without-hero/
---


# Configs.set_dtypes

---

<!-- #### Configs`.get_theme`(current=False) -->

##### Configs<span style="color:purple">.set_dtypes</span>( _<span style="color:grey">dataframe</span>_, _dtypes_dict=<span style="color:grey">None</span>_ )

<!-- To view all available themes, execute the following code:





current : _bool, default False_ -->



<div style="display: flex; justify-content: left; margin-left: 50px;">
    <div>
        <p>
        This function sets data types for variables in the provided DataFrame.
        </p>

        <p><b>Parameters :</b></p>
        <ul>
            <li><b>
            dataframe :
            </b>
            <b><i>
            pandas df
            </i></b></li>
            <p>
            The DataFrame for which data types are to be set.
            </p>
            <li><b>
            dtypes_dict :
            </b>
            <b><i>
            dict or str, optional
            </i></b></li>
            <p>
            A dictionary containing variable names
      and their corresponding data types. If <span style="color:red">'reset'</span>, resets data types to their
      original values obtained from ix.Configs.get_dtypes(). If <span style="color:red">None</span> (default),
      data types are determined automatically using ix.Configs.get_dtypes().
            </p>
        </ul>
        <p><b>Returns:</b></p>
        <ul>
            <li><b>
            str :
            </b>
            <b><i>

            </i></b></li>
            <p>
            A confirmation message indicating the operation is completed.
            </p>
            <p>

            </p>
        </ul>
    </div>
</div>


##### Examples :

The recommended approach is to copy the dictionary obtained from the get_dtypes function and paste it into this function. Then, make necessary edits to the variables based on your requirements.

By following this method, you can efficiently assign appropriate data types to the variables in your DataFrame, ensuring accurate data representation for subsequent analyses.

```python
# To set data types for variables in the Titanic dataset based on a custom dictionary:

>>> ix.Configs.set_dtypes(titanic,
    ...     dtypes_dict = {
    ...         'PassengerId': 'continuous',
    ...         'Survived': 'categorical',
    ...         'Pclass': 'categorical',
    ...         'Name': 'text',
    ...         'Sex': 'categorical',
    ...         'Age': 'continuous',
    ...         'SibSp': 'categorical',
    ...         'Parch': 'categorical',
    ...         'Ticket': 'text',
    ...         'Fare': 'continuous',
    ...         'Cabin': 'text',
    ...         'Embarked': 'categorical'
    ...     })
...
'done'
```


When dtypes_dict is set to ‘reset’, it triggers the resetting of the data types cache to its initial state, effectively reverting the values to those initially retrieved by the get_dtypes function.

```python
# To reset data types to their original values:
>>> ix.Configs.set_dtypes(titanic, dtypes_dict='reset')
...
'done'
```


When setting dtypes_dict to None (default), the function instructs to determine the data types automatically using the get_dtypes function, which executes automatically upon initializing a new dataframe for internal purposes only. This action will not reset the values to original. To reset the values, use dtypes_dict=’reset’ instead!

```python
# To determine data types automatically:
>>> ix.Configs.set_dtypes(titanic)
...
'done'

```













{% include notification.html
message="TIP:
Setting dtypes inside the ADIX environment will NOT change the data types of the pandas dataframe. They are used internally for a more precise description of the variables."
status="is-warning"
icon="fas fa-rocket"
%}

## Setting Dtypes

### set_dtypes(df, dtypes_dict)

The recommended approach is to copy the dictionary obtained from the get_dtypes function and paste it into this function. Then, make necessary edits to the variables based on your requirements.

By following this method, you can efficiently assign appropriate data types to the variables in your DataFrame, ensuring accurate data representation for subsequent analyses.

```python
# setting the dtypes based on the dtypes_dict
ix.Configs.set_dtypes(titanic,
    dtypes_dict = {
     'PassengerId': 'continuous',
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
     'Embarked': 'categorical'
     })
```

'done'


### set_dtypes(df, dtypes_dict='reset')

When dtypes_dict is set to 'reset', it triggers the resetting of the data types cache to its initial state, effectively reverting the values to those initially retrieved by the get_dtypes function.

```python
# Reset dtype values to their initial configurations retrieved from the get_dtypes function.
ix.Configs.set_dtypes(titanic, dtypes_dict='reset')
```
'done'

### set_dtypes(df, dtypes_dict=None)

When setting dtypes_dict to None (default), the function instructs to determine the data types automatically using the get_dtypes function, which executes automatically upon initializing a new dataframe for internal purposes only. This action will not reset the values to original. To reset the values, use dtypes_dict='reset' instead!

```python
# initializing df with get_dtypes values
ix.Configs.set_dtypes(titanic)
```
'done'
