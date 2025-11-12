
# Overture Maps Schema (Schema)

`ogc.overturemaps.schemas.schema` *v0.1*

A JSON Schema for the canonical GeoJSON form of Overture Maps Features.

[*Status*](http://www.opengis.net/def/status): Under development

## Examples

### Example 1
#### json
```json
{
  "id": "overture:addresses:address:1",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      -71.2086153,
      42.3373725
    ]
  },
  "properties": {
    "theme": "addresses",
    "type": "address",
    "version": 0,
    "country": "US",
    "address_levels": [
      {
        "value": "MA"
      },
      {
        "value": "NEWTON CENTRE"
      }
    ],
    "postcode": "02459",
    "street": "COMMONWEALTH AVE",
    "number": "1000"
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/schema/context.jsonld",
  "id": "overture:addresses:address:1",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      -71.2086153,
      42.3373725
    ]
  },
  "properties": {
    "theme": "addresses",
    "type": "address",
    "version": 0,
    "country": "US",
    "address_levels": [
      {
        "value": "MA"
      },
      {
        "value": "NEWTON CENTRE"
      }
    ],
    "postcode": "02459",
    "street": "COMMONWEALTH AVE",
    "number": "1000"
  }
}
```

#### ttl
```ttl
@prefix geojson: <https://purl.org/geojson/vocab#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

<overture:addresses:address:1> a <file:///github/workspace/address>,
        geojson:Feature ;
    geojson:geometry [ a geojson:Point ;
            geojson:coordinates ( -7.120862e+01 4.233737e+01 ) ] .


```


### Example 2
#### json
```json
{
  "id": "overture:bathymetry:example:1",
  "type": "Feature",
  "geometry": {
    "type": "Polygon",
    "coordinates": [
      [
        [
          -73.1902319,
          41.6678018
        ],
        [
          -73.1896302,
          41.667817
        ],
        [
          -73.1890448,
          41.6667723
        ],
        [
          -73.1899188,
          41.6666994
        ],
        [
          -73.1902319,
          41.6678018
        ]
      ]
    ]
  },
  "properties": {
    "theme": "base",
    "type": "bathymetry",
    "depth": 2500,
    "cartography": {
      "min_zoom": 0,
      "max_zoom": 23,
      "sort_key": 7
    },
    "sources": [
      {
        "record_id": "x123",
        "property": "",
        "dataset": "some source"
      }
    ],
    "version": 0
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/schema/context.jsonld",
  "id": "overture:bathymetry:example:1",
  "type": "Feature",
  "geometry": {
    "type": "Polygon",
    "coordinates": [
      [
        [
          -73.1902319,
          41.6678018
        ],
        [
          -73.1896302,
          41.667817
        ],
        [
          -73.1890448,
          41.6667723
        ],
        [
          -73.1899188,
          41.6666994
        ],
        [
          -73.1902319,
          41.6678018
        ]
      ]
    ]
  },
  "properties": {
    "theme": "base",
    "type": "bathymetry",
    "depth": 2500,
    "cartography": {
      "min_zoom": 0,
      "max_zoom": 23,
      "sort_key": 7
    },
    "sources": [
      {
        "record_id": "x123",
        "property": "",
        "dataset": "some source"
      }
    ],
    "version": 0
  }
}
```

#### ttl
```ttl
@prefix geojson: <https://purl.org/geojson/vocab#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

<overture:bathymetry:example:1> a <file:///github/workspace/bathymetry>,
        geojson:Feature ;
    geojson:geometry [ a geojson:Polygon ;
            geojson:coordinates ( ( ( -7.319023e+01 4.16678e+01 ) ( -7.318963e+01 4.166782e+01 ) ( -7.318904e+01 4.166677e+01 ) ( -7.318992e+01 4.16667e+01 ) ( -7.319023e+01 4.16678e+01 ) ) ) ] .


```


### Example 3
#### json
```json
{
  "id": "08b2748cc1383fff0001b38438099b73",
  "type": "Feature",
  "geometry": {
    "type": "Polygon",
    "coordinates": [
      [
        [
          -85.6743541,
          42.9676009
        ],
        [
          -85.6743623,
          42.9674649
        ],
        [
          -85.6744114,
          42.9674803
        ],
        [
          -85.6744559,
          42.9674919
        ],
        [
          -85.6745302,
          42.9675058
        ],
        [
          -85.6746036,
          42.9675151
        ],
        [
          -85.6746959,
          42.9675171
        ],
        [
          -85.675835,
          42.9674967
        ],
        [
          -85.6758985,
          42.9674915
        ],
        [
          -85.6759656,
          42.967483
        ],
        [
          -85.6760399,
          42.9674711
        ],
        [
          -85.676099,
          42.9674566
        ],
        [
          -85.6761817,
          42.9674324
        ],
        [
          -85.676227,
          42.9674184
        ],
        [
          -85.6762149,
          42.9675911
        ],
        [
          -85.6761726,
          42.9675857
        ],
        [
          -85.676106,
          42.9675781
        ],
        [
          -85.6760499,
          42.9675741
        ],
        [
          -85.6759947,
          42.9675723
        ],
        [
          -85.6743541,
          42.9676009
        ]
      ]
    ]
  },
  "properties": {
    "theme": "base",
    "type": "infrastructure",
    "subtype": "bridge",
    "class": "bridge",
    "names": {
      "primary": "Gillett Bridge",
      "rules": [
        {
          "variant": "alternate",
          "value": "Interurban Bridge"
        }
      ]
    },
    "sources": [
      {
        "property": "",
        "record_id": "w556368546@3",
        "dataset": "OpenStreetMap"
      }
    ],
    "version": 0
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/schema/context.jsonld",
  "id": "08b2748cc1383fff0001b38438099b73",
  "type": "Feature",
  "geometry": {
    "type": "Polygon",
    "coordinates": [
      [
        [
          -85.6743541,
          42.9676009
        ],
        [
          -85.6743623,
          42.9674649
        ],
        [
          -85.6744114,
          42.9674803
        ],
        [
          -85.6744559,
          42.9674919
        ],
        [
          -85.6745302,
          42.9675058
        ],
        [
          -85.6746036,
          42.9675151
        ],
        [
          -85.6746959,
          42.9675171
        ],
        [
          -85.675835,
          42.9674967
        ],
        [
          -85.6758985,
          42.9674915
        ],
        [
          -85.6759656,
          42.967483
        ],
        [
          -85.6760399,
          42.9674711
        ],
        [
          -85.676099,
          42.9674566
        ],
        [
          -85.6761817,
          42.9674324
        ],
        [
          -85.676227,
          42.9674184
        ],
        [
          -85.6762149,
          42.9675911
        ],
        [
          -85.6761726,
          42.9675857
        ],
        [
          -85.676106,
          42.9675781
        ],
        [
          -85.6760499,
          42.9675741
        ],
        [
          -85.6759947,
          42.9675723
        ],
        [
          -85.6743541,
          42.9676009
        ]
      ]
    ]
  },
  "properties": {
    "theme": "base",
    "type": "infrastructure",
    "subtype": "bridge",
    "class": "bridge",
    "names": {
      "primary": "Gillett Bridge",
      "rules": [
        {
          "variant": "alternate",
          "value": "Interurban Bridge"
        }
      ]
    },
    "sources": [
      {
        "property": "",
        "record_id": "w556368546@3",
        "dataset": "OpenStreetMap"
      }
    ],
    "version": 0
  }
}
```

#### ttl
```ttl
@prefix geojson: <https://purl.org/geojson/vocab#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

<file:///github/workspace/08b2748cc1383fff0001b38438099b73> a <file:///github/workspace/infrastructure>,
        geojson:Feature ;
    geojson:geometry [ a geojson:Polygon ;
            geojson:coordinates ( ( ( -8.567435e+01 4.29676e+01 ) ( -8.567436e+01 4.296746e+01 ) ( -8.567441e+01 4.296748e+01 ) ( -8.567446e+01 4.296749e+01 ) ( -8.567453e+01 4.296751e+01 ) ( -8.56746e+01 4.296752e+01 ) ( -8.56747e+01 4.296752e+01 ) ( -8.567584e+01 4.29675e+01 ) ( -8.56759e+01 4.296749e+01 ) ( -8.567597e+01 4.296748e+01 ) ( -8.567604e+01 4.296747e+01 ) ( -8.56761e+01 4.296746e+01 ) ( -8.567618e+01 4.296743e+01 ) ( -8.567623e+01 4.296742e+01 ) ( -8.567621e+01 4.296759e+01 ) ( -8.567617e+01 4.296759e+01 ) ( -8.567611e+01 4.296758e+01 ) ( -8.567605e+01 4.296757e+01 ) ( -8.567599e+01 4.296757e+01 ) ( -8.567435e+01 4.29676e+01 ) ) ) ] .


```


### Example 4
#### json
```json
{
  "id": "overture:land_cover:example:1",
  "type": "Feature",
  "geometry": {
    "type": "Polygon",
    "coordinates": [
      [
        [
          -73.1902319,
          41.6678018
        ],
        [
          -73.1896302,
          41.667817
        ],
        [
          -73.1890448,
          41.6667723
        ],
        [
          -73.1899188,
          41.6666994
        ],
        [
          -73.1902319,
          41.6678018
        ]
      ]
    ]
  },
  "properties": {
    "theme": "base",
    "type": "land_cover",
    "subtype": "forest",
    "cartography": {
      "min_zoom": 11,
      "max_zoom": 23,
      "sort_key": 2
    },
    "sources": [
      {
        "record_id": "x123",
        "property": "",
        "dataset": "some source"
      }
    ],
    "version": 0
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/schema/context.jsonld",
  "id": "overture:land_cover:example:1",
  "type": "Feature",
  "geometry": {
    "type": "Polygon",
    "coordinates": [
      [
        [
          -73.1902319,
          41.6678018
        ],
        [
          -73.1896302,
          41.667817
        ],
        [
          -73.1890448,
          41.6667723
        ],
        [
          -73.1899188,
          41.6666994
        ],
        [
          -73.1902319,
          41.6678018
        ]
      ]
    ]
  },
  "properties": {
    "theme": "base",
    "type": "land_cover",
    "subtype": "forest",
    "cartography": {
      "min_zoom": 11,
      "max_zoom": 23,
      "sort_key": 2
    },
    "sources": [
      {
        "record_id": "x123",
        "property": "",
        "dataset": "some source"
      }
    ],
    "version": 0
  }
}
```

#### ttl
```ttl
@prefix geojson: <https://purl.org/geojson/vocab#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

<overture:land_cover:example:1> a <file:///github/workspace/land_cover>,
        geojson:Feature ;
    geojson:geometry [ a geojson:Polygon ;
            geojson:coordinates ( ( ( -7.319023e+01 4.16678e+01 ) ( -7.318963e+01 4.166782e+01 ) ( -7.318904e+01 4.166677e+01 ) ( -7.318992e+01 4.16667e+01 ) ( -7.319023e+01 4.16678e+01 ) ) ) ] .


```


### Example 5
#### json
```json
{
  "id": "overture:land:example:1",
  "type": "Feature",
  "geometry": {
    "type": "Polygon",
    "coordinates": [
      [
        [
          34.4379197,
          28.7592689
        ],
        [
          34.4380109,
          28.7595816
        ],
        [
          34.4380173,
          28.7601587
        ],
        [
          34.4380538,
          28.7606186
        ],
        [
          34.438154,
          28.7609863
        ],
        [
          34.4380735,
          28.7612459
        ],
        [
          34.4377346,
          28.7608396
        ],
        [
          34.4377158,
          28.7606139
        ],
        [
          34.4377105,
          28.7605527
        ],
        [
          34.43763,
          28.7604258
        ],
        [
          34.4376407,
          28.7603599
        ],
        [
          34.4376488,
          28.7602494
        ],
        [
          34.4376863,
          28.7599673
        ],
        [
          34.4376675,
          28.759798
        ],
        [
          34.437689,
          28.7596216
        ],
        [
          34.4379197,
          28.7592689
        ]
      ]
    ]
  },
  "properties": {
    "theme": "base",
    "type": "land",
    "subtype": "sand",
    "class": "dune",
    "names": {
      "primary": "Hadeida"
    },
    "source_tags": {
      "natural": "dune",
      "surface": "sand"
    },
    "sources": [
      {
        "record_id": "w407753930@3",
        "property": "",
        "dataset": "OpenStreetMap"
      }
    ],
    "version": 0
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/schema/context.jsonld",
  "id": "overture:land:example:1",
  "type": "Feature",
  "geometry": {
    "type": "Polygon",
    "coordinates": [
      [
        [
          34.4379197,
          28.7592689
        ],
        [
          34.4380109,
          28.7595816
        ],
        [
          34.4380173,
          28.7601587
        ],
        [
          34.4380538,
          28.7606186
        ],
        [
          34.438154,
          28.7609863
        ],
        [
          34.4380735,
          28.7612459
        ],
        [
          34.4377346,
          28.7608396
        ],
        [
          34.4377158,
          28.7606139
        ],
        [
          34.4377105,
          28.7605527
        ],
        [
          34.43763,
          28.7604258
        ],
        [
          34.4376407,
          28.7603599
        ],
        [
          34.4376488,
          28.7602494
        ],
        [
          34.4376863,
          28.7599673
        ],
        [
          34.4376675,
          28.759798
        ],
        [
          34.437689,
          28.7596216
        ],
        [
          34.4379197,
          28.7592689
        ]
      ]
    ]
  },
  "properties": {
    "theme": "base",
    "type": "land",
    "subtype": "sand",
    "class": "dune",
    "names": {
      "primary": "Hadeida"
    },
    "source_tags": {
      "natural": "dune",
      "surface": "sand"
    },
    "sources": [
      {
        "record_id": "w407753930@3",
        "property": "",
        "dataset": "OpenStreetMap"
      }
    ],
    "version": 0
  }
}
```

#### ttl
```ttl
@prefix geojson: <https://purl.org/geojson/vocab#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

<overture:land:example:1> a <file:///github/workspace/land>,
        geojson:Feature ;
    geojson:geometry [ a geojson:Polygon ;
            geojson:coordinates ( ( ( 3.443792e+01 2.875927e+01 ) ( 3.443801e+01 2.875958e+01 ) ( 3.443802e+01 2.876016e+01 ) ( 3.443805e+01 2.876062e+01 ) ( 3.443815e+01 2.876099e+01 ) ( 3.443807e+01 2.876125e+01 ) ( 3.443773e+01 2.876084e+01 ) ( 3.443772e+01 2.876061e+01 ) ( 3.443771e+01 2.876055e+01 ) ( 3.443763e+01 2.876043e+01 ) ( 3.443764e+01 2.876036e+01 ) ( 3.443765e+01 2.876025e+01 ) ( 3.443769e+01 2.875997e+01 ) ( 3.443767e+01 2.87598e+01 ) ( 3.443769e+01 2.875962e+01 ) ( 3.443792e+01 2.875927e+01 ) ) ) ] .


```


### Example 6
#### json
```json
{
  "id": "overture:land_use:example:1",
  "type": "Feature",
  "geometry": {
    "type": "Polygon",
    "coordinates": [
      [
        [
          -83.8710175,
          10.3469578
        ],
        [
          -83.8700924,
          10.3470179
        ],
        [
          -83.870043,
          10.3462819
        ],
        [
          -83.8709681,
          10.3462218
        ],
        [
          -83.8710175,
          10.3469578
        ]
      ]
    ]
  },
  "properties": {
    "theme": "base",
    "type": "land_use",
    "subtype": "recreation",
    "class": "pitch",
    "surface": "recreation_grass",
    "source_tags": {
      "leisure": "pitch",
      "sport": "soccer"
    },
    "names": {
      "primary": "Plaza Deportes Finca Tres"
    },
    "sources": [
      {
        "record_id": "w509487233@1",
        "property": "",
        "dataset": "OpenStreetMap"
      }
    ],
    "version": 0
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/schema/context.jsonld",
  "id": "overture:land_use:example:1",
  "type": "Feature",
  "geometry": {
    "type": "Polygon",
    "coordinates": [
      [
        [
          -83.8710175,
          10.3469578
        ],
        [
          -83.8700924,
          10.3470179
        ],
        [
          -83.870043,
          10.3462819
        ],
        [
          -83.8709681,
          10.3462218
        ],
        [
          -83.8710175,
          10.3469578
        ]
      ]
    ]
  },
  "properties": {
    "theme": "base",
    "type": "land_use",
    "subtype": "recreation",
    "class": "pitch",
    "surface": "recreation_grass",
    "source_tags": {
      "leisure": "pitch",
      "sport": "soccer"
    },
    "names": {
      "primary": "Plaza Deportes Finca Tres"
    },
    "sources": [
      {
        "record_id": "w509487233@1",
        "property": "",
        "dataset": "OpenStreetMap"
      }
    ],
    "version": 0
  }
}
```

#### ttl
```ttl
@prefix geojson: <https://purl.org/geojson/vocab#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

<overture:land_use:example:1> a <file:///github/workspace/land_use>,
        geojson:Feature ;
    geojson:geometry [ a geojson:Polygon ;
            geojson:coordinates ( ( ( -8.387102e+01 1.034696e+01 ) ( -8.387009e+01 1.034702e+01 ) ( -8.387004e+01 1.034628e+01 ) ( -8.387097e+01 1.034622e+01 ) ( -8.387102e+01 1.034696e+01 ) ) ) ] .


```


### Example 7
#### json
```json
{
  "id": "OXOXOXOXOX",
  "type": "Feature",
  "geometry": {
    "type": "Polygon",
    "coordinates": [
      [
        [
          -91.8307764,
          43.7899936
        ],
        [
          -91.8309309,
          43.7901326
        ],
        [
          -91.8315202,
          43.7906232
        ],
        [
          -91.832079,
          43.7911798
        ],
        [
          -91.832577,
          43.7917638
        ],
        [
          -91.832839,
          43.7921615
        ],
        [
          -91.8307764,
          43.7899936
        ]
      ]
    ]
  },
  "properties": {
    "theme": "base",
    "type": "water",
    "subtype": "ocean",
    "class": "ocean",
    "names": {
      "primary": "Gulf of Gerdaus Mercator",
      "rules": [
        {
          "variant": "official",
          "perspectives": {
            "mode": "accepted_by",
            "countries": [
              "US"
            ]
          },
          "value": "Gulf of Cartographer's Tears"
        }
      ]
    },
    "source_tags": {
      "water": "ocean"
    },
    "sources": [
      {
        "record_id": "w1234567",
        "property": "",
        "dataset": "OpenStreetMap"
      }
    ],
    "is_salt": false,
    "is_intermittent": false,
    "version": 0
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/schema/context.jsonld",
  "id": "OXOXOXOXOX",
  "type": "Feature",
  "geometry": {
    "type": "Polygon",
    "coordinates": [
      [
        [
          -91.8307764,
          43.7899936
        ],
        [
          -91.8309309,
          43.7901326
        ],
        [
          -91.8315202,
          43.7906232
        ],
        [
          -91.832079,
          43.7911798
        ],
        [
          -91.832577,
          43.7917638
        ],
        [
          -91.832839,
          43.7921615
        ],
        [
          -91.8307764,
          43.7899936
        ]
      ]
    ]
  },
  "properties": {
    "theme": "base",
    "type": "water",
    "subtype": "ocean",
    "class": "ocean",
    "names": {
      "primary": "Gulf of Gerdaus Mercator",
      "rules": [
        {
          "variant": "official",
          "perspectives": {
            "mode": "accepted_by",
            "countries": [
              "US"
            ]
          },
          "value": "Gulf of Cartographer's Tears"
        }
      ]
    },
    "source_tags": {
      "water": "ocean"
    },
    "sources": [
      {
        "record_id": "w1234567",
        "property": "",
        "dataset": "OpenStreetMap"
      }
    ],
    "is_salt": false,
    "is_intermittent": false,
    "version": 0
  }
}
```

#### ttl
```ttl
@prefix geojson: <https://purl.org/geojson/vocab#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

<file:///github/workspace/OXOXOXOXOX> a <file:///github/workspace/water>,
        geojson:Feature ;
    geojson:geometry [ a geojson:Polygon ;
            geojson:coordinates ( ( ( -9.183078e+01 4.378999e+01 ) ( -9.183093e+01 4.379013e+01 ) ( -9.183152e+01 4.379062e+01 ) ( -9.183208e+01 4.379118e+01 ) ( -9.183258e+01 4.379176e+01 ) ( -9.183284e+01 4.379216e+01 ) ( -9.183078e+01 4.378999e+01 ) ) ) ] .


```


### Example 8
#### json
```json
{
  "id": "overture:buildings:building:1234",
  "type": "Feature",
  "geometry": {
    "type": "Polygon",
    "coordinates": [
      [
        [
          0,
          0
        ],
        [
          0,
          1
        ],
        [
          1,
          1
        ],
        [
          1,
          0
        ],
        [
          0,
          0
        ]
      ]
    ]
  },
  "properties": {
    "ext_foo": "I am a customer user property.",
    "ext_bar": "Me too!",
    "theme": "buildings",
    "type": "building",
    "version": 1,
    "sources": [
      {
        "dataset": "MyGreatDataset",
        "property": "/geometry",
        "update_time": "2024-04-26T23:55:01-08:00",
        "confidence": 0.3
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/schema/context.jsonld",
  "id": "overture:buildings:building:1234",
  "type": "Feature",
  "geometry": {
    "type": "Polygon",
    "coordinates": [
      [
        [
          0,
          0
        ],
        [
          0,
          1
        ],
        [
          1,
          1
        ],
        [
          1,
          0
        ],
        [
          0,
          0
        ]
      ]
    ]
  },
  "properties": {
    "ext_foo": "I am a customer user property.",
    "ext_bar": "Me too!",
    "theme": "buildings",
    "type": "building",
    "version": 1,
    "sources": [
      {
        "dataset": "MyGreatDataset",
        "property": "/geometry",
        "update_time": "2024-04-26T23:55:01-08:00",
        "confidence": 0.3
      }
    ]
  }
}
```

#### ttl
```ttl
@prefix geojson: <https://purl.org/geojson/vocab#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

<overture:buildings:building:1234> a <file:///github/workspace/building>,
        geojson:Feature ;
    geojson:geometry [ a geojson:Polygon ;
            geojson:coordinates ( ( ( 0 0 ) ( 0 1 ) ( 1 1 ) ( 1 0 ) ( 0 0 ) ) ) ] .


```


### Example 9
#### json
```json
{
  "id": "overture:buildings:part:1234",
  "type": "Feature",
  "geometry": {
    "type": "Polygon",
    "coordinates": [
      [
        [
          -77.036873,
          38.897804
        ],
        [
          -77.036873,
          38.897559
        ],
        [
          -77.03626,
          38.897559
        ],
        [
          -77.03626,
          38.897804
        ],
        [
          -77.036873,
          38.897804
        ]
      ]
    ]
  },
  "properties": {
    "ext_foo": "I am a customer user property.",
    "ext_bar": "Me too!",
    "theme": "buildings",
    "type": "building_part",
    "version": 1,
    "level": 1,
    "building_id": "abc123",
    "height": 21.34,
    "num_floors": 4,
    "min_height": 15.0,
    "min_floor": 2,
    "roof_shape": "dome",
    "roof_orientation": "across",
    "roof_direction": 23.4,
    "roof_height": 3.4,
    "sources": [
      {
        "property": "",
        "dataset": "microsoftMLBuildings"
      },
      {
        "property": "/properties/height",
        "dataset": "metaLidarExtractions"
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/schema/context.jsonld",
  "id": "overture:buildings:part:1234",
  "type": "Feature",
  "geometry": {
    "type": "Polygon",
    "coordinates": [
      [
        [
          -77.036873,
          38.897804
        ],
        [
          -77.036873,
          38.897559
        ],
        [
          -77.03626,
          38.897559
        ],
        [
          -77.03626,
          38.897804
        ],
        [
          -77.036873,
          38.897804
        ]
      ]
    ]
  },
  "properties": {
    "ext_foo": "I am a customer user property.",
    "ext_bar": "Me too!",
    "theme": "buildings",
    "type": "building_part",
    "version": 1,
    "level": 1,
    "building_id": "abc123",
    "height": 21.34,
    "num_floors": 4,
    "min_height": 15.0,
    "min_floor": 2,
    "roof_shape": "dome",
    "roof_orientation": "across",
    "roof_direction": 23.4,
    "roof_height": 3.4,
    "sources": [
      {
        "property": "",
        "dataset": "microsoftMLBuildings"
      },
      {
        "property": "/properties/height",
        "dataset": "metaLidarExtractions"
      }
    ]
  }
}
```

#### ttl
```ttl
@prefix geojson: <https://purl.org/geojson/vocab#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

<overture:buildings:part:1234> a <file:///github/workspace/building_part>,
        geojson:Feature ;
    geojson:geometry [ a geojson:Polygon ;
            geojson:coordinates ( ( ( -7.703687e+01 3.88978e+01 ) ( -7.703687e+01 3.889756e+01 ) ( -7.703626e+01 3.889756e+01 ) ( -7.703626e+01 3.88978e+01 ) ( -7.703687e+01 3.88978e+01 ) ) ) ] .


```


### Example 10
#### json
```json
{
  "id": "example:division_area:land:country:us",
  "type": "Feature",
  "geometry": {
    "type": "MultiPolygon",
    "coordinates": [
      [
        [
          [
            -170.6290015,
            25.3053671
          ],
          [
            -170.4076134,
            25.5082632
          ],
          [
            -170.6300336,
            25.7076006
          ],
          [
            -170.8506754,
            25.5056948
          ],
          [
            -170.6290015,
            25.3053671
          ]
        ]
      ],
      [
        [
          [
            -171.7380245,
            25.555318
          ],
          [
            -171.4949943,
            25.7747795
          ],
          [
            -171.726725,
            25.9865667
          ],
          [
            -171.9674222,
            25.7845748
          ],
          [
            -171.7380245,
            25.555318
          ]
        ]
      ],
      [
        [
          [
            -174.0155727,
            25.8411597
          ],
          [
            -173.7437151,
            26.0119599
          ],
          [
            -173.905507,
            26.2639004
          ],
          [
            -174.2280618,
            26.0816774
          ],
          [
            -174.0155727,
            25.8411597
          ]
        ]
      ],
      [
        [
          [
            -175.9506918,
            27.5543172
          ],
          [
            -175.5545765,
            27.7281369
          ],
          [
            -175.6295776,
            28.1237431
          ],
          [
            -176.1866168,
            27.9330153
          ],
          [
            -175.9506918,
            27.5543172
          ]
        ]
      ],
      [
        [
          [
            -166.1182936,
            23.4254685
          ],
          [
            -165.8702478,
            23.8636297
          ],
          [
            -166.3767961,
            24.0561939
          ],
          [
            -166.5303209,
            23.7815879
          ],
          [
            -166.1182936,
            23.4254685
          ]
        ]
      ],
      [
        [
          [
            -167.9975573,
            24.7968943
          ],
          [
            -167.778217,
            25.0023686
          ],
          [
            -168.005803,
            25.20088
          ],
          [
            -168.2206497,
            24.9967937
          ],
          [
            -167.9975573,
            24.7968943
          ]
        ]
      ],
      [
        [
          [
            -157.4082814,
            55.576068
          ],
          [
            -157.1024297,
            55.6733491
          ],
          [
            -157.0908436,
            55.8696588
          ],
          [
            -157.7232999,
            55.870247
          ],
          [
            -157.4082814,
            55.576068
          ]
        ]
      ],
      [
        [
          [
            -155.6071465,
            55.55087
          ],
          [
            -155.2980807,
            56.0385909
          ],
          [
            -156.1270413,
            55.9006965
          ],
          [
            -156.0182299,
            55.6525826
          ],
          [
            -155.6071465,
            55.55087
          ]
        ]
      ],
      [
        [
          [
            -178.3063127,
            28.1837783
          ],
          [
            -178.0577766,
            28.4309636
          ],
          [
            -178.3589518,
            28.655272
          ],
          [
            -178.60056,
            28.4012455
          ],
          [
            -178.3063127,
            28.1837783
          ]
        ]
      ],
      [
        [
          [
            -179.1390989,
            51.0070029
          ],
          [
            -173.0611771,
            51.8159234
          ],
          [
            -171.9740685,
            52.3514335
          ],
          [
            -178.9229631,
            52.0275532
          ],
          [
            -179.1390989,
            51.0070029
          ]
        ]
      ],
      [
        [
          [
            -180,
            51.7940888
          ],
          [
            -179.8836979,
            51.9764894
          ],
          [
            -180,
            52.138489
          ],
          [
            -180,
            51.8434509
          ],
          [
            -180,
            51.7940888
          ]
        ]
      ],
      [
        [
          [
            -170.3952428,
            56.8431693
          ],
          [
            -169.6956679,
            57.0307607
          ],
          [
            -169.5801239,
            57.2365744
          ],
          [
            -170.6525321,
            57.3494254
          ],
          [
            -170.3952428,
            56.8431693
          ]
        ]
      ],
      [
        [
          [
            -169.5771945,
            56.3323838
          ],
          [
            -169.1322924,
            56.6737641
          ],
          [
            -170.1288343,
            56.6777795
          ],
          [
            -170.0250438,
            56.4580184
          ],
          [
            -169.5771945,
            56.3323838
          ]
        ]
      ],
      [
        [
          [
            -168.0561273,
            64.76067
          ],
          [
            -167.5930406,
            65.0286657
          ],
          [
            -168.5591053,
            65.007885
          ],
          [
            -168.4482776,
            64.8327172
          ],
          [
            -168.0561273,
            64.76067
          ]
        ]
      ],
      [
        [
          [
            -156.6720152,
            20.3000654
          ],
          [
            -155.800111,
            20.8826396
          ],
          [
            -158.455088,
            21.6943824
          ],
          [
            -158.2462379,
            21.1430868
          ],
          [
            -156.6720152,
            20.3000654
          ]
        ]
      ],
      [
        [
          [
            -160.5398128,
            21.4482644
          ],
          [
            -159.3028431,
            21.7124132
          ],
          [
            -159.1241278,
            22.2798801
          ],
          [
            -160.2161715,
            22.1993854
          ],
          [
            -160.5398128,
            21.4482644
          ]
        ]
      ],
      [
        [
          [
            -161.9236658,
            22.8550496
          ],
          [
            -161.6972866,
            23.0665997
          ],
          [
            -161.9360903,
            23.2652845
          ],
          [
            -162.1455351,
            23.0568827
          ],
          [
            -161.9236658,
            22.8550496
          ]
        ]
      ],
      [
        [
          [
            -164.7000199,
            23.3734366
          ],
          [
            -164.4760626,
            23.575844
          ],
          [
            -164.7056774,
            23.7796906
          ],
          [
            -164.9238496,
            23.5726775
          ],
          [
            -164.7000199,
            23.3734366
          ]
        ]
      ],
      [
        [
          [
            -155.6810194,
            18.7091718
          ],
          [
            -154.595509,
            19.5434371
          ],
          [
            -155.877534,
            20.4681176
          ],
          [
            -156.2732568,
            19.7049213
          ],
          [
            -155.6810194,
            18.7091718
          ]
        ]
      ],
      [
        [
          [
            -82.8732511,
            24.4116731
          ],
          [
            -82.5948517,
            24.5902399
          ],
          [
            -82.7300073,
            24.8395704
          ],
          [
            -83.153058,
            24.6776636
          ],
          [
            -82.8732511,
            24.4116731
          ]
        ]
      ],
      [
        [
          [
            -81.8773353,
            24.2520071
          ],
          [
            -68.1545602,
            47.3251568
          ],
          [
            -82.6797222,
            41.6765556
          ],
          [
            -84.129,
            46.5305
          ],
          [
            -94.9573889,
            49.3701944
          ],
          [
            -125.0271096,
            48.4630615
          ],
          [
            -119.6795205,
            33.0665347
          ],
          [
            -97.40561,
            25.83764
          ],
          [
            -84.0549877,
            29.8627705
          ],
          [
            -81.8773353,
            24.2520071
          ]
        ]
      ],
      [
        [
          [
            179.2356588,
            51.1468561
          ],
          [
            178.6498473,
            52.169477
          ],
          [
            176.8813625,
            51.9348227
          ],
          [
            177.1853792,
            51.6303915
          ],
          [
            179.2356588,
            51.1468561
          ]
        ]
      ],
      [
        [
          [
            179.6302237,
            51.6862391
          ],
          [
            180,
            52.1384488
          ],
          [
            179.2193828,
            52.1042624
          ],
          [
            179.2227021,
            51.833522
          ],
          [
            179.6302237,
            51.6862391
          ]
        ]
      ],
      [
        [
          [
            175.915408,
            52.1325238
          ],
          [
            176.2623207,
            52.4572425
          ],
          [
            175.5671255,
            52.4969017
          ],
          [
            175.5586568,
            52.2829505
          ],
          [
            175.915408,
            52.1325238
          ]
        ]
      ],
      [
        [
          [
            173.6474085,
            52.1472948
          ],
          [
            174.8392132,
            52.6878183
          ],
          [
            172.1158739,
            52.9881155
          ],
          [
            173.132385,
            52.2506975
          ],
          [
            173.6474085,
            52.1472948
          ]
        ]
      ],
      [
        [
          [
            -146.3855284,
            59.1843829
          ],
          [
            -145.9234279,
            59.3169728
          ],
          [
            -145.8952803,
            59.5345003
          ],
          [
            -146.6535985,
            59.6545361
          ],
          [
            -146.3855284,
            59.1843829
          ]
        ]
      ],
      [
        [
          [
            -171.2797217,
            52.2444061
          ],
          [
            -145.9885379,
            60.1761058
          ],
          [
            -130.003485,
            56.008075
          ],
          [
            -141.00198,
            60.3063692
          ],
          [
            -140.7523256,
            69.8283004
          ],
          [
            -156.6515529,
            71.581159
          ],
          [
            -169.0485821,
            65.4690061
          ],
          [
            -161.2500247,
            63.8004626
          ],
          [
            -167.6542464,
            59.9434356
          ],
          [
            -158.0753114,
            57.7475562
          ],
          [
            -171.2797217,
            52.2444061
          ]
        ],
        [
          [
            -153.8125943,
            58.0958144
          ],
          [
            -153.5773523,
            58.3547948
          ],
          [
            -153.3559904,
            58.4231127
          ],
          [
            -153.6200524,
            58.260124
          ],
          [
            -153.8125943,
            58.0958144
          ]
        ],
        [
          [
            -153.1820044,
            58.5355625
          ],
          [
            -153.1751501,
            58.5480609
          ],
          [
            -153.1384992,
            58.5678286
          ],
          [
            -153.1470249,
            58.5552926
          ],
          [
            -153.1820044,
            58.5355625
          ]
        ],
        [
          [
            -152.8741566,
            58.7660471
          ],
          [
            -152.9882543,
            59.4696836
          ],
          [
            -152.1322999,
            60.0079718
          ],
          [
            -152.330171,
            59.1676267
          ],
          [
            -152.8741566,
            58.7660471
          ]
        ]
      ],
      [
        [
          [
            -172.7696055,
            59.9963072
          ],
          [
            -171.8272619,
            60.3517559
          ],
          [
            -173.4406927,
            60.7880772
          ],
          [
            -173.4413238,
            60.4223353
          ],
          [
            -172.7696055,
            59.9963072
          ]
        ]
      ],
      [
        [
          [
            -169.6463302,
            62.736964
          ],
          [
            -168.2509717,
            63.332816
          ],
          [
            -172.2753008,
            63.6094455
          ],
          [
            -172.0058757,
            63.2057208
          ],
          [
            -169.6463302,
            62.736964
          ]
        ]
      ]
    ]
  },
  "properties": {
    "theme": "divisions",
    "type": "division_area",
    "version": 0,
    "subtype": "country",
    "class": "land",
    "is_land": true,
    "is_territorial": false,
    "division_id": "example:division:country:us",
    "names": {
      "primary": "United States"
    },
    "country": "US"
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/schema/context.jsonld",
  "id": "example:division_area:land:country:us",
  "type": "Feature",
  "geometry": {
    "type": "MultiPolygon",
    "coordinates": [
      [
        [
          [
            -170.6290015,
            25.3053671
          ],
          [
            -170.4076134,
            25.5082632
          ],
          [
            -170.6300336,
            25.7076006
          ],
          [
            -170.8506754,
            25.5056948
          ],
          [
            -170.6290015,
            25.3053671
          ]
        ]
      ],
      [
        [
          [
            -171.7380245,
            25.555318
          ],
          [
            -171.4949943,
            25.7747795
          ],
          [
            -171.726725,
            25.9865667
          ],
          [
            -171.9674222,
            25.7845748
          ],
          [
            -171.7380245,
            25.555318
          ]
        ]
      ],
      [
        [
          [
            -174.0155727,
            25.8411597
          ],
          [
            -173.7437151,
            26.0119599
          ],
          [
            -173.905507,
            26.2639004
          ],
          [
            -174.2280618,
            26.0816774
          ],
          [
            -174.0155727,
            25.8411597
          ]
        ]
      ],
      [
        [
          [
            -175.9506918,
            27.5543172
          ],
          [
            -175.5545765,
            27.7281369
          ],
          [
            -175.6295776,
            28.1237431
          ],
          [
            -176.1866168,
            27.9330153
          ],
          [
            -175.9506918,
            27.5543172
          ]
        ]
      ],
      [
        [
          [
            -166.1182936,
            23.4254685
          ],
          [
            -165.8702478,
            23.8636297
          ],
          [
            -166.3767961,
            24.0561939
          ],
          [
            -166.5303209,
            23.7815879
          ],
          [
            -166.1182936,
            23.4254685
          ]
        ]
      ],
      [
        [
          [
            -167.9975573,
            24.7968943
          ],
          [
            -167.778217,
            25.0023686
          ],
          [
            -168.005803,
            25.20088
          ],
          [
            -168.2206497,
            24.9967937
          ],
          [
            -167.9975573,
            24.7968943
          ]
        ]
      ],
      [
        [
          [
            -157.4082814,
            55.576068
          ],
          [
            -157.1024297,
            55.6733491
          ],
          [
            -157.0908436,
            55.8696588
          ],
          [
            -157.7232999,
            55.870247
          ],
          [
            -157.4082814,
            55.576068
          ]
        ]
      ],
      [
        [
          [
            -155.6071465,
            55.55087
          ],
          [
            -155.2980807,
            56.0385909
          ],
          [
            -156.1270413,
            55.9006965
          ],
          [
            -156.0182299,
            55.6525826
          ],
          [
            -155.6071465,
            55.55087
          ]
        ]
      ],
      [
        [
          [
            -178.3063127,
            28.1837783
          ],
          [
            -178.0577766,
            28.4309636
          ],
          [
            -178.3589518,
            28.655272
          ],
          [
            -178.60056,
            28.4012455
          ],
          [
            -178.3063127,
            28.1837783
          ]
        ]
      ],
      [
        [
          [
            -179.1390989,
            51.0070029
          ],
          [
            -173.0611771,
            51.8159234
          ],
          [
            -171.9740685,
            52.3514335
          ],
          [
            -178.9229631,
            52.0275532
          ],
          [
            -179.1390989,
            51.0070029
          ]
        ]
      ],
      [
        [
          [
            -180,
            51.7940888
          ],
          [
            -179.8836979,
            51.9764894
          ],
          [
            -180,
            52.138489
          ],
          [
            -180,
            51.8434509
          ],
          [
            -180,
            51.7940888
          ]
        ]
      ],
      [
        [
          [
            -170.3952428,
            56.8431693
          ],
          [
            -169.6956679,
            57.0307607
          ],
          [
            -169.5801239,
            57.2365744
          ],
          [
            -170.6525321,
            57.3494254
          ],
          [
            -170.3952428,
            56.8431693
          ]
        ]
      ],
      [
        [
          [
            -169.5771945,
            56.3323838
          ],
          [
            -169.1322924,
            56.6737641
          ],
          [
            -170.1288343,
            56.6777795
          ],
          [
            -170.0250438,
            56.4580184
          ],
          [
            -169.5771945,
            56.3323838
          ]
        ]
      ],
      [
        [
          [
            -168.0561273,
            64.76067
          ],
          [
            -167.5930406,
            65.0286657
          ],
          [
            -168.5591053,
            65.007885
          ],
          [
            -168.4482776,
            64.8327172
          ],
          [
            -168.0561273,
            64.76067
          ]
        ]
      ],
      [
        [
          [
            -156.6720152,
            20.3000654
          ],
          [
            -155.800111,
            20.8826396
          ],
          [
            -158.455088,
            21.6943824
          ],
          [
            -158.2462379,
            21.1430868
          ],
          [
            -156.6720152,
            20.3000654
          ]
        ]
      ],
      [
        [
          [
            -160.5398128,
            21.4482644
          ],
          [
            -159.3028431,
            21.7124132
          ],
          [
            -159.1241278,
            22.2798801
          ],
          [
            -160.2161715,
            22.1993854
          ],
          [
            -160.5398128,
            21.4482644
          ]
        ]
      ],
      [
        [
          [
            -161.9236658,
            22.8550496
          ],
          [
            -161.6972866,
            23.0665997
          ],
          [
            -161.9360903,
            23.2652845
          ],
          [
            -162.1455351,
            23.0568827
          ],
          [
            -161.9236658,
            22.8550496
          ]
        ]
      ],
      [
        [
          [
            -164.7000199,
            23.3734366
          ],
          [
            -164.4760626,
            23.575844
          ],
          [
            -164.7056774,
            23.7796906
          ],
          [
            -164.9238496,
            23.5726775
          ],
          [
            -164.7000199,
            23.3734366
          ]
        ]
      ],
      [
        [
          [
            -155.6810194,
            18.7091718
          ],
          [
            -154.595509,
            19.5434371
          ],
          [
            -155.877534,
            20.4681176
          ],
          [
            -156.2732568,
            19.7049213
          ],
          [
            -155.6810194,
            18.7091718
          ]
        ]
      ],
      [
        [
          [
            -82.8732511,
            24.4116731
          ],
          [
            -82.5948517,
            24.5902399
          ],
          [
            -82.7300073,
            24.8395704
          ],
          [
            -83.153058,
            24.6776636
          ],
          [
            -82.8732511,
            24.4116731
          ]
        ]
      ],
      [
        [
          [
            -81.8773353,
            24.2520071
          ],
          [
            -68.1545602,
            47.3251568
          ],
          [
            -82.6797222,
            41.6765556
          ],
          [
            -84.129,
            46.5305
          ],
          [
            -94.9573889,
            49.3701944
          ],
          [
            -125.0271096,
            48.4630615
          ],
          [
            -119.6795205,
            33.0665347
          ],
          [
            -97.40561,
            25.83764
          ],
          [
            -84.0549877,
            29.8627705
          ],
          [
            -81.8773353,
            24.2520071
          ]
        ]
      ],
      [
        [
          [
            179.2356588,
            51.1468561
          ],
          [
            178.6498473,
            52.169477
          ],
          [
            176.8813625,
            51.9348227
          ],
          [
            177.1853792,
            51.6303915
          ],
          [
            179.2356588,
            51.1468561
          ]
        ]
      ],
      [
        [
          [
            179.6302237,
            51.6862391
          ],
          [
            180,
            52.1384488
          ],
          [
            179.2193828,
            52.1042624
          ],
          [
            179.2227021,
            51.833522
          ],
          [
            179.6302237,
            51.6862391
          ]
        ]
      ],
      [
        [
          [
            175.915408,
            52.1325238
          ],
          [
            176.2623207,
            52.4572425
          ],
          [
            175.5671255,
            52.4969017
          ],
          [
            175.5586568,
            52.2829505
          ],
          [
            175.915408,
            52.1325238
          ]
        ]
      ],
      [
        [
          [
            173.6474085,
            52.1472948
          ],
          [
            174.8392132,
            52.6878183
          ],
          [
            172.1158739,
            52.9881155
          ],
          [
            173.132385,
            52.2506975
          ],
          [
            173.6474085,
            52.1472948
          ]
        ]
      ],
      [
        [
          [
            -146.3855284,
            59.1843829
          ],
          [
            -145.9234279,
            59.3169728
          ],
          [
            -145.8952803,
            59.5345003
          ],
          [
            -146.6535985,
            59.6545361
          ],
          [
            -146.3855284,
            59.1843829
          ]
        ]
      ],
      [
        [
          [
            -171.2797217,
            52.2444061
          ],
          [
            -145.9885379,
            60.1761058
          ],
          [
            -130.003485,
            56.008075
          ],
          [
            -141.00198,
            60.3063692
          ],
          [
            -140.7523256,
            69.8283004
          ],
          [
            -156.6515529,
            71.581159
          ],
          [
            -169.0485821,
            65.4690061
          ],
          [
            -161.2500247,
            63.8004626
          ],
          [
            -167.6542464,
            59.9434356
          ],
          [
            -158.0753114,
            57.7475562
          ],
          [
            -171.2797217,
            52.2444061
          ]
        ],
        [
          [
            -153.8125943,
            58.0958144
          ],
          [
            -153.5773523,
            58.3547948
          ],
          [
            -153.3559904,
            58.4231127
          ],
          [
            -153.6200524,
            58.260124
          ],
          [
            -153.8125943,
            58.0958144
          ]
        ],
        [
          [
            -153.1820044,
            58.5355625
          ],
          [
            -153.1751501,
            58.5480609
          ],
          [
            -153.1384992,
            58.5678286
          ],
          [
            -153.1470249,
            58.5552926
          ],
          [
            -153.1820044,
            58.5355625
          ]
        ],
        [
          [
            -152.8741566,
            58.7660471
          ],
          [
            -152.9882543,
            59.4696836
          ],
          [
            -152.1322999,
            60.0079718
          ],
          [
            -152.330171,
            59.1676267
          ],
          [
            -152.8741566,
            58.7660471
          ]
        ]
      ],
      [
        [
          [
            -172.7696055,
            59.9963072
          ],
          [
            -171.8272619,
            60.3517559
          ],
          [
            -173.4406927,
            60.7880772
          ],
          [
            -173.4413238,
            60.4223353
          ],
          [
            -172.7696055,
            59.9963072
          ]
        ]
      ],
      [
        [
          [
            -169.6463302,
            62.736964
          ],
          [
            -168.2509717,
            63.332816
          ],
          [
            -172.2753008,
            63.6094455
          ],
          [
            -172.0058757,
            63.2057208
          ],
          [
            -169.6463302,
            62.736964
          ]
        ]
      ]
    ]
  },
  "properties": {
    "theme": "divisions",
    "type": "division_area",
    "version": 0,
    "subtype": "country",
    "class": "land",
    "is_land": true,
    "is_territorial": false,
    "division_id": "example:division:country:us",
    "names": {
      "primary": "United States"
    },
    "country": "US"
  }
}
```

#### ttl
```ttl
@prefix geojson: <https://purl.org/geojson/vocab#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

<example:division_area:land:country:us> a <file:///github/workspace/division_area>,
        geojson:Feature ;
    geojson:geometry [ a geojson:MultiPolygon ;
            geojson:coordinates ( ( ( ( -1.70629e+02 2.530537e+01 ) ( -1.704076e+02 2.550826e+01 ) ( -1.7063e+02 2.57076e+01 ) ( -1.708507e+02 2.550569e+01 ) ( -1.70629e+02 2.530537e+01 ) ) ) ( ( ( -1.71738e+02 2.555532e+01 ) ( -1.71495e+02 2.577478e+01 ) ( -1.717267e+02 2.598657e+01 ) ( -1.719674e+02 2.578457e+01 ) ( -1.71738e+02 2.555532e+01 ) ) ) ( ( ( -1.740156e+02 2.584116e+01 ) ( -1.737437e+02 2.601196e+01 ) ( -1.739055e+02 2.62639e+01 ) ( -1.742281e+02 2.608168e+01 ) ( -1.740156e+02 2.584116e+01 ) ) ) ( ( ( -1.759507e+02 2.755432e+01 ) ( -1.755546e+02 2.772814e+01 ) ( -1.756296e+02 2.812374e+01 ) ( -1.761866e+02 2.793302e+01 ) ( -1.759507e+02 2.755432e+01 ) ) ) ( ( ( -1.661183e+02 2.342547e+01 ) ( -1.658702e+02 2.386363e+01 ) ( -1.663768e+02 2.405619e+01 ) ( -1.665303e+02 2.378159e+01 ) ( -1.661183e+02 2.342547e+01 ) ) ) ( ( ( -1.679976e+02 2.479689e+01 ) ( -1.677782e+02 2.500237e+01 ) ( -1.680058e+02 2.520088e+01 ) ( -1.682206e+02 2.499679e+01 ) ( -1.679976e+02 2.479689e+01 ) ) ) ( ( ( -1.574083e+02 5.557607e+01 ) ( -1.571024e+02 5.567335e+01 ) ( -1.570908e+02 5.586966e+01 ) ( -1.577233e+02 5.587025e+01 ) ( -1.574083e+02 5.557607e+01 ) ) ) ( ( ( -1.556071e+02 5.555087e+01 ) ( -1.552981e+02 5.603859e+01 ) ( -1.56127e+02 5.59007e+01 ) ( -1.560182e+02 5.565258e+01 ) ( -1.556071e+02 5.555087e+01 ) ) ) ( ( ( -1.783063e+02 2.818378e+01 ) ( -1.780578e+02 2.843096e+01 ) ( -1.78359e+02 2.865527e+01 ) ( -1.786006e+02 2.840125e+01 ) ( -1.783063e+02 2.818378e+01 ) ) ) ( ( ( -1.791391e+02 5.1007e+01 ) ( -1.730612e+02 5.181592e+01 ) ( -1.719741e+02 5.235143e+01 ) ( -1.78923e+02 5.202755e+01 ) ( -1.791391e+02 5.1007e+01 ) ) ) ( ( ( -180 5.179409e+01 ) ( -1.798837e+02 5.197649e+01 ) ( -180 5.213849e+01 ) ( -180 5.184345e+01 ) ( -180 5.179409e+01 ) ) ) ( ( ( -1.703952e+02 5.684317e+01 ) ( -1.696957e+02 5.703076e+01 ) ( -1.695801e+02 5.723657e+01 ) ( -1.706525e+02 5.734943e+01 ) ( -1.703952e+02 5.684317e+01 ) ) ) ( ( ( -1.695772e+02 5.633238e+01 ) ( -1.691323e+02 5.667376e+01 ) ( -1.701288e+02 5.667778e+01 ) ( -1.70025e+02 5.645802e+01 ) ( -1.695772e+02 5.633238e+01 ) ) ) ( ( ( -1.680561e+02 6.476067e+01 ) ( -1.67593e+02 6.502867e+01 ) ( -1.685591e+02 6.500789e+01 ) ( -1.684483e+02 6.483272e+01 ) ( -1.680561e+02 6.476067e+01 ) ) ) ( ( ( -1.56672e+02 2.030007e+01 ) ( -1.558001e+02 2.088264e+01 ) ( -1.584551e+02 2.169438e+01 ) ( -1.582462e+02 2.114309e+01 ) ( -1.56672e+02 2.030007e+01 ) ) ) ( ( ( -1.605398e+02 2.144826e+01 ) ( -1.593028e+02 2.171241e+01 ) ( -1.591241e+02 2.227988e+01 ) ( -1.602162e+02 2.219939e+01 ) ( -1.605398e+02 2.144826e+01 ) ) ) ( ( ( -1.619237e+02 2.285505e+01 ) ( -1.616973e+02 2.30666e+01 ) ( -1.619361e+02 2.326528e+01 ) ( -1.621455e+02 2.305688e+01 ) ( -1.619237e+02 2.285505e+01 ) ) ) ( ( ( -1.647e+02 2.337344e+01 ) ( -1.644761e+02 2.357584e+01 ) ( -1.647057e+02 2.377969e+01 ) ( -1.649238e+02 2.357268e+01 ) ( -1.647e+02 2.337344e+01 ) ) ) ( ( ( -1.55681e+02 1.870917e+01 ) ( -1.545955e+02 1.954344e+01 ) ( -1.558775e+02 2.046812e+01 ) ( -1.562733e+02 1.970492e+01 ) ( -1.55681e+02 1.870917e+01 ) ) ) ( ( ( -8.287325e+01 2.441167e+01 ) ( -8.259485e+01 2.459024e+01 ) ( -8.273001e+01 2.483957e+01 ) ( -8.315306e+01 2.467766e+01 ) ( -8.287325e+01 2.441167e+01 ) ) ) ( ( ( -8.187734e+01 2.425201e+01 ) ( -6.815456e+01 4.732516e+01 ) ( -8.267972e+01 4.167656e+01 ) ( -8.4129e+01 4.65305e+01 ) ( -9.495739e+01 4.937019e+01 ) ( -1.250271e+02 4.846306e+01 ) ( -1.196795e+02 3.306653e+01 ) ( -9.740561e+01 2.583764e+01 ) ( -8.405499e+01 2.986277e+01 ) ( -8.187734e+01 2.425201e+01 ) ) ) ( ( ( 1.792357e+02 5.114686e+01 ) ( 1.786498e+02 5.216948e+01 ) ( 1.768814e+02 5.193482e+01 ) ( 1.771854e+02 5.163039e+01 ) ( 1.792357e+02 5.114686e+01 ) ) ) ( ( ( 1.796302e+02 5.168624e+01 ) ( 180 5.213845e+01 ) ( 1.792194e+02 5.210426e+01 ) ( 1.792227e+02 5.183352e+01 ) ( 1.796302e+02 5.168624e+01 ) ) ) ( ( ( 1.759154e+02 5.213252e+01 ) ( 1.762623e+02 5.245724e+01 ) ( 1.755671e+02 5.24969e+01 ) ( 1.755587e+02 5.228295e+01 ) ( 1.759154e+02 5.213252e+01 ) ) ) ( ( ( 1.736474e+02 5.214729e+01 ) ( 1.748392e+02 5.268782e+01 ) ( 1.721159e+02 5.298812e+01 ) ( 1.731324e+02 5.22507e+01 ) ( 1.736474e+02 5.214729e+01 ) ) ) ( ( ( -1.463855e+02 5.918438e+01 ) ( -1.459234e+02 5.931697e+01 ) ( -1.458953e+02 5.95345e+01 ) ( -1.466536e+02 5.965454e+01 ) ( -1.463855e+02 5.918438e+01 ) ) ) ( ( ( -1.712797e+02 5.224441e+01 ) ( -1.459885e+02 6.017611e+01 ) ( -1.300035e+02 5.600807e+01 ) ( -1.41002e+02 6.030637e+01 ) ( -1.407523e+02 6.98283e+01 ) ( -1.566516e+02 7.158116e+01 ) ( -1.690486e+02 6.546901e+01 ) ( -1.6125e+02 6.380046e+01 ) ( -1.676542e+02 5.994344e+01 ) ( -1.580753e+02 5.774756e+01 ) ( -1.712797e+02 5.224441e+01 ) ) ( ( -1.538126e+02 5.809581e+01 ) ( -1.535774e+02 5.835479e+01 ) ( -1.53356e+02 5.842311e+01 ) ( -1.536201e+02 5.826012e+01 ) ( -1.538126e+02 5.809581e+01 ) ) ( ( -1.53182e+02 5.853556e+01 ) ( -1.531752e+02 5.854806e+01 ) ( -1.531385e+02 5.856783e+01 ) ( -1.53147e+02 5.855529e+01 ) ( -1.53182e+02 5.853556e+01 ) ) ( ( -1.528742e+02 5.876605e+01 ) ( -1.529883e+02 5.946968e+01 ) ( -1.521323e+02 6.000797e+01 ) ( -1.523302e+02 5.916763e+01 ) ( -1.528742e+02 5.876605e+01 ) ) ) ( ( ( -1.727696e+02 5.999631e+01 ) ( -1.718273e+02 6.035176e+01 ) ( -1.734407e+02 6.078808e+01 ) ( -1.734413e+02 6.042234e+01 ) ( -1.727696e+02 5.999631e+01 ) ) ) ( ( ( -1.696463e+02 6.273696e+01 ) ( -1.68251e+02 6.333282e+01 ) ( -1.722753e+02 6.360945e+01 ) ( -1.720059e+02 6.320572e+01 ) ( -1.696463e+02 6.273696e+01 ) ) ) ) ] .


```


### Example 11
#### json
```json
{
  "id": "example:division_boundary:disputed_both",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        0,
        1
      ],
      [
        1,
        2
      ]
    ]
  },
  "properties": {
    "theme": "divisions",
    "type": "division_boundary",
    "version": 1,
    "subtype": "country",
    "class": "land",
    "is_land": true,
    "is_territorial": false,
    "division_ids": [
      "example:division:country:left",
      "example:division:country:right"
    ],
    "is_disputed": true,
    "perspectives": {
      "mode": "disputed_by",
      "countries": [
        "XX"
      ]
    }
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/schema/context.jsonld",
  "id": "example:division_boundary:disputed_both",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        0,
        1
      ],
      [
        1,
        2
      ]
    ]
  },
  "properties": {
    "theme": "divisions",
    "type": "division_boundary",
    "version": 1,
    "subtype": "country",
    "class": "land",
    "is_land": true,
    "is_territorial": false,
    "division_ids": [
      "example:division:country:left",
      "example:division:country:right"
    ],
    "is_disputed": true,
    "perspectives": {
      "mode": "disputed_by",
      "countries": [
        "XX"
      ]
    }
  }
}
```

#### ttl
```ttl
@prefix geojson: <https://purl.org/geojson/vocab#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

<example:division_boundary:disputed_both> a <file:///github/workspace/division_boundary>,
        geojson:Feature ;
    geojson:geometry [ a geojson:LineString ;
            geojson:coordinates ( ( 0 1 ) ( 1 2 ) ) ] .


```


### Example 12
#### json
```json
{
  "id": "example:division:locality:lj",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      14.5845,
      46.057
    ]
  },
  "properties": {
    "theme": "divisions",
    "type": "division",
    "version": 0,
    "subtype": "locality",
    "local_type": {
      "en": "city"
    },
    "names": {
      "primary": "Ljubljana"
    },
    "sources": [
      {
        "property": "",
        "dataset": "OpenStreetMap",
        "record_id": "N6968827.V76"
      }
    ],
    "country": "SI",
    "hierarchies": [
      [
        {
          "division_id": "example:division:country:si",
          "subtype": "country",
          "name": "Slovenia"
        }
      ]
    ],
    "capital_of_divisions": [
      {
        "division_id": "example:division:country:si",
        "subtype": "country"
      }
    ],
    "parent_division_id": "example:division:country:si",
    "population": 335509
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/schema/context.jsonld",
  "id": "example:division:locality:lj",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      14.5845,
      46.057
    ]
  },
  "properties": {
    "theme": "divisions",
    "type": "division",
    "version": 0,
    "subtype": "locality",
    "local_type": {
      "en": "city"
    },
    "names": {
      "primary": "Ljubljana"
    },
    "sources": [
      {
        "property": "",
        "dataset": "OpenStreetMap",
        "record_id": "N6968827.V76"
      }
    ],
    "country": "SI",
    "hierarchies": [
      [
        {
          "division_id": "example:division:country:si",
          "subtype": "country",
          "name": "Slovenia"
        }
      ]
    ],
    "capital_of_divisions": [
      {
        "division_id": "example:division:country:si",
        "subtype": "country"
      }
    ],
    "parent_division_id": "example:division:country:si",
    "population": 335509
  }
}
```

#### ttl
```ttl
@prefix geojson: <https://purl.org/geojson/vocab#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

<example:division:locality:lj> a <file:///github/workspace/division>,
        geojson:Feature ;
    geojson:geometry [ a geojson:Point ;
            geojson:coordinates ( 1.45845e+01 4.6057e+01 ) ] .


```


### Example 13
#### json
```json
{
  "id": "timestamp-utc",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      0,
      0
    ]
  },
  "properties": {
    "categories": {
      "primary": "some_category"
    },
    "theme": "places",
    "type": "place",
    "version": 1,
    "operating_status": "open"
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/schema/context.jsonld",
  "id": "timestamp-utc",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      0,
      0
    ]
  },
  "properties": {
    "categories": {
      "primary": "some_category"
    },
    "theme": "places",
    "type": "place",
    "version": 1,
    "operating_status": "open"
  }
}
```

#### ttl
```ttl
@prefix geojson: <https://purl.org/geojson/vocab#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

<file:///github/workspace/timestamp-utc> a <file:///github/workspace/place>,
        geojson:Feature ;
    geojson:geometry [ a geojson:Point ;
            geojson:coordinates ( 0 0 ) ] .


```


### Example 14
#### json
```json
{
  "id": "timestamp-with-tz-offset",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      0,
      0
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "connector",
    "version": 0
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/schema/context.jsonld",
  "id": "timestamp-with-tz-offset",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      0,
      0
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "connector",
    "version": 0
  }
}
```

#### ttl
```ttl
@prefix geojson: <https://purl.org/geojson/vocab#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

<file:///github/workspace/timestamp-with-tz-offset> a <file:///github/workspace/connector>,
        geojson:Feature ;
    geojson:geometry [ a geojson:Point ;
            geojson:coordinates ( 0 0 ) ] .


```


### Example 15
#### json
```json
{
  "id": "names-lexically-valid-language-tag",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        0,
        0
      ],
      [
        1,
        1
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "primary",
    "names": {
      "primary": "foo",
      "common": {
        "nan-POJ": "Lexically valid, but should be corrected to nan-Latn",
        "nan-Latn": "This is fine.",
        "ja-kana": "Use this instead of ja_kana.",
        "zh-Latn-pinyin": "Use this instead of zh_pinyin.",
        "zh-Bopo": "Use this instead of zh_zhuyin."
      },
      "rules": [
        {
          "language": "be-Latn",
          "value": "Use this instead of be-tarask.",
          "variant": "common"
        },
        {
          "language": "ja-Latn",
          "value": "Use this instead of ja_rm.",
          "variant": "alternate"
        }
      ]
    }
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/schema/context.jsonld",
  "id": "names-lexically-valid-language-tag",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        0,
        0
      ],
      [
        1,
        1
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "primary",
    "names": {
      "primary": "foo",
      "common": {
        "nan-POJ": "Lexically valid, but should be corrected to nan-Latn",
        "nan-Latn": "This is fine.",
        "ja-kana": "Use this instead of ja_kana.",
        "zh-Latn-pinyin": "Use this instead of zh_pinyin.",
        "zh-Bopo": "Use this instead of zh_zhuyin."
      },
      "rules": [
        {
          "language": "be-Latn",
          "value": "Use this instead of be-tarask.",
          "variant": "common"
        },
        {
          "language": "ja-Latn",
          "value": "Use this instead of ja_rm.",
          "variant": "alternate"
        }
      ]
    }
  }
}
```

#### ttl
```ttl
@prefix geojson: <https://purl.org/geojson/vocab#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

<file:///github/workspace/names-lexically-valid-language-tag> a <file:///github/workspace/segment>,
        geojson:Feature ;
    geojson:geometry [ a geojson:LineString ;
            geojson:coordinates ( ( 0 0 ) ( 1 1 ) ) ] .


```

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
title: Overture Maps Schema
description: A JSON Schema for the canonical GeoJSON form of Overture Maps Features.
type: object
unevaluatedProperties: false
allOf:
- $ref: https://opengeospatial.github.io/bblocks/annotated-schemas/geo/common/data_types/geojson/schema.yaml
  $comment: Every Overture feature IS A GeoJSON feature
oneOf:
- $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/addresses/address/schema.yaml
- $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/base/bathymetry/schema.yaml
- $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/base/infrastructure/schema.yaml
- $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/base/land/schema.yaml
- $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/base/land_cover/schema.yaml
- $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/base/land_use/schema.yaml
- $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/base/water/schema.yaml
- $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/buildings/building/schema.yaml
- $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/buildings/building_part/schema.yaml
- $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/divisions/division_boundary/schema.yaml
- $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/divisions/division/schema.yaml
- $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/divisions/division_area/schema.yaml
- $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/places/place/schema.yaml
- $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/connector/schema.yaml
- $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/schema.yaml

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/schema/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/schema/schema.yaml)


# JSON-LD Context

```jsonld
{
  "@context": {
    "Feature": "geojson:Feature",
    "FeatureCollection": "geojson:FeatureCollection",
    "GeometryCollection": "geojson:GeometryCollection",
    "LineString": "geojson:LineString",
    "MultiLineString": "geojson:MultiLineString",
    "MultiPoint": "geojson:MultiPoint",
    "MultiPolygon": "geojson:MultiPolygon",
    "Point": "geojson:Point",
    "Polygon": "geojson:Polygon",
    "features": {
      "@container": "@set",
      "@id": "geojson:features"
    },
    "type": "@type",
    "id": "@id",
    "properties": "@nest",
    "geometry": {
      "@context": {
        "coordinates": {
          "@container": "@list",
          "@id": "geojson:coordinates"
        }
      },
      "@id": "geojson:geometry"
    },
    "bbox": {
      "@container": "@list",
      "@id": "geojson:bbox"
    },
    "geojson": "https://purl.org/geojson/vocab#",
    "@version": 1.1
  }
}
```

You can find the full JSON-LD context here:
[context.jsonld](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/schema/context.jsonld)


# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-overturemaps](https://github.com/ogcincubator/bblocks-overturemaps)
* Path: `_sources/schemas/schema`

