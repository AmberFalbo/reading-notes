# 401 Class-29: Django Custom User
[Back to 401 Index](401-index.md)<br>

# Readings <br> 

## [**Django Custum User Model**](https://learndjango.com/tutorials/django-custom-user-model) <br>
### **Django Best Practices: Custom User Model**
 Basic Setup steps...

**AbstractUser vs AbstractBaseUser** <br>
There are two modern ways to create a custom user model in Django: AbstractUser and AbstractBaseUser. In both cases we can subclass them to extend existing functionality however AbstractBaseUser requires much, much more work. Seriously, don't mess with it unless you really know what you're doing.

**Custom User Model**
Creating our initial custom user model requires four steps:

- update config/settings.py
- create a new CustomUser model
- create new UserCreation and UserChangeForm
- update the admin

In settings.py we'll add the accounts app and use the AUTH_USER_MODEL config to tell Django to use our new custom user model in place of the built-in User model. We'll call our custom user model CustomUser.

**THEN**

Within INSTALLED_APPS add accounts at the bottom. Then at the bottom of the entire file, add the AUTH_USER_MODEL config.

```
# config/settings.py
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'accounts', # new
]
...
AUTH_USER_MODEL = 'accounts.CustomUser' # new
```
Now update accounts/models.py with a new User model which we'll call CustomUser.

```
# accounts/models.py
from django.contrib.auth.models import AbstractUser
from django.db import models

class CustomUser(AbstractUser):
    pass
    # add additional fields in here

    def __str__(self):
        return self.username
```
We need new versions of two form methods that receive heavy use working with users. Stop the local server with Control+c and create a new file in the accounts app called forms.py.

```
(accounts) $ touch accounts/forms.py
```

## [**DjangoX GitHub LINK**](https://github.com/wsvincent/djangox)  <br>



# Videos <br>

## [**Creating a Custom User Model**](https://www.youtube.com/watch?v=eCeRC7E8Z7Y&t=59s&ab_channel=CodingWithMitch)  <br>

- Really great walk through of how to make a custom user model

## [**Abstract User, User Profile and Signals in Django**](https://www.youtube.com/watch?v=EudKs1HPUfE&ab_channel=DjangoLessons)  <br>

- Great Tutorial, straight forward.

# Bookmark

## [**Substituting a custom User model**](https://docs.djangoproject.com/en/3.0/topics/auth/customizing/#auth-custom-user)  <br>

The authentication that comes with Django is good enough for most common cases, but you may have needs not met by the out-of-the-box defaults. Customizing authentication in your projects requires understanding what points of the provided system are extensible or replaceable. This document provides details about how the auth system can be customized.



[Back to 401 Index](401-index.md)