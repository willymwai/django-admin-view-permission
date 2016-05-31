# Admin View Permission
[![Build Status](https://travis-ci.org/ctxis/django-admin-view-permission.svg?branch=master)](https://travis-ci.org/ctxis/django-admin-view-permission)
[![Coverage Status](https://coveralls.io/repos/github/ctxis/django-admin-view-permission/badge.svg?branch=master)](https://coveralls.io/github/ctxis/django-admin-view-permission?branch=master)
[![Code Climate](https://codeclimate.com/github/ctxis/django-admin-view-permission/badges/gpa.svg)](https://codeclimate.com/github/ctxis/django-admin-view-permission)

Reusable application which provides a view permission for the existing models.

## Requirements
* Django: 1.9

## Setup
* `pip install https://github.com/ctxis/django-admin-view-permission/archive/master.zip`

and then add `admin_view_permission` at the INSTALLED_APPS like this:

    INSTALLED_APPS = [
        'amdin_view_permission',
        'django.contrib.admin',
        ...
    ]

and finally run `python manage.py migrate`.

## Configuration
This app provides a setting:

    ADMIN_VIEW_PERMISSION_MODELS = [
        auth.User,
        ...
    ]

in which you can provide which models you want to be added the view permission.