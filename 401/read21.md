# Django Models

## Using Models

Models are Python objects that manage data in a Django application.

Models are usually defined in an application's models.py file.

example model

```py
from django.db import models
from django.urls import reverse

class MyModelName(models.Model):
    """A typical class defining a model, derived from the Model class."""

    # Fields
    my_field_name = models.CharField(max_length=20, help_text='Enter field documentation')
    # …

    # Metadata
    class Meta:
        ordering = ['-my_field_name']

    # Methods
    def get_absolute_url(self):
        """Returns the URL to access a particular instance of MyModelName."""
        return reverse('model-detail-view', args=[str(self.id)])

    def __str__(self):
        """String for representing the MyModelName object (in Admin site etc.)."""
        return self.my_field_name
```

A model can have an arbitrary number of fields, which represent a column of data. 


Common Field Types

- CharField
- TextField
- IntegerField
- DateField
- EmailField
- FileField
- AutoField
- ForeignKey
- ManyToManyField

## Admin

The admin application allows you to build an area of your site that you can use to view and modify records.

You can start this by registering your desired models and creating a superuser

## Things I want to learn more about

Django framework and how to build awesome websites.