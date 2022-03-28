Lets get started
================

In order to activate pipenv virtual environment we run:
pipenv shell
to deactivate it just:
exit

In order to install all dependencies of the virtual environment:
pipenv run
OR alternatively (outside the pipenv),
pipenv --three sync

The Tweets Model
----------------

.. code-block:: console
    :emphasize-lines: 1

    $ .\manage.py startapp tweets

0:39:35 9. Store Data from Django Model
---------------------------------------

You Tube video uploaded at: https://www.youtube.com/watch?v=f1R_bykXHGE&t=1653s

.. code-block:: shell
    :emphasize-lines: 1

    $ .\manage.py shell
    >>> from tweets.models import Tweet
    >>> obj = Tweet()
    >>> obj.content = "Hello world!"
    >>> obj.save()

.. code-block:: shell
    :emphasize-lines: 1

    $ .\manage.py shell
    >>> from tweets.models import Tweet
    >>> obj = Tweet.objects.get(id=1)
    >>> obj.content
    'Hello world!'

0:43:10 10. Intro to URL Routing and Dynamic Routing
----------------------------------------------------

In order to create our first url we start from creating the view. We can create class view 
or function view.
After that i can go to the urls.py in my main root and add the url to my view. Of-course 
i have to build a nice html page for my url.

0:47:57 11. Handling Dynamic Routing
------------------------------------



0:51:32 12. Dynamic View into REST API Endpoint
Σταμάτησα στο 49:53