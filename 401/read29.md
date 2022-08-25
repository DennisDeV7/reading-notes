# Django Custom User

Django comes with a user model for authentication. However, making an application most likely requires a custom user model.

The Django documentation offers a way to make a custom user model at [djangoproject.com](https://docs.djangoproject.com/en/4.0/topics/auth/customizing/#a-full-example). However, according to [learndjango.com](https://learndjango.com/tutorials/django-custom-user-model), the industry tends to use a different approach to making custom user models.

Industry steps to making a custom user model:

1. Setup Django project
    - In the desired directory of the new project, create and activate a virtual environment
    - Install django: `pip install django`
    - Create project: `django-admin startproject project_name .`
    - Create an app: `python manage.py startapp app_name`
    - Test to see server runs: `python manage.py runserver`

Do not migrate yet!!

2. Create custom user model
    - In the project folder, add the app and user model to the settings file:
    this will be inside `INSTALLED_APPS` and `AUTH_USER_MODEL` respectively.
    example:

    ```txt
      # django_project/settings.py
      INSTALLED_APPS = [
        "django.contrib.admin",
        "django.contrib.auth",
        "django.contrib.contenttypes",
        "django.contrib.sessions",
        "django.contrib.messages",
        "django.contrib.staticfiles",
        "accounts",  # new
      ]
      ...
      AUTH_USER_MODEL = "accounts.CustomUser"  # new
    ```

    - Create new class in models.py for custom user usint `AbstractUser`
    - Create a form
    - Update admin.py

3. Migrate
    - `python manage.py makemigrations app_name`
    - `python manage.py migrate`

4. Create superuser
    - `python manage.py createsuperuser`

5. Update Views, URLs, and Templates

## DjangoX

DjangoX is an open source project initiated by William Vincent to provide a starting framework for a Django project. To my understaning, you can clone his repository, install the packages, and then modify the content to meet your needs.

Found at [wsvincent](https://github.com/wsvincent/djangox)

steps:

1. clone repo: `git clone https://github.com/wsvincent/djangox.git`
2. Activate virtual environment
3. Install requirements: `pip install -r requirements.txt`
4. Migrate: `python manage.py migrate`
5. Create super user: `python manage.py createsuperuser`
6. Test server: `python manage.py runserver`

## Things I want to learn more about
