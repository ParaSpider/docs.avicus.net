============
Writing YAML
============

All maps on Avicus require a file written in YAML that dictates how the map will function during a match. We have chosen to use YAML over other data serialization standards because it is efficient and human friendly but very powerful as well. You can use the documentation below to learn how to write in YAML.

.. warning::
    If you are new to markup languages, it may be wise to view examples of YAML to get a better feel of how it functions. You can find examples at `maps.avicus.net <http://maps.avicus.net>`_ by navigating the directories and locating any ``map.yml`` file.


Data Types
==========

There are various types of data that can be stored in YAML such as text, real numbers, whole numbers and binary values. Listed are the types of data used in Avicus YAML files.

* ``string``: A string holds any text. Strings should be surrounded with single quotes like so: ``'String Value'``. Single quotes in a string must be doubled to include two apostrophes instead: ``'The Alendaur''s Axe'``
* ``integer``: An integer and hold any whole number value from -2\ :sup:`31` to 2\ :sup:`31`.
* ``decimal``: Decimals can be any real number. Examples include: ``3.14``, ``-392.2``, ``60``.
* ``boolean``: There are two possible values for booleans: ``true`` or ``false``.
* ``duration``: Defines a period of time. Using ``s`` for seconds and ``m`` for minutes, durations can be written like so: ``25m``, ``30s``, ``0.5s``.
* ``coordinate``: Coordinates mark a location and direction in the world. You must specify the x, y and z values of a location in the map. Additionally, yaw (direction) and pitch (tilt) can be specified. Examples: ``25.5, 60, 30.5, -90, 0``, ``50, 80.5, 30.5``, ``0, 100, 0, 90``.


Formatting
==========

Below is an example of a YAML file. In this example, there are three data types at use: ``string``, ``boolean`` and ``integer``.  It is required, as shown in the example, to indent with two spaces. In the example, ``family`` is the parent of the sections ``parents``, ``kids``, ``happy``, ``pets`` and ``address`` because they are spaced to fall under ``family``. Take time to ensure your spacing is correct when writing YAML as that is the most common cause for issues.

.. code-block:: yaml
    
    family:
      parents:
      - 'Charles'
      - 'Lily'
      kids:
      - 'Tim'
      happy: true
      pets: 3
      address: '123 Everton Lane'