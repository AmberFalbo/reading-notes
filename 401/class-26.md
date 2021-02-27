# 401 Class-26: Intro into Django
[Back to 401 Index](401-index.md)<br>

## [**Getting started with Django**](https://www.djangoproject.com/start/)
- Just the `Intro to Django` section.

### **File Notes for `startproject`**

The *outer* `mysite/` root directory is a container for your project. Its name doesn’t matter to Django; you can rename it to anything you like.

`manage.py:` A command-line utility that lets you interact with this Django project in various ways. You can read all the details about manage.py in django-admin and manage.py.

The *inner* `mysite/` directory is the actual Python package for your project. Its name is the Python package name you’ll need to use to import anything inside it (e.g. mysite.urls).

`mysite/__init__.py`: An empty file that tells Python that this directory should be considered a Python package. If you’re a Python beginner, read more about packages in the official Python docs.

`mysite/settings.py`: Settings/configuration for this Django project. Django settings will tell you all about how settings work.

`mysite/urls.py`: The URL declarations for this Django project; a “table of contents” of your Django-powered site. You can read more about URLs in URL dispatcher.

`mysite/asgi.py`: An entry-point for ASGI-compatible web servers to serve your project. See How to deploy with ASGI for more details.

`mysite/wsgi.py`: An entry-point for WSGI-compatible web servers to serve your project. See How to deploy with WSGI for more details.


## [**How Django Works Behind the Scenes**](https://wsvincent.com/how-django-works-behind-the-scenes/)

[Django](https://www.djangoproject.com/) has a really neat story and I didn't know about the different ways open source code exists. [Free on GitHub](https://github.com/django/django) This was open source by 2005 and the [BDLF's](https://en.wikipedia.org/wiki/Benevolent_dictator_for_life) (Adrian Holovaty and Jacob Kaplan-Moss)stepped down in 2018.

1) **Corporate Sponsor** - A group of engineers within a larger, for-profit company decide to open-source internal code. This is how React (Facebook) and Angular (Google) emerged. Typically engineers at the company are paid, in part, to work on open source though community involvement from developers outside of the core company occurs as well. While this structure has the stability of a wealthy benefactor, there can be confusion around the licensing aspects at times.

2) **Solo** - An individual developer initially creates code, open sources it, and retains default control. This is the case for VueJS, Tailwind CSS, and Laravel, among others. Typically the lead developer either raises contributions directly like Evan You of VueJS, offer add-on services like Spark for Laravel, or the founders provide highly-paid consulting services.

3) **Non-profit** - This was Django’s approach early on, in 2008, when the Django Software Foundation was formed to promote, support, and advance Django.

I love how this article refers to what the Django Fellows do as unsexy but necessary work needed to keep Django on track and currently are the only two paid employees.
YES Django is mostly all volunteer based and still a non-profit which really draws me in to working with them more. I really want to check out these DjangoCons and when I can donate then donate as well. This seems like an incredible community. 

### **Bookmark/Skim**

### What is Django

### First Django App - Part 1

### First Django App - Part 2 












[Back to 401 Index](401-index.md)