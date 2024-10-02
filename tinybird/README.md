# Tinybird project

This folder contains all of the resources to build the Tinybird project for this demo.

## Project structure

This project contains:

```
├── datasources
│   └── nyc_taxis.datasource
└── pipes
    ├── nyc_taxi_geo.pipe
    └── trip_distance_trend.pipe
```

`nyc_taxi_geo.pipe` is used in the map. `trip_distance_trend.pipe` is another pipe to demonstrate additional use cases with the same data.

## Deploying the Tinybird resources

To deploy to Tinybird, you need to have the [Tinybird CLI installed](https://www.tinybird.co/docs/cli/overview). Then, you can run the following commands:

```sh
tb auth --token <your user admin token>
tb push --force
```

After deploying your resources, download the [NYC Yellow Taxi Trip Data](https://www.kaggle.com/datasets/elemento/nyc-yellow-taxi-trip-data?resource=download&select=yellow_tripdata_2016-03.csv) and append the file to the `nyc_taxis` Data Source.