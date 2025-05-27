============
django-hx
============

django-hx is a Django app that provides a simple way to use [htmx](https://htmx.org/) with Django. It allows you to easily create dynamic, interactive web applications using htmx and Django's templating system.

Quick start
-----------


1. Add `django_hx` to your `INSTALLED_APPS` setting:

   ```python
    INSTALLED_APPS = [
         ...
         'django_hx',
    ]
    ```

2. Include the `django_hx` URLconf in your project’s `urls.py` like this:
   ```python
    from django.urls import include, path

    urlpatterns = [
        ...
        path('hx/', include('django_hx.urls')),
    ]
    ```

3. Load the `hx` template tag in your templates:
   ```html
    {% load hx %}
    ```
