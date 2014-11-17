py-4chan
========

> **Notice:** Please migrate to the new and improved `BASC-py4chan <https://github.com/bibanon/BASC-py4chan>`_ wrapper, it has many improvements and new features (such as catalog support.)
> py-4chan has entered legacy support, meaning that no new features will be added. However, the `Bibliotheca Anonoma <https://github.com/bibanon/bibanon/wiki>`_ will ensure that py-4chan will work as long as we possibly can, to ensure that legacy API dumping apps still work.

Python Wrapper for 4chan API. Uses requests, respects if-modified-since
headers on updating threads. Caches thread objects. Fun stuff.

Sample Usage
~~~~~~~~~~~~

.. code:: python

    import py4chan
    b = py4chan.Board('b')
    thread = b.getThread(423491034)

    print thread

    for file in thread.Files():
        print file
        
    # In a while...
    print "I fetched", thread.update(), "new replies."

API Documentation coming soon, but you can figure most of it out from
the source. It's not rocket science.

`You can install this package straight from
PyPi <https://pypi.python.org/pypi/py-4chan>`__.

::

    # upload command
    python setup.py sdist upload

License
=======

.. code:: text

    DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
                        Version 2, December 2004

     Copyright (C) 2004 Sam Hocevar <sam@hocevar.net>

     Everyone is permitted to copy and distribute verbatim or modified
     copies of this license document, and changing it is allowed as long
     as the name is changed.

                DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
       TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION

      0. You just DO WHAT THE FUCK YOU WANT TO.

