# The Galaxy Maps project


This projects aims in collection all Galaxy servers across the earth. We stricly encourage all Galaxy Admins to add their server to this map, no matter if the server is public or not. We will use this map to guide users to you, make people and funding agencies aware of your awesome service, connect Admins between instances more closely and build a network of potential training instances.

[Look at it!](https://github.com/bgruening/galaxy-maps/blob/master/server.geojson)

You want to be in this map, simply add an entry to the [geosjon](https://github.com/bgruening/galaxy-maps/blob/master/server.geojson) file, if you are:

- A Galaxy instance:

```json
      {
        "type": "Feature",
        "geometry": {
          "type": "Point",
          "coordinates": [7.85203, 48.02559]
        },
        "properties": {
          "Name": "MPI-IE Galaxy Server",
          "URL": "http://deeptools.ie-freiburg.mpg.de",
          "Description": "The Home of deepTools - test and play around with the latest deepTools version."
        }
      }
```

- A Galaxy instance with training

```json
      {
        "type": "Feature",
        "geometry": {
          "type": "Point",
          "coordinates": [7.84831, 48.00362]
        },
        "properties": {
          "Name": "Freiburg Galaxy Server",
          "URL": "http://galaxy.uni-freiburg.de",
          "Description": "",
          "Training": "We offer twice a year a one week hands-on training course.",
          "marker-size": "medium",
          "marker-symbol": "college",
          "marker-color": "#bbbbbb"
        }
      }
```

- A possible trainer

```json
      {
        "type": "Feature",
        "geometry": {
          "type": "Point",
          "coordinates": [7.83354, 48.01462]
        },
        "properties": {
          "Name": "Björn Grüning",
          "Mail": "bjoern.gruening@gmail.com",
          "Affiliation": "University of Freiburg",
          "Website": "",
          "Training": "",
          "marker-size": "medium",
          "marker-symbol": "star",
          "marker-color": "#e5afcf"
        }
      }
```

The Latitude and Longitude for the `coordinates` section can be obtained with this service for example: http://mondeca.com/index.php/en/any-place-en. Please note that the first number is Longitude and the second is Latitude.
