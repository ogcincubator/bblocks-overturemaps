
# Land Cover schema (Schema)

`ogc.overturemaps.schemas.base.land_cover` *v0.1*

Representation of the Earth's natural surfaces

[*Status*](http://www.opengis.net/def/status): Under development

## Examples

### Example 1
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

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
title: land_cover
description: Representation of the Earth's natural surfaces
type: object
properties:
  id:
    $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyDefinitions/id
  geometry:
    unevaluatedProperties: false
    oneOf:
    - $ref: https://geojson.org/schema/Polygon.json
    - $ref: https://geojson.org/schema/MultiPolygon.json
  properties:
    unevaluatedProperties: false
    allOf:
    - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/overtureFeaturePropertiesContainer
    - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/levelContainer
    - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/cartographyContainer
    required:
    - theme
    - type
    - subtype
    properties:
      theme:
        const: base
      type:
        const: land_cover
      subtype:
        description: type of surface represented
        type: string
        enum:
        - barren
        - crop
        - forest
        - grass
        - mangrove
        - moss
        - shrub
        - snow
        - urban
        - wetland

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/base/land_cover/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/base/land_cover/schema.yaml)


# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-overturemaps](https://github.com/ogcincubator/bblocks-overturemaps)
* Path: `_sources/schemas/base/land_cover`

