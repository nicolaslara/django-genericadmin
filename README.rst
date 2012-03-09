======================
 Django Generic Admin
======================

This is a clone of http://code.google.com/p/django-genericadmin/ with
minor improvements for it to work with django 1.3

genericadmin adds support for generic relations in Django's admin
interface by making them look and feel as close to a ForeignKey field
as possible.

Installation
============

Just run::

    pip install -e git+git@github.com:nicolaslara/django-genericadmin.git#egg=django-genericadmin

And add 'genericadmin' to your INSTALLED_APPS


If you're using a custom base_site.html you'll need to add the following code to it::

    {% block footer %}
      {{ block.super }}
      <script type="text/javascript">{% include "admin/genericadmin/genericadmin.js" %}</script>
    {% endblock %}
