
# part (Schema)

`ogc.overturemaps.schemas.buildings.building_part` *v0.1*

A single building part. Parts describe their shape and color and other properties. Each building part must contain the building with which it is associated.

[*Status*](http://www.opengis.net/def/status): Under development

## Examples

### Example 1
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


### Example 2
#### json
```json
{
  "id": "overture:buildings:part:2345",
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
    "theme": "buildings",
    "type": "building_part",
    "version": 1,
    "level": 1,
    "building_id": "abc1234",
    "names": {
      "primary": "East Wing"
    },
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
        "dataset": "OpenStreetMap"
      }
    ]
  }
}
```


### Example 3
#### json
```json
{
  "id": "overture:buildings:part:100",
  "type": "Feature",
  "geometry": {
    "type": "Polygon",
    "coordinates": [
      [
        [
          -117.1707971,
          32.7240658
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
          -117.1707949,
          32.7240226
        ],
        [
          -117.1707279,
          32.7240319
        ],
        [
          -117.1707635,
          32.7241786
        ],
        [
          -117.1708208,
          32.7241677
        ],
        [
          -117.1707971,
          32.7240658
        ]
      ]
    ]
  },
  "properties": {
    "building_id": "1234",
    "ext_foo": "I am a customer user property.",
    "ext_bar": "Me too!",
    "theme": "buildings",
    "type": "building_part",
    "version": 1,
    "level": 1,
    "num_floors": 8,
    "sources": [
      {
        "property": "",
        "dataset": "OpenStreetMap"
      }
    ]
  }
}
```


### Example 4
#### json
```json
{
  "id": "overture:buildings:part:101",
  "type": "Feature",
  "geometry": {
    "type": "Polygon",
    "coordinates": [
      [
        [
          -117.1712198,
          32.724
        ],
        [
          -117.1711923,
          32.7238882
        ],
        [
          -117.1711025,
          32.7239038
        ],
        [
          -117.1710888,
          32.7238481
        ],
        [
          -117.1707783,
          32.7239022
        ],
        [
          -117.1707949,
          32.7240226
        ],
        [
          -117.1707279,
          32.7240319
        ],
        [
          -117.1707635,
          32.7241786
        ],
        [
          -117.1708208,
          32.7241677
        ],
        [
          -117.1707971,
          32.7240658
        ],
        [
          -117.1712198,
          32.724
        ]
      ]
    ]
  },
  "properties": {
    "building_id": "1234",
    "ext_foo": "I am a customer user property.",
    "ext_bar": "Me too!",
    "theme": "buildings",
    "type": "building_part",
    "version": 1,
    "level": 1,
    "num_floors": 3,
    "sources": [
      {
        "property": "",
        "dataset": "OpenStreetMap"
      }
    ]
  }
}
```

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
title: part
description: A single building part. Parts describe their shape and color and other
  properties. Each building part must contain the building with which it is associated.
type: object
properties:
  geometry:
    description: The part's geometry. It must be a polygon or multipolygon.
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
    - building_id
    properties:
      theme:
        const: buildings
      type:
        const: building_part
      building_id:
        description: The building ID to which this part belongs
        type: string

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/buildings/building_part/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/buildings/building_part/schema.yaml)


# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-overturemaps](https://github.com/ogcincubator/bblocks-overturemaps)
* Path: `_sources/schemas/buildings/building_part`

