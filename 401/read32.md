# Permissions & Postgresql

## Permissions

A permission is a script of code which determines if the user has access to the api or data.

In a REST framework permissions are typically determined before the main program runs. When it comes to writing the code, this is handled with exceptions. Some exceptions you can expect to use include:

- PermissionDenied
- NotAuthenticated

Some errors you can expect to see if permission is denied when running your code

- 403: Forbidden
- 401: Unauthorized

The permissions are typically set in a permissions.py file

for an example see: [django-rest-framework](https://github.com/encode/django-rest-framework/blob/master/rest_framework/permissions.py)

## Things I want to learn more about