
# building (Schema)

`ogc.overturemaps.schemas.buildings.building` *v0.1*

A building is a man-made structure with a roof that exists permanently in one place. Buildings are compatible with GeoJSON Polygon features.

[*Status*](http://www.opengis.net/def/status): Under development

## Examples

### Example 1
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


### Example 2
#### json
```json
{
  "id": "overture:buildings:building:1234",
  "type": "Feature",
  "geometry": {
    "type": "MultiPolygon",
    "coordinates": [
      [
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
    ]
  },
  "properties": {
    "ext_foo": "I am a customer user property.",
    "ext_bar": "Me too!",
    "theme": "buildings",
    "type": "building",
    "version": 0
  }
}
```


### Example 3
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
    "type": "building",
    "version": 1,
    "level": 1,
    "height": 21.34,
    "num_floors": 4,
    "num_floors_underground": 1,
    "subtype": "transportation",
    "class": "parking",
    "is_underground": false,
    "sources": [
      {
        "property": "",
        "dataset": "microsoftMLBuildings,",
        "confidence": 1
      },
      {
        "property": "/properties/height",
        "dataset": "metaLidarExtractions,",
        "confidence": 0.95
      }
    ]
  }
}
```


### Example 4
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
    "theme": "buildings",
    "type": "building",
    "version": 1,
    "sources": [
      {
        "dataset": "MyGreatDataset",
        "property": "/geometry",
        "update_time": "2024-04-26T23:55:01-08:00",
        "confidence": 0.3,
        "license": "beep"
      }
    ]
  }
}
```


### Example 5
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
    "names": {
      "primary": "Empire State Building"
    }
  }
}
```


### Example 6
#### json
```json
{
  "id": "overture:buildings:building:1234",
  "type": "Feature",
  "properties": {
    "ext_foo": "I am a customer user property.",
    "ext_bar": "Me too!",
    "theme": "buildings",
    "type": "building",
    "version": 1,
    "names": {
      "primary": "The White house",
      "common": {
        "es": "La Casa Blanca"
      },
      "rules": [
        {
          "variant": "official",
          "value": "The White House"
        },
        {
          "variant": "alternate",
          "value": "White House"
        }
      ]
    }
  },
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
  }
}
```


### Example 7
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
    "names": {
      "primary": "Local value",
      "common": {
        "ru-Latn": "Language Script",
        "en-US": "Language Region"
      },
      "rules": [
        {
          "variant": "official",
          "language": "es",
          "value": "Official Name"
        },
        {
          "variant": "short",
          "language": "es",
          "value": "Official Spanish Name"
        },
        {
          "variant": "alternate",
          "language": "ru",
          "value": "Official Russian Name"
        }
      ]
    }
  }
}
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
          -117.1710888,
          32.7238481
        ],
        [
          -117.1711025,
          32.7239038
        ],
        [
          -117.1711923,
          32.7238882
        ],
        [
          -117.1712198,
          32.724
        ],
        [
          -117.1712713,
          32.7242091
        ],
        [
          -117.1706665,
          32.7243145
        ],
        [
          -117.1705738,
          32.7239379
        ],
        [
          -117.1707783,
          32.7239022
        ],
        [
          -117.1710888,
          32.7238481
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
    "level": 1,
    "names": {
      "primary": "Valentina by Alta"
    },
    "num_floors": 8,
    "subtype": "commercial",
    "class": "commercial",
    "sources": [
      {
        "property": "",
        "dataset": "OpenStreetMap"
      }
    ]
  }
}
```


### Example 9
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
    "version": 1
  }
}
```


### Example 10
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
    "version": 1
  }
}
```

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
title: building
description: A building is a man-made structure with a roof that exists permanently
  in one place. Buildings are compatible with GeoJSON Polygon features.
type: object
properties:
  id:
    $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyDefinitions/id
  geometry:
    description: A regular building's geometry is defined as its footprint or roofprint
      (if traced from aerial/satellite imagery). It MUST be a Polygon or MultiPolygon
      as defined by the GeoJSON schema.
    unevaluatedProperties: false
    oneOf:
    - $ref: https://geojson.org/schema/Polygon.json
    - $ref: https://geojson.org/schema/MultiPolygon.json
  properties:
    unevaluatedProperties: false
    allOf:
    - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/overtureFeaturePropertiesContainer
    - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/namesContainer
    - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/levelContainer
    - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/buildings/definitions/schema.yaml#/$defs/propertyContainers/shapeContainer
    required:
    - theme
    - type
    properties:
      theme:
        const: buildings
      type:
        const: building
      subtype:
        description: A broad category of the building type/purpose. When the current
          use of the building does not match the built purpose, the subtype should
          be set to represent the current use of the building.
        type: string
        enum:
        - agricultural
        - civic
        - commercial
        - education
        - entertainment
        - industrial
        - medical
        - military
        - outbuilding
        - religious
        - residential
        - service
        - transportation
      class:
        description: Further delineation of the building's built purpose.
        type: string
        enum:
        - agricultural
        - allotment_house
        - apartments
        - barn
        - beach_hut
        - boathouse
        - bridge_structure
        - bungalow
        - bunker
        - cabin
        - carport
        - cathedral
        - chapel
        - church
        - civic
        - college
        - commercial
        - cowshed
        - detached
        - digester
        - dormitory
        - dwelling_house
        - factory
        - farm
        - farm_auxiliary
        - fire_station
        - garage
        - garages
        - ger
        - glasshouse
        - government
        - grandstand
        - greenhouse
        - guardhouse
        - hangar
        - hospital
        - hotel
        - house
        - houseboat
        - hut
        - industrial
        - kindergarten
        - kiosk
        - library
        - manufacture
        - military
        - monastery
        - mosque
        - office
        - outbuilding
        - parking
        - pavilion
        - post_office
        - presbytery
        - public
        - religious
        - residential
        - retail
        - roof
        - school
        - semi
        - semidetached_house
        - service
        - shed
        - shrine
        - silo
        - slurry_tank
        - sports_centre
        - sports_hall
        - stable
        - stadium
        - static_caravan
        - stilt_house
        - storage_tank
        - sty
        - supermarket
        - synagogue
        - temple
        - terrace
        - toilets
        - train_station
        - transformer_tower
        - transportation
        - trullo
        - university
        - warehouse
        - wayside_shrine
      has_parts:
        description: Flag indicating whether the building has parts
        type: boolean

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/buildings/building/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/buildings/building/schema.yaml)


# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-overturemaps](https://github.com/ogcincubator/bblocks-overturemaps)
* Path: `_sources/schemas/buildings/building`

