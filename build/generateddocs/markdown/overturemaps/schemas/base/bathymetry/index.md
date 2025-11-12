
# Bathymetry schema (Schema)

`ogc.overturemaps.schemas.base.bathymetry` *v0.1*

Topographic representation of an underwater area, such as a part of the ocean floor.

[*Status*](http://www.opengis.net/def/status): Under development

## Examples

### Example 1
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

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
title: bathymetry
description: Topographic representation of an underwater area, such as a part of the
  ocean floor.
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
    - depth
    - theme
    - type
    properties:
      theme:
        const: base
      type:
        const: bathymetry
      depth:
        $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/base/definitions/schema.yaml#/$defs/propertyDefinitions/depth

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/base/bathymetry/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/base/bathymetry/schema.yaml)


# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-overturemaps](https://github.com/ogcincubator/bblocks-overturemaps)
* Path: `_sources/schemas/base/bathymetry`

