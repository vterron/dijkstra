Dijkstra's algorithm
====================

A Pythonic implementation of Dijkstra's algorithm, as shown during my keynote talk at [PyConES 2015](http://2015.es.pycon.org/en/). This implementation finds the cheapest route between any two airports in the world. As we do not have actual data on all flight prices, this implementation assumes that fares are directly proportional to the traveled distance. This means that what we are therefore actually minimizing is the total distance, following a route as close as possible to the [great-circle arc](https://en.wikipedia.org/wiki/Haversine_formula) between the two airports.

To use the code, follow these steps:

* ``pip3 install haversine # to compute distances between two points on a sphere``
* ``wget https://raw.githubusercontent.com/jpatokal/openflights/master/data/airports.dat``
* ``wget https://raw.githubusercontent.com/jpatokal/openflights/master/data/routes.dat -O flights.dat``
* ``python3 dijkstra.py``

This generates the following output, finding the cheapest route between [Valencia](https://en.wikipedia.org/wiki/Valencia) (Spain) and [Portland](https://en.wikipedia.org/wiki/Portland,_Oregon) (Oregon, United States):

```
0 | Airport(code='VLC', name='Valencia', country='Spain', latitude=39.489314, longitude=-0.481625)
1 | Airport(code='BRS', name='Bristol', country='United Kingdom', latitude=51.382669, longitude=-2.719089)
2 | Airport(code='KEF', name='Keflavik International Airport', country='Iceland', latitude=63.985, longitude=-22.605556)
3 | Airport(code='SEA', name='Seattle Tacoma Intl', country='United States', latitude=47.449, longitude=-122.309306)
4 | Airport(code='PDX', name='Portland Intl', country='United States', latitude=45.588722, longitude=-122.5975)
917.0652085335274 €
```

This is not an official Google product.
