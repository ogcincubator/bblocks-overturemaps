
# part (Schema)

`ogc.overturemaps.schemas.buildings.building_part` *v0.1*

A single building part. Parts describe their shape and color and other properties. Each building part must contain the building with which it is associated.

[*Status*](http://www.opengis.net/def/status): Under development

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
    - $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/defs.yaml#/$defs/propertyContainers/overtureFeaturePropertiesContainer
    - $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/defs.yaml#/$defs/propertyContainers/namesContainer
    - $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/defs.yaml#/$defs/propertyContainers/levelContainer
    - $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/buildings/defs.yaml#/$defs/propertyContainers/shapeContainer
    required:
    - building_id
    properties:
      building_id:
        description: The building ID to which this part belongs
        type: string

```

Links to the schema:

* YAML version: [schema.yaml](https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/buildings/building_part/schema.json)
* JSON version: [schema.json](https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/buildings/building_part/schema.yaml)


# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-overturemaps](https://github.com/ogcincubator/bblocks-overturemaps)
* Path: `_sources/schemas/buildings/building_part`

