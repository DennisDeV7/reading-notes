# API Deployment

## Django Settings

[djangostars.com](https://djangostars.com/blog/configuring-django-settings-best-practices/)

It is important to have the same settings as a team when creating projects and deploying them to live servers. The author has suggested layouts for the settings.py file when deploying an api to a live server.

settings.py

```py
ALLOWED_HOSTS = ['example.com']
DEBUG = False
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'production_db',
        'USER': 'user',
        'PASSWORD': 'password',
        'HOST': 'db.example.com',
        'PORT': '5432',
        'OPTIONS': {
            'sslmode': 'require'
        }
    }
}

...

from .settings_local import *
```

settings_local.py

```py
ALLOWED_HOSTS = ['localhost']
DEBUG = True
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'local_db',
        'HOST': '127.0.0.1',
        'PORT': '5432',
    }
}
```

## SSH

SSH or secure shell is a secure way to connect to a server or different computer. On Linux and Mac it can be done by simply typing `ssh {user}@{host}` an example is `ssh pi@raspberrypi.local`

Secure shells work by encrypting and hashing data

There are three ways they encrypt data:

- Symmetric: a secret key is used for both encryption and decryption
- Asymmetric: a different key is used for encryption and decryption
- Hashing: a cryptograph that is never meant to be decrypted

## Things I want to learn more about