# Django Models

**Models:** is the structure of stored data, including the field types and possibly also their maximum size, default values, selection list options, help text for documentation, label text for forms, etc.

Django allows you to define **relationships** that are **one to one** (OneToOneField), **one to many** (ForeignKey) and **many to many** (ManyToManyField).


**The diagram** also shows the relationships between the models, including their multiplicities.

**The multiplicities** are the numbers on the diagram showing the numbers (**maximum** and **minimum**) of each model that may be present in the relationship.

## Fields:
`models.CharField`: means that this field will contain strings of alphanumeric characters.

`max_length=20`: — States that the maximum length of a value in this field is 20 characters.

`help_text='Enter field documentation'`: text that may be displayed in a form to help users understand how the field is used.

The **field name** is used to refer to it in queries and templates. Fields also have a **label**, which is specified using the **verbose_name** argument (with a default value of **None**). If **verbose_name** is not set, the label is created from the field name by replacing any underscores with a space.

## COMMON FIELD ARGUMENTS
The following common arguments can be used when declaring many/most of the different field types:
- **help_text**: Provides a text label for HTML forms.
- **verbose_name**: A human-readable name for the field used in field labels. If not specified, Django will infer the default verbose name from the field name.
- **default**: The default value for the field. This can be a value or a callable object, in which case the object will be called every time a new record is created.
- **null**: If True, Django will store blank values as **NULL** in the database for fields where this is appropriate (a CharField will instead store an empty string). The default is False.

## Metadata
You can declare model-level metadata for your Model by declaring class Meta. One of the most **useful features** of this metadata **is to control the default ordering of records returned when you query the model type**


## Methods
A model can also have methods.

Minimally, in every model you should define the standard Python class method __str__() to return a **human-readable** string for each object. This string is **used** to **represent individual records in the administration site** (and anywhere else you need to refer to a model instance). Often this will return a title or name field from the model.


## Creating a superuser:
`python3 manage.py createsuperuser` use to create the superuser. You will be prompted to enter a **username**, **email address**, and **strong password**.
