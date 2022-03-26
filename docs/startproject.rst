Lets get started
================

The Tweets Model
----------------

.. code-block:: console
    :emphasize-lines: 1

    $ .\manage.py startapp tweets

0:39:35 9. Store Data from Django Model
---------------------------------------

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