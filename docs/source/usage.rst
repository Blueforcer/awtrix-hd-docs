Usage
=====

.. _installation:

Installation
------------

You need a license to run AWTRIX HD
https://blueforcer.gumroad.com/l/awtrixhd
As one of the alpha tester (limited seats) you will get a 100% coupon if you want. -> PM me
You can also buy a license to support the development. Minimum value is 10€.

.. code-block:: console

   (.venv) $ pip install lumache

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

