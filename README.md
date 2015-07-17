# django_vulnerable_app
Vulnerable App in Django


Install instructions:
-------------------

Lets assume you are on Ubuntu or Debian.

<pre>

$ sudo apt-get update && sudo apt-get upgrade

$ sudo apt-get install python-virtualenv git python-dev python-pip

$ git clone https://github.com/kurtcoke/django_vulnerable_app.git

$ virtualenv django_vulnerable_app


$ cd django_vulnerable_app

$ source bin/activate

$ pip install django

If you are using a proxy then run pip with --proxy="http://192.168.1.20:8080"

$ django-admin.py startproject webapp

$ cd webapp

$ python manage.py runserver

$ cd webapp

$ vim settings.py
</pre>

Add 'webapp' to INSTALLED_APPS

like this:

<pre>

INSTALLED_APPS = (
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'webapp',
)
</pre>

