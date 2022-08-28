# Djand REST and Docker

## Docker

Docker is a form of virtualization that allows the user to isolate projects and all of its environmental factors such as language, packages, and databases

Docker is at its root, Linux containers. Linux containers are a virtual machine that enables the user to work on an entire computer system virtually.

Docker can be downloaded from their website at [docker.com](https://www.docker.com/get-started/)

An additional package needs to be installed for Linux users by running: `sudo pip install docker-compose`

### Docker commands

- `docker run program-name`
- `docker info`
- `docker image ls`
- `docker container ls -la`

## Django REST

Set up a new Django project and app first

Create project:  `django-admin startproject project-name .`

Create app: `python manage.py startapp app-name`

Add app to setting.py file

Create a Model

Migrate

    - `python manage.py makemigrations app-name`
    - `python manage.py migrate`

Create Superuser: `python manage.py createsuperuser`

Serialize: add serializer.py file

Create read-write endpoint and read-write-delete endpoint

Update Views, URLs, and Templates


## Things I want to learn more about
