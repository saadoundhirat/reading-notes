# About Django Custom User Model

- There is a far easier yet still powerful approach to starting off new Django projects with a custom user model which I'll demonstrate here.

## Setup

- To start, create a new Django project from the command line. We need to do several things:
- create and navigate into a dedicated directory called accounts for our code
- install Django
- make a new Django project called config
- make a new app accounts
- start the local web server

![](https://www.geekinsta.com/content/images/2021/03/create-custom-django-user-model.jpg)

## Here are the commands to run

```
$ cd ~/Desktop
$ mkdir accounts && cd accounts
$ pipenv install django~=3.1.0
$ pipenv shell
(accounts) $ django-admin.py startproject config .
(accounts) $ python manage.py startapp accounts
(accounts) $ python manage.py runserver
```

## AbstractUser vs AbstractBaseUser

- There are two modern ways to create a custom user model in Django: AbstractUser and AbstractBaseUser. In both cases we can subclass them to extend existing functionality however AbstractBaseUser requires much, much more work.

## Custom User Model

- Creating our initial custom user model requires four steps:

- update config/settings.py
- create a new CustomUser model
- create new UserCreation and UserChangeForm
- update the admin
- In settings. py we'll add the accounts app and use the AUTH_USER_MODEL config to tell Django to use our new custom user model in place of the built-in User model. We'll call     our custom user model CustomUser.

- Within INSTALLED_APPS add accounts at the bottom. Then at the bottom of the entire file, add the AUTH_USER_MODEL config.
