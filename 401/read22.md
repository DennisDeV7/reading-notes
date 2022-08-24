# Django CRUD

## Django Forms

An HTML Form "is a group of one or more fields on a webpage, which can be used to collect informatino from users for submission to a server" [developer.org](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Forms)

The main steps Django handles forms:

1. Display default form
2. Receive data from a submit
3. Clean and validate data
4. If data is invalid, display form again and repopulate information
5. If data is valid, perform the actions
6. When finished, redirect to another page

Example form creation, made in a forms.py file:

```py
from django import forms

class RenewBookForm(forms.Form):
    renewal_date = forms.DateField(help_text="Enter a date between now and 4 weeks (default 3).")
```

There are many form fields to help format the form to see them all visit, [devleoper.org](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Forms#renew-book_form_using_a_form_and_function_view)

## Things I want to learn more about

I want to learn more about how to create forms in Django!