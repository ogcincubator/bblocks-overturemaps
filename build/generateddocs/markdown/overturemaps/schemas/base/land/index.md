
# Land schema (Schema)

`ogc.overturemaps.schemas.base.land` *v0.1*

Physical representations of land surfaces. Global land derived from the inverse of OSM Coastlines. Translates `natural` tags from OpenStreetMap.

[*Status*](http://www.opengis.net/def/status): Under development

## Examples

### Example 1
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

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
title: land
description: Physical representations of land surfaces. Global land derived from the
  inverse of OSM Coastlines. Translates `natural` tags from OpenStreetMap.
type: object
properties:
  id:
    $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyDefinitions/id
  geometry:
    unevaluatedProperties: false
    oneOf:
    - $ref: https://geojson.org/schema/Point.json
    - $ref: https://geojson.org/schema/LineString.json
    - $ref: https://geojson.org/schema/Polygon.json
    - $ref: https://geojson.org/schema/MultiPolygon.json
  properties:
    unevaluatedProperties: false
    allOf:
    - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/overtureFeaturePropertiesContainer
    - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/namesContainer
    - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/levelContainer
    - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/base/definitions/schema.yaml#/$defs/propertyContainers/osmPropertiesContainer
    required:
    - theme
    - type
    - subtype
    - class
    properties:
      theme:
        const: base
      type:
        const: land
      subtype:
        description: Further description of the type of land cover, such as forest,
          glacier, grass, or a physical feature, such as a mountain peak.
        default:
        - land
        type: string
        enum:
        - crater
        - desert
        - forest
        - glacier
        - grass
        - land
        - physical
        - reef
        - rock
        - sand
        - shrub
        - tree
        - wetland
      class:
        description: Further classification of type of landcover
        default:
        - land
        type: string
        enum:
        - archipelago
        - bare_rock
        - beach
        - cave_entrance
        - cliff
        - desert
        - dune
        - fell
        - forest
        - glacier
        - grass
        - grassland
        - heath
        - hill
        - island
        - islet
        - land
        - meadow
        - meteor_crater
        - mountain_range
        - peak
        - peninsula
        - plateau
        - reef
        - ridge
        - rock
        - saddle
        - sand
        - scree
        - scrub
        - shingle
        - shrub
        - shrubbery
        - stone
        - tree
        - tree_row
        - tundra
        - valley
        - volcanic_caldera_rim
        - volcano
        - wetland
        - wood
      elevation:
        $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/base/definitions/schema.yaml#/$defs/propertyDefinitions/elevation
      surface:
        $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/base/definitions/schema.yaml#/$defs/propertyDefinitions/surface

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/base/land/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/base/land/schema.yaml)


# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-overturemaps](https://github.com/ogcincubator/bblocks-overturemaps)
* Path: `_sources/schemas/base/land`

