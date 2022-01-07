**NOTE: Please use https://github.com/matthiask/html-sanitizer instead, it's the successor and works the same (except with less bugs).**

===============
feincms-cleanse
===============

.. image:: https://travis-ci.org/feincms/feincms-cleanse.svg?branch=master
    :target: https://travis-ci.org/feincms/feincms-cleanse

This is the FeinCMS HTML cleansing function which lived under the name of
``feincms.utils.html.cleanse.cleanse_html``, and has been moved to
its own repository now to be usable in other projects, and to not set a
precedent for a particular HTML cleaning technique in FeinCMS anymore.

Usage is simple::

    from feincms_cleanse import cleanse_html

    >>> cleanse_html(u'<span style="font-weight:bold">some text</span>')
    u'<strong>some text</strong>'
