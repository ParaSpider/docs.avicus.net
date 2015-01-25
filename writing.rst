============
Writing YAML
============

All maps on Avicus require a file written in YAML that dictates how the map will function during a match. We have chosen to use YAML over other data serialization standards because it is efficient and human friendly but very powerful as well. You can use the documentation below to learn how to write in YAML.

.. warning::
    If you are new to markup languages, it may be wise to view examples of YAML to get a better feel of how it functions. You can find examples at `maps.avicus.net <http://maps.avicus.net>`_ by navigating the directories and locating any `map.yml` file.

Data Types
==========

There are various types of data that can be stored in YAML such as text, real numbers, whole numbers and binary values. Listed are the types of data used in Avicus YAML files.

* `string`: A string holds any text. Strings should be surrounded with apostrophes like so: `key: 'String Value'`
* `integer`: An integer and hold any whole number value (..., -1, 0, 1, ...)
* `decimal`: Decimals can be any real number. Examples include: `3.14`, `-392.2`, `60`.