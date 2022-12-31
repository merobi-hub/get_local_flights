# Flights

KFOs in your bounding box from the OpenSky API

### Description

A script for pulling flight data for a defined area from the [OpenSky API](https://openskynetwork.github.io/opensky-api/rest.html).

### How to Use

Execute `flights.py` with an OpenSky username and password, passing in either one
of the preconfigured area options ('Barrington', 'Nayatt', 'RI', 'NY'), setting 
a custom bounding box using the `--lamin`, `--lomin`, `--lamax`, and `--lomax` 
arguments, or passing in an ISO country code (e.g., 'USA'). The default area is 
Barrington, RI, and the default country is USA.

For example:

```
$ python3 flights.py --bbox True --lamin 41.146 --lomin -71.862 --lamax 42.018 --lomax -71.120 --username username --password password
```

```
$ python3 flights.py --area RI --username username --password password
```

```
python3 flights.py --country True --username username --password password
```

```
python3 flights.py --country True --iso GB --username username --password password
```

### Prerequisites

OpenSky account  
Python 3.10.7

### License

MIT License

