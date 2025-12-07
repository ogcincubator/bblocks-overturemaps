
# Transportation Segment schema (Schema)

`ogc.overturemaps.schemas.transportation.segment` *v0.1*

Segments are paths which can be traveled by people or things. Segments are compatible with GeoJSON LineString features.

[*Status*](http://www.opengis.net/def/status): Under development

## Examples

### Example 1
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
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
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


```


### Example 2
#### json
```json
{
  "id": "timestamp-leap-second",
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
    "subtype": "road",
    "class": "primary",
    "version": 1
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "timestamp-leap-second",
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
    "subtype": "road",
    "class": "primary",
    "version": 1
  }
}
```

#### ttl
```ttl


```


### Example 3
#### json
```json
{
  "id": "access-restrictions-segment-blanket",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        0,
        0
      ],
      [
        0,
        1
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "residential",
    "access_restrictions": [
      {
        "access_type": "denied"
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "access-restrictions-segment-blanket",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        0,
        0
      ],
      [
        0,
        1
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "residential",
    "access_restrictions": [
      {
        "access_type": "denied"
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 4
#### json
```json
{
  "id": "access-restrictions-segment-private-with-deliveries",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        0,
        0
      ],
      [
        0,
        1
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "residential",
    "access_restrictions": [
      {
        "access_type": "denied"
      },
      {
        "access_type": "allowed",
        "when": {
          "recognized": [
            "as_private"
          ]
        }
      },
      {
        "access_type": "allowed",
        "when": {
          "using": [
            "to_deliver"
          ],
          "during": "Mo-Fr 08:30-16:30"
        }
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "access-restrictions-segment-private-with-deliveries",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        0,
        0
      ],
      [
        0,
        1
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "residential",
    "access_restrictions": [
      {
        "access_type": "denied"
      },
      {
        "access_type": "allowed",
        "when": {
          "recognized": [
            "as_private"
          ]
        }
      },
      {
        "access_type": "allowed",
        "when": {
          "using": [
            "to_deliver"
          ],
          "during": "Mo-Fr 08:30-16:30"
        }
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 5
#### json
```json
{
  "id": "access-restrictions-segment-motor-vehicles-destination-only",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        0,
        0
      ],
      [
        0,
        1
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "residential",
    "access_restrictions": [
      {
        "access_type": "denied",
        "when": {
          "mode": [
            "motor_vehicle"
          ]
        }
      },
      {
        "access_type": "allowed",
        "when": {
          "using": [
            "at_destination"
          ]
        }
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "access-restrictions-segment-motor-vehicles-destination-only",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        0,
        0
      ],
      [
        0,
        1
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "residential",
    "access_restrictions": [
      {
        "access_type": "denied",
        "when": {
          "mode": [
            "motor_vehicle"
          ]
        }
      },
      {
        "access_type": "allowed",
        "when": {
          "using": [
            "at_destination"
          ]
        }
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 6
#### json
```json
{
  "id": "access-restrictions-segment-axle-limit",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        0,
        0
      ],
      [
        0,
        1
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "motorway",
    "access_restrictions": [
      {
        "access_type": "denied",
        "when": {
          "mode": [
            "hgv"
          ],
          "vehicle": [
            {
              "dimension": "axle_count",
              "comparison": "greater_than_equal",
              "value": 5
            }
          ]
        }
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "access-restrictions-segment-axle-limit",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        0,
        0
      ],
      [
        0,
        1
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "motorway",
    "access_restrictions": [
      {
        "access_type": "denied",
        "when": {
          "mode": [
            "hgv"
          ],
          "vehicle": [
            {
              "dimension": "axle_count",
              "comparison": "greater_than_equal",
              "value": 5
            }
          ]
        }
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 7
#### json
```json
{
  "id": "overture:transportation:example:simple-road1",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -122.152944,
        47.629681
      ],
      [
        -122.152916,
        47.629686
      ],
      [
        -122.152501,
        47.62977
      ],
      [
        -122.152188,
        47.62984
      ],
      [
        -122.151813,
        47.629934
      ],
      [
        -122.151747,
        47.629952
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 4,
    "subtype": "road",
    "class": "motorway",
    "connectors": [
      {
        "connector_id": "fooConnector",
        "at": 0
      },
      {
        "connector_id": "barConnector",
        "at": 1
      }
    ],
    "names": {
      "primary": "SR 520"
    },
    "access_restrictions": [
      {
        "access_type": "denied",
        "when": {
          "mode": [
            "foot"
          ]
        }
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:example:simple-road1",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -122.152944,
        47.629681
      ],
      [
        -122.152916,
        47.629686
      ],
      [
        -122.152501,
        47.62977
      ],
      [
        -122.152188,
        47.62984
      ],
      [
        -122.151813,
        47.629934
      ],
      [
        -122.151747,
        47.629952
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 4,
    "subtype": "road",
    "class": "motorway",
    "connectors": [
      {
        "connector_id": "fooConnector",
        "at": 0
      },
      {
        "connector_id": "barConnector",
        "at": 1
      }
    ],
    "names": {
      "primary": "SR 520"
    },
    "access_restrictions": [
      {
        "access_type": "denied",
        "when": {
          "mode": [
            "foot"
          ]
        }
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 8
#### json
```json
{
  "id": "overture:transportation:example:geometric-scoping",
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
    "speed_limits": [
      {
        "between": [
          0,
          0.15
        ],
        "max_speed": {
          "value": 100,
          "unit": "km/h"
        }
      },
      {
        "between": [
          0.15,
          1
        ],
        "max_speed": {
          "value": 60,
          "unit": "km/h"
        }
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:example:geometric-scoping",
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
    "speed_limits": [
      {
        "between": [
          0,
          0.15
        ],
        "max_speed": {
          "value": 100,
          "unit": "km/h"
        }
      },
      {
        "between": [
          0.15,
          1
        ],
        "max_speed": {
          "value": 60,
          "unit": "km/h"
        }
      }
    ]
  }
}
```

#### ttl
```ttl
@prefix om: <https://w3id.org/ogc/om/> .
@prefix qudt: <http://qudt.org/schema/qudt/> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

[] om:hasSpeedLimit [ om:hasMaxSpeed [ qudt:hasUnit "km/h" ;
                    rdf:value 100 ] ],
        [ om:hasMaxSpeed [ qudt:hasUnit "km/h" ;
                    rdf:value 60 ] ] .


```


### Example 9
#### json
```json
{
  "id": "overture:transportation:example:simple-road",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -123.13538016118466,
        49.28584368472093
      ],
      [
        -123.13430200328841,
        49.28656927229528
      ],
      [
        -123.13325122717998,
        49.28727252390803
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 5,
    "subtype": "road",
    "class": "residential",
    "connectors": [
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector1",
        "at": 0
      },
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector2",
        "at": 1
      }
    ],
    "names": {
      "primary": "Nicola Street"
    },
    "road_surface": [
      {
        "value": "paved"
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:example:simple-road",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -123.13538016118466,
        49.28584368472093
      ],
      [
        -123.13430200328841,
        49.28656927229528
      ],
      [
        -123.13325122717998,
        49.28727252390803
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 5,
    "subtype": "road",
    "class": "residential",
    "connectors": [
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector1",
        "at": 0
      },
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector2",
        "at": 1
      }
    ],
    "names": {
      "primary": "Nicola Street"
    },
    "road_surface": [
      {
        "value": "paved"
      }
    ]
  }
}
```

#### ttl
```ttl
@prefix ns1: <osm:> .

[] ns1:hasSurfaceType <https://w3id.org/ogc/om/surfaces/paved> .


```


### Example 10
#### json
```json
{
  "id": "speed-limits-simple",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -123.09348187774302,
        49.280278741717865
      ],
      [
        -123.0895720621171,
        49.280195795155265
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "residential",
    "speed_limits": [
      {
        "max_speed": {
          "value": 30,
          "unit": "km/h"
        }
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "speed-limits-simple",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -123.09348187774302,
        49.280278741717865
      ],
      [
        -123.0895720621171,
        49.280195795155265
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "residential",
    "speed_limits": [
      {
        "max_speed": {
          "value": 30,
          "unit": "km/h"
        }
      }
    ]
  }
}
```

#### ttl
```ttl
@prefix om: <https://w3id.org/ogc/om/> .
@prefix qudt: <http://qudt.org/schema/qudt/> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

[] om:hasSpeedLimit [ om:hasMaxSpeed [ qudt:hasUnit "km/h" ;
                    rdf:value 30 ] ] .


```


### Example 11
#### json
```json
{
  "id": "speed-limits-variable-max",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        0,
        0
      ],
      [
        0,
        1
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 2,
    "subtype": "road",
    "class": "secondary",
    "speed_limits": [
      {
        "max_speed": {
          "value": 70,
          "unit": "mph"
        }
      },
      {
        "when": {
          "mode": [
            "hgv"
          ],
          "heading": "forward"
        },
        "max_speed": {
          "value": 65,
          "unit": "mph"
        }
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "speed-limits-variable-max",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        0,
        0
      ],
      [
        0,
        1
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 2,
    "subtype": "road",
    "class": "secondary",
    "speed_limits": [
      {
        "max_speed": {
          "value": 70,
          "unit": "mph"
        }
      },
      {
        "when": {
          "mode": [
            "hgv"
          ],
          "heading": "forward"
        },
        "max_speed": {
          "value": 65,
          "unit": "mph"
        }
      }
    ]
  }
}
```

#### ttl
```ttl
@prefix om: <https://w3id.org/ogc/om/> .
@prefix qudt: <http://qudt.org/schema/qudt/> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

[] om:hasSpeedLimit [ om:hasMaxSpeed [ qudt:hasUnit "mph" ;
                    rdf:value 65 ] ;
            om:when "{\"heading\":\"forward\",\"mode\":[\"hgv\"]}"^^rdf:JSON ],
        [ om:hasMaxSpeed [ qudt:hasUnit "mph" ;
                    rdf:value 70 ] ] .


```


### Example 12
#### json
```json
{
  "id": "speed-limits-variable-max",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -123.12895930023527,
        50.007761789070344
      ],
      [
        -123.12637500433082,
        50.00945836227345
      ],
      [
        -123.12506896231434,
        50.011762034223324
      ],
      [
        -123.12415195409014,
        50.01351203677902
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "motorway",
    "speed_limits": [
      {
        "max_speed": {
          "value": 100,
          "unit": "km/h"
        },
        "is_max_speed_variable": true
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "speed-limits-variable-max",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -123.12895930023527,
        50.007761789070344
      ],
      [
        -123.12637500433082,
        50.00945836227345
      ],
      [
        -123.12506896231434,
        50.011762034223324
      ],
      [
        -123.12415195409014,
        50.01351203677902
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "motorway",
    "speed_limits": [
      {
        "max_speed": {
          "value": 100,
          "unit": "km/h"
        },
        "is_max_speed_variable": true
      }
    ]
  }
}
```

#### ttl
```ttl
@prefix om: <https://w3id.org/ogc/om/> .
@prefix qudt: <http://qudt.org/schema/qudt/> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

[] om:hasSpeedLimit [ om:hasMaxSpeed [ qudt:hasUnit "km/h" ;
                    rdf:value 100 ] ;
            om:isMaxSpeedVariable true ] .


```


### Example 13
#### json
```json
{
  "id": "overture:transportation:example:subjective-heading-scoping",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -1.3023158,
        54.5579329
      ],
      [
        -1.302009,
        54.5577898
      ],
      [
        -1.3014511,
        54.5575155
      ],
      [
        -1.3009618,
        54.5572737
      ],
      [
        -1.3004518,
        54.5570288
      ],
      [
        -1.3003009,
        54.556958
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 2,
    "subtype": "road",
    "class": "primary",
    "access_restrictions": [
      {
        "access_type": "denied",
        "when": {
          "heading": "backward"
        }
      },
      {
        "access_type": "allowed",
        "when": {
          "heading": "backward",
          "mode": [
            "bus"
          ]
        }
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:example:subjective-heading-scoping",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -1.3023158,
        54.5579329
      ],
      [
        -1.302009,
        54.5577898
      ],
      [
        -1.3014511,
        54.5575155
      ],
      [
        -1.3009618,
        54.5572737
      ],
      [
        -1.3004518,
        54.5570288
      ],
      [
        -1.3003009,
        54.556958
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 2,
    "subtype": "road",
    "class": "primary",
    "access_restrictions": [
      {
        "access_type": "denied",
        "when": {
          "heading": "backward"
        }
      },
      {
        "access_type": "allowed",
        "when": {
          "heading": "backward",
          "mode": [
            "bus"
          ]
        }
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 14
#### json
```json
{
  "id": "overture:transportation:example:subjective-status-scoping",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -123.12791513926058,
        49.287502049554945
      ],
      [
        -123.12795068403449,
        49.287522915661725
      ],
      [
        -123.12797769806272,
        49.28756882106529
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "tertiary",
    "access_restrictions": [
      {
        "access_type": "denied"
      },
      {
        "access_type": "allowed",
        "when": {
          "recognized": [
            "as_private"
          ]
        }
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:example:subjective-status-scoping",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -123.12791513926058,
        49.287502049554945
      ],
      [
        -123.12795068403449,
        49.287522915661725
      ],
      [
        -123.12797769806272,
        49.28756882106529
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "tertiary",
    "access_restrictions": [
      {
        "access_type": "denied"
      },
      {
        "access_type": "allowed",
        "when": {
          "recognized": [
            "as_private"
          ]
        }
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 15
#### json
```json
{
  "id": "overture:transportation:example:subjective-usage-purpose-scoping",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -123.12700676422021,
        49.279826628301635
      ],
      [
        -123.12680748254229,
        49.27995121574301
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "tertiary",
    "access_restrictions": [
      {
        "access_type": "denied"
      },
      {
        "access_type": "allowed",
        "when": {
          "using": [
            "as_customer",
            "at_destination"
          ]
        }
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:example:subjective-usage-purpose-scoping",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -123.12700676422021,
        49.279826628301635
      ],
      [
        -123.12680748254229,
        49.27995121574301
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "tertiary",
    "access_restrictions": [
      {
        "access_type": "denied"
      },
      {
        "access_type": "allowed",
        "when": {
          "using": [
            "as_customer",
            "at_destination"
          ]
        }
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 16
#### json
```json
{
  "id": "overture:transportation:example:subjective-vehicle-attributes-scoping",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -123.12791513926058,
        49.287502049554945
      ],
      [
        -123.12795068403449,
        49.287522915661725
      ],
      [
        -123.12797769806272,
        49.28756882106529
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "residential",
    "access_restrictions": [
      {
        "access_type": "denied",
        "when": {
          "vehicle": [
            {
              "dimension": "weight",
              "comparison": "greater_than",
              "value": 23,
              "unit": "t"
            }
          ]
        }
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:example:subjective-vehicle-attributes-scoping",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -123.12791513926058,
        49.287502049554945
      ],
      [
        -123.12795068403449,
        49.287522915661725
      ],
      [
        -123.12797769806272,
        49.28756882106529
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "residential",
    "access_restrictions": [
      {
        "access_type": "denied",
        "when": {
          "vehicle": [
            {
              "dimension": "weight",
              "comparison": "greater_than",
              "value": 23,
              "unit": "t"
            }
          ]
        }
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 17
#### json
```json
{
  "id": "overture:transportation:example:temporal-scoping",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -122.90019762265949,
        49.20784664905824
      ],
      [
        -122.9003738558948,
        49.207833436710956
      ],
      [
        -122.90052986564378,
        49.207871186265805
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 2,
    "subtype": "road",
    "class": "unknown",
    "access_restrictions": [
      {
        "access_type": "denied",
        "when": {
          "mode": [
            "bus"
          ],
          "during": "Mo-Fr 15:00-18:00"
        }
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:example:temporal-scoping",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -122.90019762265949,
        49.20784664905824
      ],
      [
        -122.9003738558948,
        49.207833436710956
      ],
      [
        -122.90052986564378,
        49.207871186265805
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 2,
    "subtype": "road",
    "class": "unknown",
    "access_restrictions": [
      {
        "access_type": "denied",
        "when": {
          "mode": [
            "bus"
          ],
          "during": "Mo-Fr 15:00-18:00"
        }
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 18
#### json
```json
{
  "id": "overture:transportation:example:simple-turn-restriction-exit",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -113.57831482025354,
        50.018860947117304
      ],
      [
        -113.5783121688577,
        50.019016827708754
      ],
      [
        -113.57829228338763,
        50.019079861246865
      ],
      [
        -113.57826444373009,
        50.019121599625294
      ],
      [
        -113.57816369068271,
        50.01919400284882
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "secondary",
    "connectors": [
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector1",
        "at": 0
      },
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector2",
        "at": 1
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:example:simple-turn-restriction-exit",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -113.57831482025354,
        50.018860947117304
      ],
      [
        -113.5783121688577,
        50.019016827708754
      ],
      [
        -113.57829228338763,
        50.019079861246865
      ],
      [
        -113.57826444373009,
        50.019121599625294
      ],
      [
        -113.57816369068271,
        50.01919400284882
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "secondary",
    "connectors": [
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector1",
        "at": 0
      },
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector2",
        "at": 1
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 19
#### json
```json
{
  "id": "overture:transportation:example:simple-turn-restriction-source",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -113.57822030759499,
        50.01868388494378
      ],
      [
        -113.57831482025354,
        50.018860947117304
      ],
      [
        -113.57851814418316,
        50.01923724443006
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 5,
    "subtype": "road",
    "class": "secondary",
    "connectors": [
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector1",
        "at": 0
      },
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector2",
        "at": 1
      }
    ],
    "prohibited_transitions": [
      {
        "sequence": [
          {
            "segment_id": "overture:transportation:example:simple-turn-restriction-target",
            "connector_id": "overture:transportation:example:simple-turn-restriction-connector2"
          }
        ],
        "final_heading": "forward",
        "when": {
          "heading": "forward"
        }
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:example:simple-turn-restriction-source",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -113.57822030759499,
        50.01868388494378
      ],
      [
        -113.57831482025354,
        50.018860947117304
      ],
      [
        -113.57851814418316,
        50.01923724443006
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 5,
    "subtype": "road",
    "class": "secondary",
    "connectors": [
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector1",
        "at": 0
      },
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector2",
        "at": 1
      }
    ],
    "prohibited_transitions": [
      {
        "sequence": [
          {
            "segment_id": "overture:transportation:example:simple-turn-restriction-target",
            "connector_id": "overture:transportation:example:simple-turn-restriction-connector2"
          }
        ],
        "final_heading": "forward",
        "when": {
          "heading": "forward"
        }
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 20
#### json
```json
{
  "id": "overture:transportation:example:simple-turn-restriction-target",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -113.57851814418316,
        50.01923724443006
      ],
      [
        -113.57837460847787,
        50.01919574268962
      ],
      [
        -113.57812342099429,
        50.01919343703648
      ],
      [
        -113.57803729957116,
        50.01923263312719
      ],
      [
        -113.57766410673773,
        50.01923263312719
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "secondary",
    "connectors": [
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector1",
        "at": 0
      },
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector2",
        "at": 1
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:example:simple-turn-restriction-target",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -113.57851814418316,
        50.01923724443006
      ],
      [
        -113.57837460847787,
        50.01919574268962
      ],
      [
        -113.57812342099429,
        50.01919343703648
      ],
      [
        -113.57803729957116,
        50.01923263312719
      ],
      [
        -113.57766410673773,
        50.01923263312719
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "secondary",
    "connectors": [
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector1",
        "at": 0
      },
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector2",
        "at": 1
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 21
#### json
```json
{
  "id": "overture:transportation:example:via-turn-restriction-source",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -71.1100226929593,
        42.30156668552357
      ],
      [
        -71.11055493812631,
        42.30157222996385
      ],
      [
        -71.11102971081017,
        42.30157407811038
      ],
      [
        -71.11143701579662,
        42.30156114108277
      ],
      [
        -71.11197425857047,
        42.30152602627953
      ],
      [
        -71.11234408150312,
        42.30149091145671
      ],
      [
        -71.1126589307566,
        42.30147612626226
      ],
      [
        -71.11301376086777,
        42.301494607754876
      ],
      [
        -71.11320616874515,
        42.301516785538524
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 5,
    "subtype": "road",
    "class": "primary",
    "connectors": [
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector1",
        "at": 0
      },
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector2",
        "at": 1
      }
    ],
    "names": {
      "primary": "Arborway"
    },
    "prohibited_transitions": [
      {
        "sequence": [
          {
            "segment_id": "overture:transportation:example:via-turn-restriction-target",
            "connector_id": "overture:transportation:example:via-turn-restriction-connector2"
          },
          {
            "segment_id": "overture:transportation:example:via-turn-restriction-via",
            "connector_id": "overture:transportation:example:via-turn-restriction-connector1"
          }
        ],
        "final_heading": "forward",
        "when": {
          "heading": "forward",
          "during": "Mo-Fr 06:00-09:00, 15:00-19:00"
        }
      }
    ],
    "road_surface": [
      {
        "value": "paved"
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:example:via-turn-restriction-source",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -71.1100226929593,
        42.30156668552357
      ],
      [
        -71.11055493812631,
        42.30157222996385
      ],
      [
        -71.11102971081017,
        42.30157407811038
      ],
      [
        -71.11143701579662,
        42.30156114108277
      ],
      [
        -71.11197425857047,
        42.30152602627953
      ],
      [
        -71.11234408150312,
        42.30149091145671
      ],
      [
        -71.1126589307566,
        42.30147612626226
      ],
      [
        -71.11301376086777,
        42.301494607754876
      ],
      [
        -71.11320616874515,
        42.301516785538524
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 5,
    "subtype": "road",
    "class": "primary",
    "connectors": [
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector1",
        "at": 0
      },
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector2",
        "at": 1
      }
    ],
    "names": {
      "primary": "Arborway"
    },
    "prohibited_transitions": [
      {
        "sequence": [
          {
            "segment_id": "overture:transportation:example:via-turn-restriction-target",
            "connector_id": "overture:transportation:example:via-turn-restriction-connector2"
          },
          {
            "segment_id": "overture:transportation:example:via-turn-restriction-via",
            "connector_id": "overture:transportation:example:via-turn-restriction-connector1"
          }
        ],
        "final_heading": "forward",
        "when": {
          "heading": "forward",
          "during": "Mo-Fr 06:00-09:00, 15:00-19:00"
        }
      }
    ],
    "road_surface": [
      {
        "value": "paved"
      }
    ]
  }
}
```

#### ttl
```ttl
@prefix ns1: <osm:> .

[] ns1:hasSurfaceType <https://w3id.org/ogc/om/surfaces/paved> .


```


### Example 22
#### json
```json
{
  "id": "overture:transportation:example:turn-restriction-target",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -71.11325364601365,
        42.301374477956756
      ],
      [
        -71.11278137213321,
        42.3013264259736
      ],
      [
        -71.11248901211202,
        42.3013264259736
      ],
      [
        -71.11157195119078,
        42.30139295947919
      ],
      [
        -71.1109997251666,
        42.301428074356636
      ],
      [
        -71.11058492376937,
        42.30143177065813
      ],
      [
        -71.11002519176327,
        42.301415137298676
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 5,
    "subtype": "road",
    "class": "primary",
    "connectors": [
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector1",
        "at": 0
      },
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector2",
        "at": 1
      }
    ],
    "names": {
      "primary": "Arborway"
    },
    "road_surface": [
      {
        "value": "paved"
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:example:turn-restriction-target",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -71.11325364601365,
        42.301374477956756
      ],
      [
        -71.11278137213321,
        42.3013264259736
      ],
      [
        -71.11248901211202,
        42.3013264259736
      ],
      [
        -71.11157195119078,
        42.30139295947919
      ],
      [
        -71.1109997251666,
        42.301428074356636
      ],
      [
        -71.11058492376937,
        42.30143177065813
      ],
      [
        -71.11002519176327,
        42.301415137298676
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 5,
    "subtype": "road",
    "class": "primary",
    "connectors": [
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector1",
        "at": 0
      },
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector2",
        "at": 1
      }
    ],
    "names": {
      "primary": "Arborway"
    },
    "road_surface": [
      {
        "value": "paved"
      }
    ]
  }
}
```

#### ttl
```ttl
@prefix ns1: <osm:> .

[] ns1:hasSurfaceType <https://w3id.org/ogc/om/surfaces/paved> .


```


### Example 23
#### json
```json
{
  "id": "overture:transportation:example:simple-road2",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -71.11213418200086,
        42.3017182333833
      ],
      [
        -71.11234408150312,
        42.30149091145671
      ],
      [
        -71.11248901211202,
        42.3013264259736
      ],
      [
        -71.11283634581244,
        42.30093831245662
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 5,
    "subtype": "road",
    "class": "secondary",
    "connectors": [
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector1",
        "at": 0
      },
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector2",
        "at": 1
      }
    ],
    "names": {
      "primary": "Washington Street"
    },
    "road_surface": [
      {
        "value": "paved"
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:example:simple-road2",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -71.11213418200086,
        42.3017182333833
      ],
      [
        -71.11234408150312,
        42.30149091145671
      ],
      [
        -71.11248901211202,
        42.3013264259736
      ],
      [
        -71.11283634581244,
        42.30093831245662
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 5,
    "subtype": "road",
    "class": "secondary",
    "connectors": [
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector1",
        "at": 0
      },
      {
        "connector_id": "overture:transportation:example:via-turn-restriction-connector2",
        "at": 1
      }
    ],
    "names": {
      "primary": "Washington Street"
    },
    "road_surface": [
      {
        "value": "paved"
      }
    ]
  }
}
```

#### ttl
```ttl
@prefix ns1: <osm:> .

[] ns1:hasSurfaceType <https://w3id.org/ogc/om/surfaces/paved> .


```


### Example 24
#### json
```json
{
  "id": "overture:transportation:segment:123",
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
    "ext_baz": "I am a custom user property...",
    "theme": "transportation",
    "type": "segment",
    "version": 3,
    "subtype": "rail",
    "class": "standard_gauge",
    "names": {
      "primary": "Generic Rail Name"
    },
    "rail_flags": [
      {
        "values": [
          "is_freight"
        ],
        "between": [
          0,
          0.5
        ]
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:segment:123",
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
    "ext_baz": "I am a custom user property...",
    "theme": "transportation",
    "type": "segment",
    "version": 3,
    "subtype": "rail",
    "class": "standard_gauge",
    "names": {
      "primary": "Generic Rail Name"
    },
    "rail_flags": [
      {
        "values": [
          "is_freight"
        ],
        "between": [
          0,
          0.5
        ]
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 25
#### json
```json
{
  "id": "overture:transportation:segment:123",
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
    "ext_baz": "I am a custom user property...",
    "theme": "transportation",
    "type": "segment",
    "version": 3,
    "subtype": "rail",
    "class": "subway",
    "names": {
      "primary": "Generic Rail Name"
    },
    "rail_flags": [
      {
        "values": [
          "is_tunnel"
        ],
        "between": [
          0,
          0.5
        ]
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:segment:123",
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
    "ext_baz": "I am a custom user property...",
    "theme": "transportation",
    "type": "segment",
    "version": 3,
    "subtype": "rail",
    "class": "subway",
    "names": {
      "primary": "Generic Rail Name"
    },
    "rail_flags": [
      {
        "values": [
          "is_tunnel"
        ],
        "between": [
          0,
          0.5
        ]
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 26
#### json
```json
{
  "id": "overture:transportation:segment:123",
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
    "ext_baz": "I am a custom user property...",
    "theme": "transportation",
    "type": "segment",
    "version": 3,
    "subtype": "rail",
    "class": "funicular",
    "connectors": [
      {
        "connector_id": "fooConnector",
        "at": 0
      },
      {
        "connector_id": "barConnector",
        "at": 1
      }
    ],
    "names": {
      "primary": "Generic Rail Name"
    },
    "rail_flags": [
      {
        "values": [
          "is_tunnel",
          "is_freight"
        ]
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:segment:123",
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
    "ext_baz": "I am a custom user property...",
    "theme": "transportation",
    "type": "segment",
    "version": 3,
    "subtype": "rail",
    "class": "funicular",
    "connectors": [
      {
        "connector_id": "fooConnector",
        "at": 0
      },
      {
        "connector_id": "barConnector",
        "at": 1
      }
    ],
    "names": {
      "primary": "Generic Rail Name"
    },
    "rail_flags": [
      {
        "values": [
          "is_tunnel",
          "is_freight"
        ]
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 27
#### json
```json
{
  "id": "overture:transportation:segment:example:destinations:1",
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
    "subtype": "road",
    "class": "secondary",
    "version": 0,
    "connectors": [
      {
        "connector_id": "overture:transportation:connector:123",
        "at": 0
      },
      {
        "connector_id": "overture:transportation:connector:678",
        "at": 1
      }
    ],
    "destinations": [
      {
        "when": {
          "heading": "forward"
        },
        "from_connector_id": "overture:transportation:connector:123",
        "to_connector_id": "overture:transportation:connector:123",
        "to_segment_id": "overture:transportation:segment:567",
        "final_heading": "backward",
        "labels": [
          {
            "value": "Seattle",
            "type": "unknown"
          },
          {
            "value": "Main Street",
            "type": "street"
          },
          {
            "value": "I90",
            "type": "route_ref"
          }
        ],
        "symbols": [
          "motorway",
          "airport"
        ]
      },
      {
        "when": {
          "heading": "backward"
        },
        "from_connector_id": "overture:transportation:connector:123",
        "to_connector_id": "overture:transportation:connector:123",
        "to_segment_id": "overture:transportation:segment:567",
        "final_heading": "backward",
        "labels": [
          {
            "value": "Redmond",
            "type": "unknown"
          },
          {
            "value": "I5",
            "type": "toward_route_ref"
          }
        ]
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:segment:example:destinations:1",
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
    "subtype": "road",
    "class": "secondary",
    "version": 0,
    "connectors": [
      {
        "connector_id": "overture:transportation:connector:123",
        "at": 0
      },
      {
        "connector_id": "overture:transportation:connector:678",
        "at": 1
      }
    ],
    "destinations": [
      {
        "when": {
          "heading": "forward"
        },
        "from_connector_id": "overture:transportation:connector:123",
        "to_connector_id": "overture:transportation:connector:123",
        "to_segment_id": "overture:transportation:segment:567",
        "final_heading": "backward",
        "labels": [
          {
            "value": "Seattle",
            "type": "unknown"
          },
          {
            "value": "Main Street",
            "type": "street"
          },
          {
            "value": "I90",
            "type": "route_ref"
          }
        ],
        "symbols": [
          "motorway",
          "airport"
        ]
      },
      {
        "when": {
          "heading": "backward"
        },
        "from_connector_id": "overture:transportation:connector:123",
        "to_connector_id": "overture:transportation:connector:123",
        "to_segment_id": "overture:transportation:segment:567",
        "final_heading": "backward",
        "labels": [
          {
            "value": "Redmond",
            "type": "unknown"
          },
          {
            "value": "I5",
            "type": "toward_route_ref"
          }
        ]
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 28
#### json
```json
{
  "id": "overture:transportation:segment:example:access",
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
        0
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "subtype": "road",
    "class": "primary",
    "version": 2,
    "access_restrictions": [
      {
        "access_type": "denied",
        "between": [
          0,
          0.5
        ]
      },
      {
        "access_type": "denied",
        "when": {
          "during": "PH"
        }
      },
      {
        "access_type": "denied",
        "when": {
          "heading": "forward"
        }
      },
      {
        "access_type": "allowed",
        "when": {
          "heading": "forward",
          "mode": [
            "vehicle"
          ]
        }
      },
      {
        "access_type": "allowed",
        "when": {
          "heading": "forward",
          "using": [
            "at_destination"
          ]
        }
      },
      {
        "access_type": "allowed",
        "when": {
          "heading": "forward",
          "recognized": [
            "as_employee"
          ]
        }
      },
      {
        "access_type": "allowed",
        "when": {
          "heading": "forward",
          "vehicle": [
            {
              "dimension": "axle_count",
              "comparison": "less_than",
              "value": 3
            },
            {
              "dimension": "weight",
              "comparison": "less_than_equal",
              "value": 600,
              "unit": "kg"
            },
            {
              "dimension": "height",
              "comparison": "less_than",
              "value": 12,
              "unit": "ft"
            }
          ]
        }
      },
      {
        "access_type": "denied",
        "between": [
          0.25,
          0.5
        ],
        "when": {
          "heading": "forward",
          "during": "PH",
          "mode": [
            "car",
            "hgv"
          ],
          "using": [
            "at_destination"
          ],
          "recognized": [
            "as_employee"
          ],
          "vehicle": [
            {
              "dimension": "axle_count",
              "comparison": "less_than",
              "value": 3
            },
            {
              "dimension": "weight",
              "comparison": "less_than_equal",
              "value": 600,
              "unit": "kg"
            },
            {
              "dimension": "height",
              "comparison": "less_than",
              "value": 12,
              "unit": "ft"
            }
          ]
        }
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:segment:example:access",
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
        0
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "subtype": "road",
    "class": "primary",
    "version": 2,
    "access_restrictions": [
      {
        "access_type": "denied",
        "between": [
          0,
          0.5
        ]
      },
      {
        "access_type": "denied",
        "when": {
          "during": "PH"
        }
      },
      {
        "access_type": "denied",
        "when": {
          "heading": "forward"
        }
      },
      {
        "access_type": "allowed",
        "when": {
          "heading": "forward",
          "mode": [
            "vehicle"
          ]
        }
      },
      {
        "access_type": "allowed",
        "when": {
          "heading": "forward",
          "using": [
            "at_destination"
          ]
        }
      },
      {
        "access_type": "allowed",
        "when": {
          "heading": "forward",
          "recognized": [
            "as_employee"
          ]
        }
      },
      {
        "access_type": "allowed",
        "when": {
          "heading": "forward",
          "vehicle": [
            {
              "dimension": "axle_count",
              "comparison": "less_than",
              "value": 3
            },
            {
              "dimension": "weight",
              "comparison": "less_than_equal",
              "value": 600,
              "unit": "kg"
            },
            {
              "dimension": "height",
              "comparison": "less_than",
              "value": 12,
              "unit": "ft"
            }
          ]
        }
      },
      {
        "access_type": "denied",
        "between": [
          0.25,
          0.5
        ],
        "when": {
          "heading": "forward",
          "during": "PH",
          "mode": [
            "car",
            "hgv"
          ],
          "using": [
            "at_destination"
          ],
          "recognized": [
            "as_employee"
          ],
          "vehicle": [
            {
              "dimension": "axle_count",
              "comparison": "less_than",
              "value": 3
            },
            {
              "dimension": "weight",
              "comparison": "less_than_equal",
              "value": 600,
              "unit": "kg"
            },
            {
              "dimension": "height",
              "comparison": "less_than",
              "value": 12,
              "unit": "ft"
            }
          ]
        }
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 29
#### json
```json
{
  "id": "overture:transportation:segment:example:prohibited-transitions",
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
        0
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "subtype": "road",
    "class": "secondary",
    "version": 2,
    "prohibited_transitions": [
      {
        "sequence": [
          {
            "connector_id": "connector1",
            "segment_id": "segment1"
          }
        ],
        "final_heading": "forward",
        "between": [
          0,
          0.5
        ]
      },
      {
        "sequence": [
          {
            "connector_id": "connector1",
            "segment_id": "segment1"
          }
        ],
        "final_heading": "forward",
        "when": {
          "during": "PH"
        }
      },
      {
        "sequence": [
          {
            "connector_id": "connector1",
            "segment_id": "segment1"
          }
        ],
        "final_heading": "forward",
        "when": {
          "heading": "forward"
        }
      },
      {
        "sequence": [
          {
            "connector_id": "connector1",
            "segment_id": "segment1"
          }
        ],
        "final_heading": "forward",
        "when": {
          "heading": "forward",
          "mode": [
            "car",
            "hgv"
          ]
        }
      },
      {
        "sequence": [
          {
            "connector_id": "connector1",
            "segment_id": "segment1"
          }
        ],
        "final_heading": "forward",
        "when": {
          "heading": "forward",
          "using": [
            "at_destination"
          ]
        }
      },
      {
        "sequence": [
          {
            "connector_id": "connector1",
            "segment_id": "segment1"
          }
        ],
        "final_heading": "forward",
        "when": {
          "heading": "forward",
          "recognized": [
            "as_employee"
          ]
        }
      },
      {
        "sequence": [
          {
            "connector_id": "connector1",
            "segment_id": "segment1"
          }
        ],
        "final_heading": "forward",
        "when": {
          "heading": "forward",
          "vehicle": [
            {
              "dimension": "axle_count",
              "comparison": "less_than",
              "value": 3
            },
            {
              "dimension": "weight",
              "comparison": "less_than_equal",
              "value": 600,
              "unit": "kg"
            },
            {
              "dimension": "height",
              "comparison": "less_than",
              "value": 12,
              "unit": "ft"
            }
          ]
        }
      },
      {
        "sequence": [
          {
            "connector_id": "connector1",
            "segment_id": "segment1"
          }
        ],
        "final_heading": "forward",
        "between": [
          0.25,
          0.5
        ],
        "when": {
          "heading": "forward",
          "during": "PH",
          "mode": [
            "car",
            "hgv"
          ],
          "using": [
            "at_destination"
          ],
          "recognized": [
            "as_employee"
          ],
          "vehicle": [
            {
              "dimension": "axle_count",
              "comparison": "less_than",
              "value": 3
            },
            {
              "dimension": "weight",
              "comparison": "less_than_equal",
              "value": 600,
              "unit": "kg"
            },
            {
              "dimension": "height",
              "comparison": "less_than",
              "value": 12,
              "unit": "ft"
            }
          ]
        }
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:segment:example:prohibited-transitions",
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
        0
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "subtype": "road",
    "class": "secondary",
    "version": 2,
    "prohibited_transitions": [
      {
        "sequence": [
          {
            "connector_id": "connector1",
            "segment_id": "segment1"
          }
        ],
        "final_heading": "forward",
        "between": [
          0,
          0.5
        ]
      },
      {
        "sequence": [
          {
            "connector_id": "connector1",
            "segment_id": "segment1"
          }
        ],
        "final_heading": "forward",
        "when": {
          "during": "PH"
        }
      },
      {
        "sequence": [
          {
            "connector_id": "connector1",
            "segment_id": "segment1"
          }
        ],
        "final_heading": "forward",
        "when": {
          "heading": "forward"
        }
      },
      {
        "sequence": [
          {
            "connector_id": "connector1",
            "segment_id": "segment1"
          }
        ],
        "final_heading": "forward",
        "when": {
          "heading": "forward",
          "mode": [
            "car",
            "hgv"
          ]
        }
      },
      {
        "sequence": [
          {
            "connector_id": "connector1",
            "segment_id": "segment1"
          }
        ],
        "final_heading": "forward",
        "when": {
          "heading": "forward",
          "using": [
            "at_destination"
          ]
        }
      },
      {
        "sequence": [
          {
            "connector_id": "connector1",
            "segment_id": "segment1"
          }
        ],
        "final_heading": "forward",
        "when": {
          "heading": "forward",
          "recognized": [
            "as_employee"
          ]
        }
      },
      {
        "sequence": [
          {
            "connector_id": "connector1",
            "segment_id": "segment1"
          }
        ],
        "final_heading": "forward",
        "when": {
          "heading": "forward",
          "vehicle": [
            {
              "dimension": "axle_count",
              "comparison": "less_than",
              "value": 3
            },
            {
              "dimension": "weight",
              "comparison": "less_than_equal",
              "value": 600,
              "unit": "kg"
            },
            {
              "dimension": "height",
              "comparison": "less_than",
              "value": 12,
              "unit": "ft"
            }
          ]
        }
      },
      {
        "sequence": [
          {
            "connector_id": "connector1",
            "segment_id": "segment1"
          }
        ],
        "final_heading": "forward",
        "between": [
          0.25,
          0.5
        ],
        "when": {
          "heading": "forward",
          "during": "PH",
          "mode": [
            "car",
            "hgv"
          ],
          "using": [
            "at_destination"
          ],
          "recognized": [
            "as_employee"
          ],
          "vehicle": [
            {
              "dimension": "axle_count",
              "comparison": "less_than",
              "value": 3
            },
            {
              "dimension": "weight",
              "comparison": "less_than_equal",
              "value": 600,
              "unit": "kg"
            },
            {
              "dimension": "height",
              "comparison": "less_than",
              "value": 12,
              "unit": "ft"
            }
          ]
        }
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 30
#### json
```json
{
  "id": "overture:transportation:segment:example:speed-limits",
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
        0
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "subtype": "road",
    "class": "tertiary",
    "version": 3,
    "speed_limits": [
      {
        "max_speed": {
          "value": 20,
          "unit": "km/h"
        },
        "between": [
          0,
          0.5
        ]
      },
      {
        "min_speed": {
          "value": 25,
          "unit": "mph"
        },
        "when": {
          "during": "PH"
        }
      },
      {
        "max_speed": {
          "value": 100,
          "unit": "km/h"
        },
        "min_speed": {
          "value": 75,
          "unit": "km/h"
        },
        "when": {
          "heading": "forward"
        }
      },
      {
        "min_speed": {
          "value": 25,
          "unit": "mph"
        },
        "when": {
          "heading": "forward",
          "mode": [
            "car",
            "hgv"
          ]
        }
      },
      {
        "max_speed": {
          "value": 60,
          "unit": "mph"
        },
        "is_max_speed_variable": true,
        "when": {
          "heading": "forward",
          "using": [
            "at_destination"
          ]
        }
      },
      {
        "min_speed": {
          "value": 25,
          "unit": "mph"
        },
        "when": {
          "heading": "forward",
          "recognized": [
            "as_employee"
          ]
        }
      },
      {
        "min_speed": {
          "value": 40,
          "unit": "mph"
        },
        "when": {
          "heading": "forward",
          "vehicle": [
            {
              "dimension": "axle_count",
              "comparison": "less_than",
              "value": 3
            },
            {
              "dimension": "weight",
              "comparison": "less_than_equal",
              "value": 600,
              "unit": "kg"
            },
            {
              "dimension": "height",
              "comparison": "less_than",
              "value": 12,
              "unit": "ft"
            }
          ]
        }
      },
      {
        "max_speed": {
          "value": 30,
          "unit": "km/h"
        },
        "min_speed": {
          "value": 20,
          "unit": "mph"
        },
        "is_max_speed_variable": true,
        "between": [
          0.25,
          0.5
        ],
        "when": {
          "heading": "forward",
          "during": "PH",
          "mode": [
            "car",
            "hgv"
          ],
          "using": [
            "at_destination"
          ],
          "recognized": [
            "as_employee"
          ],
          "vehicle": [
            {
              "dimension": "axle_count",
              "comparison": "less_than",
              "value": 3
            },
            {
              "dimension": "weight",
              "comparison": "less_than_equal",
              "value": 600,
              "unit": "kg"
            },
            {
              "dimension": "height",
              "comparison": "less_than",
              "value": 12,
              "unit": "ft"
            }
          ]
        }
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:segment:example:speed-limits",
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
        0
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "subtype": "road",
    "class": "tertiary",
    "version": 3,
    "speed_limits": [
      {
        "max_speed": {
          "value": 20,
          "unit": "km/h"
        },
        "between": [
          0,
          0.5
        ]
      },
      {
        "min_speed": {
          "value": 25,
          "unit": "mph"
        },
        "when": {
          "during": "PH"
        }
      },
      {
        "max_speed": {
          "value": 100,
          "unit": "km/h"
        },
        "min_speed": {
          "value": 75,
          "unit": "km/h"
        },
        "when": {
          "heading": "forward"
        }
      },
      {
        "min_speed": {
          "value": 25,
          "unit": "mph"
        },
        "when": {
          "heading": "forward",
          "mode": [
            "car",
            "hgv"
          ]
        }
      },
      {
        "max_speed": {
          "value": 60,
          "unit": "mph"
        },
        "is_max_speed_variable": true,
        "when": {
          "heading": "forward",
          "using": [
            "at_destination"
          ]
        }
      },
      {
        "min_speed": {
          "value": 25,
          "unit": "mph"
        },
        "when": {
          "heading": "forward",
          "recognized": [
            "as_employee"
          ]
        }
      },
      {
        "min_speed": {
          "value": 40,
          "unit": "mph"
        },
        "when": {
          "heading": "forward",
          "vehicle": [
            {
              "dimension": "axle_count",
              "comparison": "less_than",
              "value": 3
            },
            {
              "dimension": "weight",
              "comparison": "less_than_equal",
              "value": 600,
              "unit": "kg"
            },
            {
              "dimension": "height",
              "comparison": "less_than",
              "value": 12,
              "unit": "ft"
            }
          ]
        }
      },
      {
        "max_speed": {
          "value": 30,
          "unit": "km/h"
        },
        "min_speed": {
          "value": 20,
          "unit": "mph"
        },
        "is_max_speed_variable": true,
        "between": [
          0.25,
          0.5
        ],
        "when": {
          "heading": "forward",
          "during": "PH",
          "mode": [
            "car",
            "hgv"
          ],
          "using": [
            "at_destination"
          ],
          "recognized": [
            "as_employee"
          ],
          "vehicle": [
            {
              "dimension": "axle_count",
              "comparison": "less_than",
              "value": 3
            },
            {
              "dimension": "weight",
              "comparison": "less_than_equal",
              "value": 600,
              "unit": "kg"
            },
            {
              "dimension": "height",
              "comparison": "less_than",
              "value": 12,
              "unit": "ft"
            }
          ]
        }
      }
    ]
  }
}
```

#### ttl
```ttl
@prefix om: <https://w3id.org/ogc/om/> .
@prefix qudt: <http://qudt.org/schema/qudt/> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

[] om:hasSpeedLimit [ om:hasMinSpeed [ qudt:hasUnit "mph" ;
                    rdf:value 40 ] ;
            om:when "{\"heading\":\"forward\",\"vehicle\":[{\"comparison\":\"less_than\",\"dimension\":\"axle_count\",\"value\":3},{\"comparison\":\"less_than_equal\",\"dimension\":\"weight\",\"unit\":\"kg\",\"value\":600},{\"comparison\":\"less_than\",\"dimension\":\"height\",\"unit\":\"ft\",\"value\":12}]}"^^rdf:JSON ],
        [ om:hasMaxSpeed [ qudt:hasUnit "km/h" ;
                    rdf:value 20 ] ],
        [ om:hasMinSpeed [ qudt:hasUnit "mph" ;
                    rdf:value 25 ] ;
            om:when "{\"heading\":\"forward\",\"mode\":[\"car\",\"hgv\"]}"^^rdf:JSON ],
        [ om:hasMaxSpeed [ qudt:hasUnit "mph" ;
                    rdf:value 60 ] ;
            om:isMaxSpeedVariable true ;
            om:when "{\"heading\":\"forward\",\"using\":[\"at_destination\"]}"^^rdf:JSON ],
        [ om:hasMinSpeed [ qudt:hasUnit "mph" ;
                    rdf:value 25 ] ;
            om:when "{\"during\":\"PH\"}"^^rdf:JSON ],
        [ om:hasMaxSpeed [ qudt:hasUnit "km/h" ;
                    rdf:value 30 ] ;
            om:hasMinSpeed [ qudt:hasUnit "mph" ;
                    rdf:value 20 ] ;
            om:isMaxSpeedVariable true ;
            om:when "{\"during\":\"PH\",\"heading\":\"forward\",\"mode\":[\"car\",\"hgv\"],\"recognized\":[\"as_employee\"],\"using\":[\"at_destination\"],\"vehicle\":[{\"comparison\":\"less_than\",\"dimension\":\"axle_count\",\"value\":3},{\"comparison\":\"less_than_equal\",\"dimension\":\"weight\",\"unit\":\"kg\",\"value\":600},{\"comparison\":\"less_than\",\"dimension\":\"height\",\"unit\":\"ft\",\"value\":12}]}"^^rdf:JSON ],
        [ om:hasMinSpeed [ qudt:hasUnit "mph" ;
                    rdf:value 25 ] ;
            om:when "{\"heading\":\"forward\",\"recognized\":[\"as_employee\"]}"^^rdf:JSON ],
        [ om:hasMaxSpeed [ qudt:hasUnit "km/h" ;
                    rdf:value 100 ] ;
            om:hasMinSpeed [ qudt:hasUnit "km/h" ;
                    rdf:value 75 ] ;
            om:when "{\"heading\":\"forward\"}"^^rdf:JSON ] .


```


### Example 31
#### json
```json
{
  "id": "overture:transportation:segment:789",
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
    "version": 3,
    "subtype": "road",
    "class": "tertiary",
    "road_surface": [
      {
        "value": "gravel"
      }
    ],
    "road_flags": [
      {
        "values": [
          "is_abandoned"
        ]
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:segment:789",
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
    "version": 3,
    "subtype": "road",
    "class": "tertiary",
    "road_surface": [
      {
        "value": "gravel"
      }
    ],
    "road_flags": [
      {
        "values": [
          "is_abandoned"
        ]
      }
    ]
  }
}
```

#### ttl
```ttl
@prefix ns1: <osm:> .

[] ns1:hasSurfaceType <https://w3id.org/ogc/om/surfaces/gravel> .


```


### Example 32
#### json
```json
{
  "id": "overture:transportation:segment:1415",
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
    "ext_baz": "I am a custom user property...",
    "ext_description": "This is an example road segment in which as many properties as possible are specified using rules instead of flat values. For example, the road flags are specified using rules.",
    "theme": "transportation",
    "type": "segment",
    "version": 5,
    "subtype": "road",
    "class": "primary",
    "access_restrictions": [
      {
        "access_type": "denied"
      },
      {
        "access_type": "designated",
        "when": {
          "mode": [
            "truck"
          ]
        },
        "between": [
          0.1,
          0.25
        ]
      },
      {
        "access_type": "allowed",
        "when": {
          "using": [
            "as_customer",
            "to_farm"
          ],
          "recognized": [
            "as_permitted",
            "as_employee"
          ]
        },
        "between": [
          0.25,
          0.5
        ]
      },
      {
        "access_type": "allowed",
        "when": {
          "vehicle": [
            {
              "dimension": "axle_count",
              "comparison": "greater_than",
              "value": 5
            }
          ]
        },
        "between": [
          0.5,
          0.7
        ]
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:segment:1415",
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
    "ext_baz": "I am a custom user property...",
    "ext_description": "This is an example road segment in which as many properties as possible are specified using rules instead of flat values. For example, the road flags are specified using rules.",
    "theme": "transportation",
    "type": "segment",
    "version": 5,
    "subtype": "road",
    "class": "primary",
    "access_restrictions": [
      {
        "access_type": "denied"
      },
      {
        "access_type": "designated",
        "when": {
          "mode": [
            "truck"
          ]
        },
        "between": [
          0.1,
          0.25
        ]
      },
      {
        "access_type": "allowed",
        "when": {
          "using": [
            "as_customer",
            "to_farm"
          ],
          "recognized": [
            "as_permitted",
            "as_employee"
          ]
        },
        "between": [
          0.25,
          0.5
        ]
      },
      {
        "access_type": "allowed",
        "when": {
          "vehicle": [
            {
              "dimension": "axle_count",
              "comparison": "greater_than",
              "value": 5
            }
          ]
        },
        "between": [
          0.5,
          0.7
        ]
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 33
#### json
```json
{
  "id": "overture:transportation:segment:1555",
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
    "version": 5,
    "subtype": "road",
    "class": "service",
    "subclass_rules": [
      {
        "value": "alley",
        "between": [
          0,
          0.5
        ]
      }
    ],
    "access_restrictions": [
      {
        "access_type": "allowed",
        "when": {
          "using": [
            "at_destination"
          ]
        }
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:segment:1555",
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
    "version": 5,
    "subtype": "road",
    "class": "service",
    "subclass_rules": [
      {
        "value": "alley",
        "between": [
          0,
          0.5
        ]
      }
    ],
    "access_restrictions": [
      {
        "access_type": "allowed",
        "when": {
          "using": [
            "at_destination"
          ]
        }
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 34
#### json
```json
{
  "id": "overture:transportation:segment:example:covered",
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
    "version": 3,
    "subtype": "road",
    "class": "tertiary",
    "road_surface": [
      {
        "value": "paved"
      }
    ],
    "road_flags": [
      {
        "values": [
          "is_covered"
        ]
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:segment:example:covered",
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
    "version": 3,
    "subtype": "road",
    "class": "tertiary",
    "road_surface": [
      {
        "value": "paved"
      }
    ],
    "road_flags": [
      {
        "values": [
          "is_covered"
        ]
      }
    ]
  }
}
```

#### ttl
```ttl
@prefix ns1: <osm:> .

[] ns1:hasSurfaceType <https://w3id.org/ogc/om/surfaces/paved> .


```


### Example 35
#### json
```json
{
  "id": "overture:transportation:segment:example:indoor",
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
    "class": "tertiary",
    "road_surface": [
      {
        "value": "unknown"
      }
    ],
    "road_flags": [
      {
        "values": [
          "is_indoor"
        ]
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:segment:example:indoor",
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
    "class": "tertiary",
    "road_surface": [
      {
        "value": "unknown"
      }
    ],
    "road_flags": [
      {
        "values": [
          "is_indoor"
        ]
      }
    ]
  }
}
```

#### ttl
```ttl
@prefix ns1: <osm:> .

[] ns1:hasSurfaceType <https://w3id.org/ogc/om/surfaces/unknown> .


```


### Example 36
#### json
```json
{
  "id": "overture:transportation:segment:example:level",
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
        0
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "subtype": "road",
    "version": 2,
    "class": "residential",
    "level_rules": [
      {
        "value": -1,
        "between": [
          0,
          0.5
        ]
      },
      {
        "value": 1,
        "between": [
          0.75,
          1
        ]
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:segment:example:level",
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
        0
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "subtype": "road",
    "version": 2,
    "class": "residential",
    "level_rules": [
      {
        "value": -1,
        "between": [
          0,
          0.5
        ]
      },
      {
        "value": 1,
        "between": [
          0.75,
          1
        ]
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 37
#### json
```json
{
  "id": "overture:transportation:segment:123",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        0,
        0
      ],
      [
        0.03,
        0
      ],
      [
        0.1,
        0
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "secondary",
    "connectors": [
      {
        "connector_id": "fooConnector",
        "at": 0
      },
      {
        "connector_id": "barConnector",
        "at": 0.3
      },
      {
        "connector_id": "bazConnector",
        "at": 1
      }
    ],
    "road_surface": [
      {
        "value": "paved"
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:segment:123",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        0,
        0
      ],
      [
        0.03,
        0
      ],
      [
        0.1,
        0
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "secondary",
    "connectors": [
      {
        "connector_id": "fooConnector",
        "at": 0
      },
      {
        "connector_id": "barConnector",
        "at": 0.3
      },
      {
        "connector_id": "bazConnector",
        "at": 1
      }
    ],
    "road_surface": [
      {
        "value": "paved"
      }
    ]
  }
}
```

#### ttl
```ttl
@prefix ns1: <osm:> .

[] ns1:hasSurfaceType <https://w3id.org/ogc/om/surfaces/paved> .


```


### Example 38
#### json
```json
{
  "id": "overture:transportation:segment:1213",
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
    "version": 6,
    "subtype": "road",
    "class": "secondary",
    "connectors": [
      {
        "connector_id": "fooConnector",
        "at": 0
      },
      {
        "connector_id": "barConnector",
        "at": 1
      }
    ],
    "access_restrictions": [
      {
        "access_type": "denied",
        "when": {
          "heading": "forward"
        }
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:segment:1213",
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
    "version": 6,
    "subtype": "road",
    "class": "secondary",
    "connectors": [
      {
        "connector_id": "fooConnector",
        "at": 0
      },
      {
        "connector_id": "barConnector",
        "at": 1
      }
    ],
    "access_restrictions": [
      {
        "access_type": "denied",
        "when": {
          "heading": "forward"
        }
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 39
#### json
```json
{
  "id": "overture:transportation:segment:1516",
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
    "version": 5,
    "subtype": "road",
    "class": "path"
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:segment:1516",
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
    "version": 5,
    "subtype": "road",
    "class": "path"
  }
}
```

#### ttl
```ttl


```


### Example 40
#### json
```json
{
  "id": "overture:transportation:segment:123",
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
    "ext_baz": "I am a custom user property...",
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "secondary",
    "connectors": [
      {
        "connector_id": "fooConnector",
        "at": 0
      },
      {
        "connector_id": "barConnector",
        "at": 1
      }
    ],
    "names": {
      "primary": "Common Road Name 1",
      "rules": [
        {
          "variant": "common",
          "value": "Common Road Name 1",
          "between": [
            0,
            0.5
          ]
        },
        {
          "variant": "short",
          "value": "SRN1",
          "between": [
            0,
            0.5
          ]
        },
        {
          "variant": "common",
          "value": "Common Road Name 2",
          "between": [
            0.5,
            1
          ]
        }
      ]
    }
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:segment:123",
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
    "ext_baz": "I am a custom user property...",
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "secondary",
    "connectors": [
      {
        "connector_id": "fooConnector",
        "at": 0
      },
      {
        "connector_id": "barConnector",
        "at": 1
      }
    ],
    "names": {
      "primary": "Common Road Name 1",
      "rules": [
        {
          "variant": "common",
          "value": "Common Road Name 1",
          "between": [
            0,
            0.5
          ]
        },
        {
          "variant": "short",
          "value": "SRN1",
          "between": [
            0,
            0.5
          ]
        },
        {
          "variant": "common",
          "value": "Common Road Name 2",
          "between": [
            0.5,
            1
          ]
        }
      ]
    }
  }
}
```

#### ttl
```ttl


```


### Example 41
#### json
```json
{
  "id": "overture:transportation:segment:456",
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
      ],
      [
        2,
        2
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "secondary",
    "connectors": [
      {
        "connector_id": "startConnector",
        "at": 0
      },
      {
        "connector_id": "endConnector",
        "at": 1
      }
    ],
    "names": {
      "primary": "Main Street"
    },
    "sources": [
      {
        "property": "/names/primary",
        "dataset": "OpenStreetMap",
        "record_id": "w12345@1",
        "between": [
          0,
          0.5
        ]
      },
      {
        "property": "",
        "dataset": "OpenStreetMap",
        "record_id": "w67890@1",
        "between": [
          0.5,
          1
        ]
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:segment:456",
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
      ],
      [
        2,
        2
      ]
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "secondary",
    "connectors": [
      {
        "connector_id": "startConnector",
        "at": 0
      },
      {
        "connector_id": "endConnector",
        "at": 1
      }
    ],
    "names": {
      "primary": "Main Street"
    },
    "sources": [
      {
        "property": "/names/primary",
        "dataset": "OpenStreetMap",
        "record_id": "w12345@1",
        "between": [
          0,
          0.5
        ]
      },
      {
        "property": "",
        "dataset": "OpenStreetMap",
        "record_id": "w67890@1",
        "between": [
          0.5,
          1
        ]
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 42
#### json
```json
{
  "id": "overture:transportation:segment:123",
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
    "ext_baz": "I am a custom user property...",
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "secondary",
    "connectors": [
      {
        "connector_id": "fooConnector",
        "at": 0
      },
      {
        "connector_id": "barConnector",
        "at": 1
      }
    ],
    "width_rules": [
      {
        "between": [
          0,
          0.5
        ],
        "value": 1.5
      },
      {
        "between": [
          0.5,
          1
        ],
        "value": 2.0
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:segment:123",
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
    "ext_baz": "I am a custom user property...",
    "theme": "transportation",
    "type": "segment",
    "version": 1,
    "subtype": "road",
    "class": "secondary",
    "connectors": [
      {
        "connector_id": "fooConnector",
        "at": 0
      },
      {
        "connector_id": "barConnector",
        "at": 1
      }
    ],
    "width_rules": [
      {
        "between": [
          0,
          0.5
        ],
        "value": 1.5
      },
      {
        "between": [
          0.5,
          1
        ],
        "value": 2.0
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 43
#### json
```json
{
  "id": "overture:transportation:segment:123",
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
    "class": "motorway",
    "connectors": [
      {
        "connector_id": "fooConnector",
        "at": 0
      },
      {
        "connector_id": "barConnector",
        "at": 1
      }
    ],
    "routes": [
      {
        "name": "I 95",
        "network": "US:I",
        "ref": "95",
        "symbol": "https://upload.wikimedia.org/wikipedia/commons/6/61/I-95.svg",
        "wikidata": "Q94967",
        "between": [
          0,
          0.5
        ]
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:segment:123",
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
    "class": "motorway",
    "connectors": [
      {
        "connector_id": "fooConnector",
        "at": 0
      },
      {
        "connector_id": "barConnector",
        "at": 1
      }
    ],
    "routes": [
      {
        "name": "I 95",
        "network": "US:I",
        "ref": "95",
        "symbol": "https://upload.wikimedia.org/wikipedia/commons/6/61/I-95.svg",
        "wikidata": "Q94967",
        "between": [
          0,
          0.5
        ]
      }
    ]
  }
}
```

#### ttl
```ttl


```


### Example 44
#### json
```json
{
  "id": "overture:transportation:segment:123",
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
    "ext_baz": "I am a custom user property...",
    "theme": "transportation",
    "type": "segment",
    "version": 3,
    "subtype": "road",
    "class": "secondary",
    "subclass": "link",
    "subclass_rules": [
      {
        "value": "link"
      }
    ],
    "connectors": [
      {
        "connector_id": "fooConnector",
        "at": 0
      },
      {
        "connector_id": "barConnector",
        "at": 1
      }
    ],
    "names": {
      "primary": "Common Road Name"
    },
    "road_surface": [
      {
        "value": "gravel"
      }
    ],
    "road_flags": [
      {
        "values": [
          "is_link",
          "is_tunnel"
        ]
      }
    ],
    "level": -1,
    "level_rules": [
      {
        "value": -1
      }
    ],
    "width_rules": [
      {
        "value": 10
      }
    ],
    "speed_limits": [
      {
        "min_speed": {
          "value": 90,
          "unit": "km/h"
        },
        "max_speed": {
          "value": 110,
          "unit": "mph"
        },
        "is_max_speed_variable": true
      },
      {
        "max_speed": {
          "value": 55,
          "unit": "mph"
        },
        "when": {
          "mode": [
            "truck"
          ]
        }
      },
      {
        "max_speed": {
          "value": 30,
          "unit": "km/h"
        },
        "between": [
          0.25,
          0.5
        ],
        "when": {
          "during": "Mo-Sa 09:00-12:00, We 15:00-18:00"
        }
      }
    ],
    "prohibited_transitions": [
      {
        "sequence": [
          {
            "segment_id": "overture:transportation:segment:234",
            "connector_id": "overture:transportation:connector:123"
          }
        ],
        "final_heading": "forward",
        "when": {
          "heading": "forward"
        }
      },
      {
        "sequence": [
          {
            "segment_id": "overture:transportation:segment:456",
            "connector_id": "overture:transportation:connector:345"
          },
          {
            "segment_id": "overture:transportation:segment:567",
            "connector_id": "overture:transportation:connector:456"
          }
        ],
        "final_heading": "backward",
        "when": {
          "heading": "backward"
        }
      }
    ],
    "destinations": [
      {
        "labels": [
          {
            "value": "Seattle",
            "type": "unknown"
          },
          {
            "value": "I 90",
            "type": "route_ref"
          }
        ],
        "symbols": [
          "airport"
        ],
        "when": {
          "heading": "forward"
        },
        "from_connector_id": "overture:transportation:connector:123",
        "to_connector_id": "overture:transportation:connector:123",
        "to_segment_id": "overture:transportation:segment:567",
        "final_heading": "backward"
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:segment:123",
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
    "ext_baz": "I am a custom user property...",
    "theme": "transportation",
    "type": "segment",
    "version": 3,
    "subtype": "road",
    "class": "secondary",
    "subclass": "link",
    "subclass_rules": [
      {
        "value": "link"
      }
    ],
    "connectors": [
      {
        "connector_id": "fooConnector",
        "at": 0
      },
      {
        "connector_id": "barConnector",
        "at": 1
      }
    ],
    "names": {
      "primary": "Common Road Name"
    },
    "road_surface": [
      {
        "value": "gravel"
      }
    ],
    "road_flags": [
      {
        "values": [
          "is_link",
          "is_tunnel"
        ]
      }
    ],
    "level": -1,
    "level_rules": [
      {
        "value": -1
      }
    ],
    "width_rules": [
      {
        "value": 10
      }
    ],
    "speed_limits": [
      {
        "min_speed": {
          "value": 90,
          "unit": "km/h"
        },
        "max_speed": {
          "value": 110,
          "unit": "mph"
        },
        "is_max_speed_variable": true
      },
      {
        "max_speed": {
          "value": 55,
          "unit": "mph"
        },
        "when": {
          "mode": [
            "truck"
          ]
        }
      },
      {
        "max_speed": {
          "value": 30,
          "unit": "km/h"
        },
        "between": [
          0.25,
          0.5
        ],
        "when": {
          "during": "Mo-Sa 09:00-12:00, We 15:00-18:00"
        }
      }
    ],
    "prohibited_transitions": [
      {
        "sequence": [
          {
            "segment_id": "overture:transportation:segment:234",
            "connector_id": "overture:transportation:connector:123"
          }
        ],
        "final_heading": "forward",
        "when": {
          "heading": "forward"
        }
      },
      {
        "sequence": [
          {
            "segment_id": "overture:transportation:segment:456",
            "connector_id": "overture:transportation:connector:345"
          },
          {
            "segment_id": "overture:transportation:segment:567",
            "connector_id": "overture:transportation:connector:456"
          }
        ],
        "final_heading": "backward",
        "when": {
          "heading": "backward"
        }
      }
    ],
    "destinations": [
      {
        "labels": [
          {
            "value": "Seattle",
            "type": "unknown"
          },
          {
            "value": "I 90",
            "type": "route_ref"
          }
        ],
        "symbols": [
          "airport"
        ],
        "when": {
          "heading": "forward"
        },
        "from_connector_id": "overture:transportation:connector:123",
        "to_connector_id": "overture:transportation:connector:123",
        "to_segment_id": "overture:transportation:segment:567",
        "final_heading": "backward"
      }
    ]
  }
}
```

#### ttl
```ttl
@prefix ns1: <osm:> .
@prefix om: <https://w3id.org/ogc/om/> .
@prefix qudt: <http://qudt.org/schema/qudt/> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

[] om:hasLevel -1 ;
    om:hasSpeedLimit [ om:hasMaxSpeed [ qudt:hasUnit "km/h" ;
                    rdf:value 30 ] ;
            om:when "{\"during\":\"Mo-Sa 09:00-12:00, We 15:00-18:00\"}"^^rdf:JSON ],
        [ om:hasMaxSpeed [ qudt:hasUnit "mph" ;
                    rdf:value 55 ] ;
            om:when "{\"mode\":[\"truck\"]}"^^rdf:JSON ],
        [ om:hasMaxSpeed [ qudt:hasUnit "mph" ;
                    rdf:value 110 ] ;
            om:hasMinSpeed [ qudt:hasUnit "km/h" ;
                    rdf:value 90 ] ;
            om:isMaxSpeedVariable true ] ;
    ns1:hasSurfaceType <https://w3id.org/ogc/om/surfaces/gravel> .


```


### Example 45
#### json
```json
{
  "id": "overture:transportation:segment:999",
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
    "class": "footway",
    "subclass": "sidewalk",
    "subclass_rules": [
      {
        "value": "sidewalk"
      }
    ],
    "connectors": [
      {
        "connector_id": "fooConnector",
        "at": 0
      },
      {
        "connector_id": "barConnector",
        "at": 1
      }
    ],
    "road_surface": [
      {
        "value": "paved"
      }
    ]
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld",
  "id": "overture:transportation:segment:999",
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
    "class": "footway",
    "subclass": "sidewalk",
    "subclass_rules": [
      {
        "value": "sidewalk"
      }
    ],
    "connectors": [
      {
        "connector_id": "fooConnector",
        "at": 0
      },
      {
        "connector_id": "barConnector",
        "at": 1
      }
    ],
    "road_surface": [
      {
        "value": "paved"
      }
    ]
  }
}
```

#### ttl
```ttl
@prefix ns1: <osm:> .

[] ns1:hasSurfaceType <https://w3id.org/ogc/om/surfaces/paved> .


```

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
title: segment
description: Segments are paths which can be traveled by people or things. Segments
  are compatible with GeoJSON LineString features.
type: object
properties:
  id:
    $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyDefinitions/id
  geometry:
    description: Segment's geometry which MUST be a LineSting as defined by GeoJSON
      schema.
    unevaluatedProperties: false
    allOf:
    - $ref: https://geojson.org/schema/LineString.json
  properties:
    unevaluatedProperties: false
    required:
    - theme
    - type
    - subtype
    allOf:
    - title: Common Segment Properties
      properties:
        subclass_rules:
          $ref: '#/$defs/propertyContainers/subclassRulesContainer'
        access_restrictions:
          $ref: '#/$defs/propertyContainers/accessContainer'
        level:
          $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyDefinitions/level
          x-jsonld-id: https://w3id.org/ogc/om/hasLevel
        level_rules:
          $ref: '#/$defs/propertyContainers/levelRulesContainer'
    - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/overtureFeaturePropertiesContainer
    - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/namesContainer
    oneOf:
    - title: Road-Specific Properties
      required:
      - class
      properties:
        subtype:
          const: road
        class:
          $ref: '#/$defs/propertyDefinitions/roadClass'
        destinations:
          $ref: '#/$defs/propertyDefinitions/destinations'
        prohibited_transitions:
          $ref: '#/$defs/propertyContainers/prohibitedTransitionsContainer'
        road_surface:
          $ref: '#/$defs/propertyContainers/surfaceContainer'
          x-jsonld-id: osm:hasSurfaceType
          x-jsonld-base: https://w3id.org/ogc/om/surfaces/
        road_flags:
          $ref: '#/$defs/propertyContainers/roadFlagsContainer'
        speed_limits:
          $ref: '#/$defs/propertyContainers/speedLimitsContainer'
          x-jsonld-id: https://w3id.org/ogc/om/hasSpeedLimit
        width_rules:
          $ref: '#/$defs/propertyContainers/widthRulesContainer'
        subclass:
          $ref: '#/$defs/propertyDefinitions/subclass'
    - title: Rail-Specific Properties
      required:
      - class
      properties:
        subtype:
          const: rail
        class:
          $ref: '#/$defs/propertyDefinitions/railClass'
        rail_flags:
          $ref: '#/$defs/propertyContainers/railFlagsContainer'
    - title: Water-Specific Properties
      properties:
        subtype:
          const: water
    properties:
      theme:
        const: transportation
      type:
        const: segment
      subtype:
        description: Broad category of transportation segment.
        type: string
        enum:
        - road
        - rail
        - water
        $comment: Should not be confused with a transport mode. A segment kind has
          an (implied) set of default transport modes.
      connectors:
        description: List of connectors which this segment is physically connected
          to and their relative location. Each connector is a possible routing decision
          point, meaning it defines a place along the segment in which there is possibility
          to transition to other segments which share the same connector.
        type: array
        items:
          type: object
          $comment: Contains the GERS ID and relative position between 0 and 1 of
            a connector feature along the segment.
          unevaluatedProperties: false
          required:
          - connector_id
          - at
          properties:
            connector_id:
              $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyDefinitions/id
            at:
              $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyDefinitions/linearlyReferencedPosition
        uniqueItems: true
        minItems: 2
        default: []
      routes:
        $ref: '#/$defs/propertyDefinitions/routes'
    x-jsonld-id: '@nest'
$defs:
  propertyDefinitions:
    destinationLabelType:
      description: The type of object of the destination label.
      type: string
      enum:
      - street
      - country
      - route_ref
      - toward_route_ref
      - unknown
    destinations:
      description: Describes objects that can be reached by following a transportation
        segment in the same way those objects are described on signposts or ground
        writing that a traveller following the segment would observe in the real world.
        This allows navigation systems to refer to signs and observable writing that
        a traveller actually sees.
      type: array
      items:
        type: object
        unevaluatedProperties: false
        required:
        - from_connector_id
        - to_connector_id
        - to_segment_id
        - final_heading
        anyOf:
        - required:
          - labels
        - required:
          - symbols
        properties:
          labels:
            description: Labeled destinations that can be reached by following the
              segment.
            type: array
            items:
              type: object
              unevaluatedProperties: false
              required:
              - value
              - type
              properties:
                value:
                  description: Names the object that is reached
                  type: string
                  pattern: ^(\S.*)?\S$
                type:
                  $ref: '#/$defs/propertyDefinitions/destinationLabelType'
            minItems: 1
            uniqueItems: true
          symbols:
            description: A collection of symbols or icons present on the sign next
              to current destination label.
            type: array
            items:
              $ref: '#/$defs/propertyDefinitions/destinationSignSymbol'
            uniqueItems: true
            minLength: 1
          from_connector_id:
            description: Identifies the point of physical connection on this segment
              before which the destination sign or marking is visible.
            type: string
          to_segment_id:
            description: Identifies the segment to transition to reach the destination(s)
              labeled on the sign or marking.
            type: string
          to_connector_id:
            description: Identifies the point of physical connection on the segment
              identified by 'to_segment_id' to transition to for reaching the destination(s).
            type: string
          when:
            allOf:
            - $ref: '#/$defs/propertyContainers/headingScopeContainer'
            minProperties: 1
            unevaluatedProperties: false
          final_heading:
            description: Direction of travel on the segment identified by 'to_segment_id'
              that leads to the destination.
            $ref: '#/$defs/propertyDefinitions/heading'
    roadClass:
      description: Captures the kind of road and its position in the road network
        hierarchy.
      type: string
      enum:
      - motorway
      - primary
      - secondary
      - tertiary
      - residential
      - living_street
      - trunk
      - unclassified
      - service
      - pedestrian
      - footway
      - steps
      - path
      - track
      - cycleway
      - bridleway
      - unknown
    railClass:
      description: Captures the kind of rail segment.
      type: string
      enum:
      - funicular
      - light_rail
      - monorail
      - narrow_gauge
      - standard_gauge
      - subway
      - tram
      - unknown
    heading:
      description: Enumerates possible travel headings along segment geometry.
      type: string
      enum:
      - forward
      - backward
    travelMode:
      description: Enumerates possible travel modes. Some modes represent groups of
        modes.
      type: string
      enum:
      - vehicle
      - motor_vehicle
      - car
      - truck
      - motorcycle
      - foot
      - bicycle
      - bus
      - hgv
      - hov
      - emergency
      $comment: motor_vehicle includes car, truck and motorcycle
    destinationSignSymbol:
      description: Indicates what special symbol/icon is present on a signpost, visible
        as road marking or similar.
      type: string
      enum:
      - motorway
      - airport
      - hospital
      - center
      - industrial
      - parking
      - bus
      - train_station
      - rest_area
      - ferry
      - motorroad
      - fuel
      - viewpoint
      - fuel_diesel
      - food
      - lodging
      - info
      - camp_site
      - interchange
      - restrooms
    roadFlag:
      description: Simple flags that can be on or off for a road segment. Specifies
        physical characteristics and can overlap.
      type: string
      enum:
      - is_bridge
      - is_link
      - is_tunnel
      - is_under_construction
      - is_abandoned
      - is_covered
      - is_indoor
    railFlag:
      description: Simple flags that can be on or off for a railway segment. Specifies
        physical characteristics and can overlap.
      type: string
      enum:
      - is_bridge
      - is_tunnel
      - is_under_construction
      - is_abandoned
      - is_covered
      - is_passenger
      - is_freight
      - is_disused
    roadSurface:
      description: Physical surface of the road
      type: string
      enum:
      - unknown
      - paved
      - unpaved
      - gravel
      - dirt
      - paving_stones
      - metal
    routes:
      description: Routes this segment belongs to
      type: array
      items:
        type: object
        unevaluatedProperties: false
        allOf:
        - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/geometricRangeScopeContainer
        properties:
          name:
            description: Full name of the route
            type: string
            minLength: 1
            pattern: ^(\S.*)?\S$
          network:
            description: Name of the highway system this route belongs to
            type: string
            minLength: 1
            pattern: ^(\S.*)?\S$
          ref:
            description: Code or number used to reference the route
            type: string
            minLength: 1
            pattern: ^(\S.*)?\S$
          symbol:
            description: URL or description of route signage
            type: string
            minLength: 1
            pattern: ^(\S.*)?\S$
          wikidata:
            $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyDefinitions/wikidata
    subclass:
      description: Refines expected usage of the segment, must not overlap.
      type: string
      enum:
      - link
      - sidewalk
      - crosswalk
      - parking_aisle
      - driveway
      - alley
      - cycle_crossing
    speed:
      description: A speed value, i.e. a certain number of distance units travelled
        per unit time.
      type: object
      properties:
        value:
          description: Speed value
          type: integer
          minimum: 1
          maximum: 350
          x-jsonld-id: rdf:value
        unit:
          description: Speed unit
          type: string
          enum:
          - km/h
          - mph
          x-jsonld-id: http://qudt.org/schema/qudt/hasUnit
      required:
      - value
      - unit
      unevaluatedProperties: false
    purposeOfUse:
      description: Reason why a person or entity travelling on the transportation
        network is using a particular location.
      type: string
      enum:
      - as_customer
      - at_destination
      - to_deliver
      - to_farm
      - for_forestry
    recognizedStatus:
      description: Status of the person or entity travelling as recognized by authorities
        controlling the particular location
      type: string
      enum:
      - as_permitted
      - as_private
      - as_disabled
      - as_employee
      - as_student
    integerRelation:
      description: "Completes an integer relational expression of the form <lhs> <operator>
        <integer_value>. An example of such an expression is:\n  `{ axle_count: {
        is_more_than: 2 } }`."
      type: object
      unevaluatedProperties: false
      oneOf:
      - required:
        - is_more_than
        properties:
          is_more_than:
            type: integer
      - required:
        - is_at_least
        properties:
          is_at_least:
            type: integer
      - required:
        - is_equal_to
        properties:
          is_equal_to:
            type: integer
      - required:
        - is_at_most
        properties:
          is_at_most:
            type: integer
      - required:
        - is_less_than
        properties:
          is_less_than:
            type: integer
    vehicleScopeDimension:
      description: Enumerates possible vehicle dimensions for use in restrictions
      type: string
      enum:
      - axle_count
      - height
      - length
      - weight
      - width
    vehicleScopeComparison:
      description: Enumerates possible comparison operators for use in scoping
      type: string
      enum:
      - greater_than
      - greater_than_equal
      - equal
      - less_than
      - less_than_equal
    vehicleScopeUnit:
      description: Parent enum of both length and width for use in vehicle scoping
      anyOf:
      - $ref: '#/$defs/propertyDefinitions/lengthUnit'
      - $ref: '#/$defs/propertyDefinitions/weightUnit'
    lengthUnit:
      description: Enumerates length units supported by the Overture schema.
      $comment: Keep in sync with `combobulib/measure.py`.
      type: string
      enum:
      - in
      - ft
      - yd
      - mi
      - cm
      - m
      - km
    lengthValueWithUnit:
      description: Combines a length value with a length unit.
      type: object
      unevaluatedProperties: false
      required:
      - value
      - unit
      properties:
        value:
          type: number
          minimum: 0
        unit:
          $ref: '#/$defs/propertyDefinitions/lengthUnit'
    lengthRelation:
      description: "Completes a length relational expression of the form <lhs> <operator>
        <length_value>. An example of such an expression is:\n  `{ height: { is_less_than:
        { value: 3, unit: 'm' } } }`."
      type: object
      unevaluatedProperties: false
      oneOf:
      - required:
        - is_more_than
        properties:
          is_more_than:
            allOf:
            - $ref: '#/$defs/propertyDefinitions/lengthValueWithUnit'
      - required:
        - is_at_least
        properties:
          is_at_least:
            allOf:
            - $ref: '#/$defs/propertyDefinitions/lengthValueWithUnit'
      - required:
        - is_equal_to
        properties:
          is_equal_to:
            allOf:
            - $ref: '#/$defs/propertyDefinitions/lengthValueWithUnit'
      - required:
        - is_at_most
        properties:
          is_at_most:
            allOf:
            - $ref: '#/$defs/propertyDefinitions/lengthValueWithUnit'
      - required:
        - is_less_than
        properties:
          is_less_than:
            allOf:
            - $ref: '#/$defs/propertyDefinitions/lengthValueWithUnit'
    weightUnit:
      description: Enumerates weight units supported by the Overture schema.
      $comment: Keep in sync with `combobulib/measure.py`.
      type: string
      enum:
      - oz
      - lb
      - st
      - lt
      - g
      - kg
      - t
    weightValueWithUnit:
      description: Combines a weight value with a weight unit.
      type: object
      unevaluatedProperties: false
      required:
      - value
      - unit
      properties:
        value:
          type: number
          minimum: 0
        unit:
          $ref: '#/$defs/propertyDefinitions/weightUnit'
    weightRelation:
      description: "Completes a weight relational expression of the form <lhs> <operator>
        <weight_value>. An example of such an expression is:\n  `{ weight: { is_more_than:
        { value: 2, unit: 't' } } }`."
      type: object
      unevaluatedProperties: false
      oneOf:
      - required:
        - is_more_than
        properties:
          is_more_than:
            allOf:
            - $ref: '#/$defs/propertyDefinitions/weightValueWithUnit'
      - required:
        - is_at_least
        properties:
          is_at_least:
            allOf:
            - $ref: '#/$defs/propertyDefinitions/weightValueWithUnit'
      - required:
        - is_equal_to
        properties:
          is_equal_to:
            allOf:
            - $ref: '#/$defs/propertyDefinitions/weightValueWithUnit'
      - required:
        - is_at_most
        properties:
          is_at_most:
            allOf:
            - $ref: '#/$defs/propertyDefinitions/weightValueWithUnit'
      - required:
        - is_less_than
        properties:
          is_less_than:
            allOf:
            - $ref: '#/$defs/propertyDefinitions/weightValueWithUnit'
    width:
      type: number
      exclusiveMinimum: 0
    sequenceEntry:
      description: A segment/connector pair in a prohibited transition sequence.
      type: object
      required:
      - connector_id
      - segment_id
      properties:
        connector_id:
          description: Identifies the point of physical connection between the previous
            segment in the sequence and the segment in this sequence entry.
          type: string
        segment_id:
          description: Identifies the segment that the previous segment in the sequence
            is physically connected to via the sequence entry's connector.
          type: string
  propertyContainers:
    headingScopeContainer:
      description: Properties defining travel headings that match a rule.
      properties:
        heading:
          $ref: '#/$defs/propertyDefinitions/heading'
    purposeOfUseScopeContainer:
      description: Properties defining usage purposes that match a rule.
      properties:
        using:
          type: array
          items:
            $ref: '#/$defs/propertyDefinitions/purposeOfUse'
          uniqueItems: true
          minLength: 1
    temporalScopeContainer:
      $comment: Temporal scoping properties defining the time spans when a recurring
        rule is active.
      properties:
        during:
          $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyDefinitions/openingHours
    travelModeScopeContainer:
      description: Properties defining travel modes that match a rule.
      type: object
      properties:
        mode:
          description: Travel mode(s) to which the rule applies
          type: array
          items:
            $ref: '#/$defs/propertyDefinitions/travelMode'
          uniqueItems: true
          minLength: 1
    recognizedStatusScopeContainer:
      description: Properties defining statuses that match a rule.
      properties:
        recognized:
          type: array
          items:
            $ref: '#/$defs/propertyDefinitions/recognizedStatus'
          uniqueItems: true
          minLength: 1
    vehicleScopeContainer:
      description: Properties defining vehicle attributes for which a rule is active.
      type: object
      properties:
        vehicle:
          description: Vehicle attributes for which the rule applies
          type: array
          uniqueItems: true
          minLength: 1
          items:
            description: An individual vehicle scope rule
            type: object
            unevaluatedProperties: false
            required:
            - dimension
            - comparison
            - value
            properties:
              dimension:
                $ref: '#/$defs/propertyDefinitions/vehicleScopeDimension'
              comparison:
                $ref: '#/$defs/propertyDefinitions/vehicleScopeComparison'
              value:
                type: number
                minimum: 0
                x-jsonld-id: rdf:value
              unit:
                $ref: '#/$defs/propertyDefinitions/vehicleScopeUnit'
                x-jsonld-id: http://qudt.org/vocab/unit/
    speedLimitsContainer:
      description: Rules governing speed on this road segment
      type: array
      items:
        description: An individual speed limit rule
        $comment: 'TODO: Speed limits probably have directionality, so should factor
          out a headingScopeContainer for this purpose and use it to introduce an
          optional direction property in each rule.'
        type: object
        anyOf:
        - required:
          - min_speed
        - required:
          - max_speed
        allOf:
        - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/geometricRangeScopeContainer
        unevaluatedProperties: false
        properties:
          min_speed:
            $ref: '#/$defs/propertyDefinitions/speed'
            x-jsonld-id: https://w3id.org/ogc/om/hasMinSpeed
          max_speed:
            $ref: '#/$defs/propertyDefinitions/speed'
            x-jsonld-id: https://w3id.org/ogc/om/hasMaxSpeed
          is_max_speed_variable:
            description: Indicates a variable speed corridor
            type: boolean
            default: false
            x-jsonld-id: https://w3id.org/ogc/om/isMaxSpeedVariable
          when:
            allOf:
            - $ref: '#/$defs/propertyContainers/temporalScopeContainer'
            - $ref: '#/$defs/propertyContainers/headingScopeContainer'
            - $ref: '#/$defs/propertyContainers/purposeOfUseScopeContainer'
            - $ref: '#/$defs/propertyContainers/recognizedStatusScopeContainer'
            - $ref: '#/$defs/propertyContainers/travelModeScopeContainer'
            - $ref: '#/$defs/propertyContainers/vehicleScopeContainer'
            minProperties: 1
            unevaluatedProperties: false
            x-jsonld-id: https://w3id.org/ogc/om/when
            x-jsonld-type: '@json'
      minLength: 1
      uniqueItems: true
    accessContainer:
      description: Rules governing access to this road segment
      type: array
      items:
        type: object
        unevaluatedProperties: false
        allOf:
        - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/geometricRangeScopeContainer
        required:
        - access_type
        properties:
          access_type:
            type: string
            enum:
            - allowed
            - denied
            - designated
          when:
            allOf:
            - $ref: '#/$defs/propertyContainers/temporalScopeContainer'
            - $ref: '#/$defs/propertyContainers/headingScopeContainer'
            - $ref: '#/$defs/propertyContainers/purposeOfUseScopeContainer'
            - $ref: '#/$defs/propertyContainers/recognizedStatusScopeContainer'
            - $ref: '#/$defs/propertyContainers/travelModeScopeContainer'
            - $ref: '#/$defs/propertyContainers/vehicleScopeContainer'
            minProperties: 1
            unevaluatedProperties: false
        minLength: 1
        uniqueItems: true
    prohibitedTransitionsContainer:
      description: Rules preventing transitions from this segment to another segment.
      type: array
      items:
        type: object
        unevaluatedProperties: false
        allOf:
        - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/geometricRangeScopeContainer
        required:
        - sequence
        - final_heading
        properties:
          sequence:
            description: Ordered sequence of connector/segment pairs that it is prohibited
              to follow from this segment.
            type: array
            items:
              description: Pair of segment and connector IDs along the sequence
              $ref: '#/$defs/propertyDefinitions/sequenceEntry'
            minItems: 1
            uniqueItems: true
          final_heading:
            description: Direction of travel that is prohibited on the destination
              segment of the sequence.
            $ref: '#/$defs/propertyDefinitions/heading'
          when:
            allOf:
            - $ref: '#/$defs/propertyContainers/headingScopeContainer'
            - $ref: '#/$defs/propertyContainers/temporalScopeContainer'
            - $ref: '#/$defs/propertyContainers/purposeOfUseScopeContainer'
            - $ref: '#/$defs/propertyContainers/recognizedStatusScopeContainer'
            - $ref: '#/$defs/propertyContainers/travelModeScopeContainer'
            - $ref: '#/$defs/propertyContainers/vehicleScopeContainer'
            minProperties: 1
            unevaluatedProperties: false
    roadFlagsContainer:
      description: Set of boolean attributes applicable to roads. May be specified
        either as a single flag array of flag values, or as an array of flag rules.
      type: array
      items:
        type: object
        allOf:
        - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/geometricRangeScopeContainer
        unevaluatedProperties: false
        properties:
          values:
            type: array
            items:
              $ref: '#/$defs/propertyDefinitions/roadFlag'
            uniqueItems: true
            minLength: 1
      uniqueItems: true
      minLength: 1
    railFlagsContainer:
      description: Set of boolean attributes applicable to railways. May be specified
        either as a single flag array of flag values, or as an array of flag rules.
      type: array
      items:
        type: object
        allOf:
        - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/geometricRangeScopeContainer
        unevaluatedProperties: false
        properties:
          values:
            type: array
            items:
              $ref: '#/$defs/propertyDefinitions/railFlag'
            uniqueItems: true
            minLength: 1
      uniqueItems: true
      minLength: 1
    levelRulesContainer:
      description: Defines the Z-order, i.e. stacking order, of the road segment.
      type: array
      items:
        description: A single level rule defining the Z-order, i.e. stacking order,
          applicable within a given scope on the road segment.
        type: object
        allOf:
        - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/geometricRangeScopeContainer
        unevaluatedProperties: false
        required:
        - value
        properties:
          value:
            $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyDefinitions/level
    subclassRulesContainer:
      description: Set of subclasses scoped along segment
      type: array
      items:
        type: object
        allOf:
        - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/geometricRangeScopeContainer
        unevaluatedProperties: false
        properties:
          value:
            $ref: '#/$defs/propertyDefinitions/subclass'
    surfaceContainer:
      description: Physical surface of the road. May either be specified as a single
        global value for the segment, or as an array of surface rules.
      type: array
      items:
        type: object
        allOf:
        - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/geometricRangeScopeContainer
        unevaluatedProperties: false
        properties:
          value:
            $ref: '#/$defs/propertyDefinitions/roadSurface'
            x-jsonld-id: '@id'
      minItems: 1
      uniqueItems: true
      $comment: We should likely restrict the available surface types to the subset
        of the common OSM surface=* tag values that are useful both for routing and
        for map tile rendering.
    widthRulesContainer:
      description: 'Edge-to-edge width of the road modeled by this segment, in meters.

        Examples: (1) If this segment models a carriageway without sidewalk, this
        value represents the edge-to-edge width of the carriageway, inclusive of any
        shoulder. (2) If this segment models a sidewalk by itself, this value represents
        the edge-to-edge width of the sidewalk. (3) If this segment models a combined
        sidewalk and carriageway, this value represents the edge-to-edge width inclusive
        of sidewalk.'
      type: array
      items:
        type: object
        allOf:
        - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/geometricRangeScopeContainer
        required:
        - value
        properties:
          value:
            $ref: '#/$defs/propertyDefinitions/width'
        unevaluatedProperties: false
      minItems: 1
      uniqueItems: true
x-jsonld-prefixes:
  om: https://w3id.org/ogc/om/
  qudt: http://qudt.org/schema/qudt/

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/schema.yaml)


# JSON-LD Context

```jsonld
{
  "@context": {
    "id": {},
    "type": {},
    "coordinates": {},
    "bbox": {},
    "geometry": {},
    "between": {},
    "value": {},
    "subclass_rules": {},
    "access_type": {},
    "when": {
      "@context": {
        "during": {},
        "heading": {},
        "using": {},
        "recognized": {},
        "mode": {},
        "vehicle": {
          "@context": {
            "dimension": {},
            "comparison": {},
            "value": "rdf:value",
            "unit": "http://qudt.org/vocab/unit/"
          }
        }
      }
    },
    "access_restrictions": {},
    "level": "om:hasLevel",
    "level_rules": {},
    "theme": {},
    "version": {},
    "sources": {
      "@context": {
        "property": {},
        "dataset": {},
        "license": {},
        "record_id": {},
        "update_time": {},
        "confidence": {}
      }
    },
    "names": {
      "@context": {
        "primary": {},
        "common": {},
        "rules": {
          "@context": {
            "side": {},
            "variant": {},
            "language": {},
            "perspectives": {
              "@context": {
                "mode": {},
                "countries": {}
              }
            }
          }
        }
      }
    },
    "subtype": {},
    "class": {},
    "labels": {},
    "symbols": {},
    "from_connector_id": {},
    "to_segment_id": {},
    "to_connector_id": {},
    "final_heading": {},
    "destinations": {},
    "sequence": {
      "@context": {
        "segment_id": {}
      }
    },
    "prohibited_transitions": {},
    "road_surface": {
      "@context": {
        "@base": "https://w3id.org/ogc/om/surfaces/",
        "value": "@id"
      },
      "@id": "osm:hasSurfaceType"
    },
    "values": {},
    "road_flags": {},
    "speed_limits": {
      "@context": {
        "min_speed": {
          "@context": {
            "value": "rdf:value",
            "unit": "qudt:hasUnit"
          },
          "@id": "om:hasMinSpeed"
        },
        "max_speed": {
          "@context": {
            "value": "rdf:value",
            "unit": "qudt:hasUnit"
          },
          "@id": "om:hasMaxSpeed"
        },
        "is_max_speed_variable": "om:isMaxSpeedVariable",
        "when": {
          "@context": {
            "during": {},
            "heading": {},
            "using": {},
            "recognized": {},
            "mode": {},
            "vehicle": {
              "@context": {
                "dimension": {},
                "comparison": {},
                "value": "rdf:value",
                "unit": "http://qudt.org/vocab/unit/"
              }
            }
          },
          "@id": "om:when",
          "@type": "@json"
        }
      },
      "@id": "om:hasSpeedLimit"
    },
    "width_rules": {},
    "subclass": {},
    "rail_flags": {},
    "connector_id": {},
    "at": {},
    "connectors": {},
    "name": {},
    "network": {},
    "ref": {},
    "symbol": {},
    "wikidata": {},
    "routes": {},
    "properties": "@nest",
    "address": {
      "@id": "vcard:hasAddress",
      "@type": "@id",
      "@context": {
        "freeform": "rdf:value",
        "locality": "vcard:hasLocality",
        "postCode": "vcard:hasPostalCode",
        "region": "vcard:hasRegion",
        "countryName": "vcard:hasCountryName"
      }
    },
    "allNames": {
      "@id": "@nest",
      "@context": {
        "primary": "skos:prefLabel",
        "common": {
          "@id": "skos:altLabel",
          "@container": "@language"
        }
      }
    },
    "om": "https://w3id.org/ogc/om/",
    "qudt": "http://qudt.org/schema/qudt/",
    "vcard": "http://www.w3.org/2006/vcard/ns#",
    "rdf": "http://www.w3.org/1999/02/22-rdf-syntax-ns#",
    "skos": "http://www.w3.org/2004/02/skos/core#",
    "@version": 1.1
  }
}
```

You can find the full JSON-LD context here:
[context.jsonld](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/segment/context.jsonld)


# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-overturemaps](https://github.com/ogcincubator/bblocks-overturemaps)
* Path: `_sources/schemas/transportation/segment`

