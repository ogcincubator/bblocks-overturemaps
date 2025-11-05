
# land (Schema)

`ogc.overturemaps.schemas.base.land` *v0.1*

Physical representations of land surfaces. Global land derived from the inverse of OSM Coastlines. Translates `natural` tags from OpenStreetMap.

[*Status*](http://www.opengis.net/def/status): Under development

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
title: land
description: Physical representations of land surfaces. Global land derived from the
  inverse of OSM Coastlines. Translates `natural` tags from OpenStreetMap.
type: object
properties:
  id:
    $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/defs.yaml#/$defs/propertyDefinitions/id
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
    - $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/defs.yaml#/$defs/propertyContainers/overtureFeaturePropertiesContainer
    - $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/defs.yaml#/$defs/propertyContainers/namesContainer
    - $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/defs.yaml#/$defs/propertyContainers/levelContainer
    - $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/base/defs.yaml#/$defs/propertyContainers/osmPropertiesContainer
    required:
    - subtype
    - class
    properties:
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
        $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/base/defs.yaml#/$defs/propertyDefinitions/elevation
      surface:
        $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/base/defs.yaml#/$defs/propertyDefinitions/surface

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/base/land/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/base/land/schema.yaml)


# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-overturemaps](https://github.com/ogcincubator/bblocks-overturemaps)
* Path: `_sources/schemas/base/land`

