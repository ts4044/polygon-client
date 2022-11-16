
# Polygon Rest Client

This library is written on top of Max's Final exam submission. The goal of the library is to run calculations and store data into a sql database.

The library can be imported as follows:
```
from polygon_client import RestClient
```

This creates an object with the following functions:
```
@static
fetch_key()
```

To initialize the Polygon client, you can use the fetch_key() method to obtain the key provided by professor.
```
key = RestClient.fetch_key()
client = RESTClient(key)
```