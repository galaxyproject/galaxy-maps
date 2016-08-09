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

Additional informations
-----------------------

You can add more properties to your entry. Here is an example with some comments:

```cpp
        "properties": {
            /* OPTIONAL: default "" 
               A title to show when this item is clicked or
               hovered over
            */
            "title": "A title",

            /*
                OPTIONAL: default ""
                A description to show when this item is clicked or hovered over
            */
            "description": "A description",

            /*  OPTIONAL: default "medium"
                specify the size of the marker. sizes
                can be different pixel sizes in different
                implementations value must be one of
                "small"
                "medium"
                "large"
            */
            "marker-size": "medium",

            /*  OPTIONAL: default ""
                a symbol to position in the center of this icon
                if not provided or "", no symbol is overlaid
                and only the marker is shown
                Allowed values include
                - Icon ID from the Maki project at http://mapbox.com/maki/
                - An integer 0 through 9
                - A lowercase character "a" through "z"
            */
            "marker-symbol": "bus",

            /*  OPTIONAL: default "7e7e7e"
                the marker's color
            
                value must follow COLOR RULES
            */
            "marker-color": "#fff",

            /*  OPTIONAL: default "555555"
                the color of a line as part of a polygon, polyline, or multigeometry

                value must follow COLOR RULES
            */
            "stroke": "#555555",

            /*  OPTIONAL: default 1.0
                the opacity of the line component of a polygon, polyline, or multigeometry
            
                value must be a floating point number greater than or equal to
                zero and less or equal to than one
            */
            "stroke-opacity": 1.0,

            /*  OPTIONAL: default 2
                the width of the line component of a polygon, polyline, or multigeometry
            
                value must be a floating point number greater than or equal to 0
            */
            "stroke-width": 2,

            /*  OPTIONAL: default "555555"
                the color of the interior of a polygon
            
                value must follow COLOR RULES
            */
            "fill": "#555555",

            /*  OPTIONAL: default 0.6
                the opacity of the interior of a polygon. Implementations
                may choose to set this to 0 for line features.
            
                value must be a floating point number greater than or equal to
                zero and less or equal to than one
            */
            "fill-opacity": 0.5,
            /* Name of the Galaxy Server */
            "name": "Freiburg Galaxy Server",
            /* URL of the Galaxy Server */
            "URL": "http://galaxy.uni-freiburg.de",
            /* Some details about offered training, can be a URL as well. */
            "Training": "We offer twice a year a one week hands-on training course."
      }
```

