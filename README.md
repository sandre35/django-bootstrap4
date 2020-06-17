# django-bootstrap 4

[![image](https://travis-ci.org/zostera/django-bootstrap4.svg?branch=main)](https://travis-ci.org/zostera/django-bootstrap4)
[![image](https://coveralls.io/repos/github/zostera/django-bootstrap4/badge.svg?branch=main)](https://coveralls.io/github/zostera/django-bootstrap4?branch=main)
[![Latest PyPI version](https://img.shields.io/pypi/v/django-bootstrap4.svg)](https://pypi.python.org/pypi/django-bootstrap4)
[![Any color you like](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)

Bootstrap 4 integration for Django.

## Goal

The goal of this project is to seamlessly blend Django and Bootstrap 4.

## Requirements

Django 2.2 or 3.0 with Python 3.6 or higher.

## Documentation

The full documentation is at https://django-bootstrap4.readthedocs.io/

## Installation

1. Install using pip:

    ```shell script
    pip install django-bootstrap4
    ```
   
   Alternatively, you can install download or clone this repo and call ``pip install -e .``.

2. Add to `INSTALLED_APPS` in your `settings.py`:

   ```python
   INSTALLED_APPS = (
       # ...
       "bootstrap4",
       # ...
   )
   ````

3. In your templates, load the `bootstrap4` library and use the `bootstrap_*` tags:

## Example template

```djangotemplate
{% load bootstrap4 %}

{# Display a form #}

<form action="/url/to/submit/" method="post" class="form">
    {% csrf_token %}
    {% bootstrap_form form %}
    {% buttons %}
        <button type="submit" class="btn btn-primary">Submit</button>
    {% endbuttons %}
</form>
```

Demo
----

A demo app is provided in `demo`. You can run it from your virtualenv with `python manage.py runserver`.


Bugs and suggestions
--------------------

If you have found a bug or if you have a request for additional functionality, please use the issue tracker on GitHub.

https://github.com/zostera/django-bootstrap4/issues


License
-------

You can use this under BSD-3-Clause. See [LICENSE](LICENSE) file for details.


Author
------

Developed and maintained by [Zostera](https://zostera.nl).

Original author: [Dylan Verheul](https://github.com/dyve).

Thanks to everybody that has contributed pull requests, ideas, issues, comments and kind words.

Please see [AUTHORS.md](AUTHORS.md) for a list of contributors.