# The Galaxy Maps project


This projects aims in collection all Galaxy servers across the earth. We stricly encourage all Galaxy Admins to add their server to this map, no matter if the server is public or not. We will use this map to guide users to you, make people and funding agencies aware of your awesome service, connect Admins between instances more closely and build a network of potential training instances.

[Look at it!](https://github.com/bgruening/galaxy-maps/blob/master/server.geojson)


Simply add an entry like this to the [geosjon](https://github.com/bgruening/galaxy-maps/blob/master/server.geojson) file:

```json
      {
        "type": "Feature",
        "geometry": {
          "type": "Point",
          "coordinates": [7.85203, 48.02559]
        },
        "properties": {
          "name": "MPI-IE Galaxy Server",
          "URL": "http://deeptools.ie-freiburg.mpg.de",
          "description": "The Home of deepTools - test and play around with the latest deepTools version."
        }
      }
```

The Latitude and Longitude  for the `coordinates` section can be optained with this service for example: http://mondeca.com/index.php/en/any-place-en. Please note that the first number is Longitude and the second is Latitude.
