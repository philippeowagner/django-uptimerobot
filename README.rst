Uptime Robot integration for Django
============

Uptime Robot http://uptimerobot.com integration for your Django project.

Installation
------------

To get the latest stable release from PyPi

.. code-block:: bash

    $ pip install django-uptimerobot

To get the latest commit from GitHub

.. code-block:: bash

    $ pip install -e git+git://github.com/arteria.ch/django-uptimerobot.git#egg=uptimerobot

TODO: Describe further installation steps (edit / remove the examples below):

Add ``uptimerobot`` to your ``INSTALLED_APPS``

.. code-block:: python

    INSTALLED_APPS = (
        ...,
        'uptimerobot',
    )

Add the ``uptimerobot`` URLs to your ``urls.py``

.. code-block:: python

    urlpatterns = patterns('',
        ...
        url(r'^uptimerobot/', include('uptimerobot.urls')),
    )

Before your tags/filters are available in your templates, load them by using

.. code-block:: html

	{% load uptimerobot_tags %}


Don't forget to migrate your database

.. code-block:: bash

    ./manage.py migrate uptimerobot


Usage
-----

TODO: Describe usage or point to docs. Also describe available settings and
templatetags.


Contribute
----------

If you want to contribute to this project, please perform the following steps

.. code-block:: bash

    # Fork this repository
    # Clone your fork
    $ mkvirtualenv -p python2.7 django-uptimerobot
    $ python setup.py install
    $ pip install -r dev_requirements.txt

    $ git co -b feature_branch master
    # Implement your feature and tests
    $ git add . && git commit
    $ git push -u origin feature_branch
    # Send us a pull request for your feature branch