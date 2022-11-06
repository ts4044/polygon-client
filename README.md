
# Polygon Rest Client

This library is written on top of Max's Final exam submission. The goal of the library is to run calculations and store data into a sql database.

The library can be imported as follows:
```
from polygon_client import RestClient
```

This creates an object with the following functions:
```
@static
ts_to_datetime(timestamp)

@static
reset_raw_data_tables(engine, currency_pairs)

@static
initialize_raw_data_tables(engine, currency_pairs)

@static
initialize_aggregated_tables(engine, currency_pairs)

@static
aggregate_raw_data_tables(engine, currency_pairs)

calculate(currency_pairs)
```

calculate() is the main function of the library. After initializing the library object, you can call object.calculate(currency_pairs) to run the calculations on a currency pair and store into a sqlite database.

```
client = RestClient()
client.calculate(currency_pairs)
```