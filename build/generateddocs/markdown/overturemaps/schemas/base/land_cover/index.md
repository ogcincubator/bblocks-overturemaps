
# land_cover (Schema)

`ogc.overturemaps.schemas.base.land_cover` *v0.1*

Representation of the Earth's natural surfaces

[*Status*](http://www.opengis.net/def/status): Under development

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
title: land_cover
description: Representation of the Earth's natural surfaces
type: object
properties:
  id:
    $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/defs.yaml#/$defs/propertyDefinitions/id
  geometry:
    unevaluatedProperties: false
    oneOf:
    - $ref: https://geojson.org/schema/Polygon.json
    - $ref: https://geojson.org/schema/MultiPolygon.json
  properties:
    unevaluatedProperties: false
    allOf:
    - $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/defs.yaml#/$defs/propertyContainers/overtureFeaturePropertiesContainer
    - $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/defs.yaml#/$defs/propertyContainers/levelContainer
    - $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/defs.yaml#/$defs/propertyContainers/cartographyContainer
    required:
    - subtype
    properties:
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

* YAML version: [schema.yaml](https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/base/land_cover/schema.json)
* JSON version: [schema.json](https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/base/land_cover/schema.yaml)


# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-overturemaps](https://github.com/ogcincubator/bblocks-overturemaps)
* Path: `_sources/schemas/base/land_cover`

