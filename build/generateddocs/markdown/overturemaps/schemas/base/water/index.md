
# water (Schema)

`ogc.overturemaps.schemas.base.water` *v0.1*

Physical representations of inland and ocean marine surfaces. Translates `natural` and `waterway` tags from OpenStreetMap.

[*Status*](http://www.opengis.net/def/status): Under development

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
title: water
description: Physical representations of inland and ocean marine surfaces. Translates
  `natural` and `waterway` tags from OpenStreetMap.
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
    - $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/defs.yaml#/$defs/propertyContainers/levelContainer
    - $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/defs.yaml#/$defs/propertyContainers/namesContainer
    - $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/base/defs.yaml#/$defs/propertyContainers/osmPropertiesContainer
    required:
    - subtype
    - class
    properties:
      subtype:
        description: The type of water body such as an river, ocean or lake.
        default:
        - water
        type: string
        enum:
        - canal
        - human_made
        - lake
        - ocean
        - physical
        - pond
        - reservoir
        - river
        - spring
        - stream
        - wastewater
        - water
      class:
        description: Further description of the type of water
        default:
        - water
        type: string
        enum:
        - basin
        - bay
        - blowhole
        - canal
        - cape
        - ditch
        - dock
        - drain
        - fairway
        - fish_pass
        - fishpond
        - geyser
        - hot_spring
        - lagoon
        - lake
        - moat
        - ocean
        - oxbow
        - pond
        - reflecting_pool
        - reservoir
        - river
        - salt_pond
        - sea
        - sewage
        - shoal
        - spring
        - strait
        - stream
        - swimming_pool
        - tidal_channel
        - wastewater
        - water
        - water_storage
        - waterfall
      is_salt:
        description: Is it salt water or not
        type: boolean
      is_intermittent:
        description: Is it intermittent water or not
        type: boolean

```

Links to the schema:

* YAML version: [schema.yaml](https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/base/water/schema.json)
* JSON version: [schema.json](https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/base/water/schema.yaml)


# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-overturemaps](https://github.com/ogcincubator/bblocks-overturemaps)
* Path: `_sources/schemas/base/water`

