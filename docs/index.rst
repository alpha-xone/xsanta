xsanta
======

Secret Santa sender / receiver generator

|pypi| |actions| |version| |download|

|coffee|

Installation
============

.. code-block:: console

   pip install xsanta

Example
=======

In python:

.. code-block:: python

    >>> from secret import santa

    >>> invited = [
    ...     'Iron Man', 'Captain America', 'Thanos', 'Hulk',
    ...    'Black Widow', 'Thor', 'Loki', 'Wanda Maximoff',
    ... ]
    >>> excluded = [
    ...     ('Iron Man', 'Captain America'),
    ...     ('Thor', 'Loki'),
    ...     ('Black Widow', 'Hulk'),
    ... ]

    >>> santa.run(invited, excluded, emoji=False)
    Thor >> Thanos >> Loki >> Hulk >> Iron Man >> Thor
    Captain America >> Black Widow >> Wanda Maximoff >> Captain America

.. |pypi| image:: https://img.shields.io/pypi/v/xsanta.svg
    :target: https://badge.fury.io/py/xsanta
.. |version| image:: https://img.shields.io/pypi/pyversions/xsanta.svg
    :target: https://badge.fury.io/py/xsanta
.. |actions| image:: https://github.com/alpha-xone/xsanta/workflows/Auto%20CI/badge.svg
    :target: https://github.com/alpha-xone/xsanta/actions
.. |docs| image:: https://readthedocs.org/projects/xsanta/badge/?version=latest
    :target: https://xsanta.readthedocs.io/
.. |download| image:: https://img.shields.io/pypi/dm/xsanta
   :target: https://pypistats.org/packages/xsanta
.. |coffee| image:: https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png
   :target: https://www.buymeacoffee.com/Lntx29Oof

In command line:

.. code-block:: console

    python secret\santa.py "['Iron Man', 'Captain America', 'Thanos']" --emoji=False
    Captain America >> Thanos >> Iron Man >> Captain America
