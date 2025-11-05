
# connector (Schema)

`ogc.overturemaps.schemas.transportation.connector` *v0.1*

Connectors create physical connections between segments. Connectors are compatible with GeoJSON Point features.

[*Status*](http://www.opengis.net/def/status): Under development

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
title: connector
description: Connectors create physical connections between segments. Connectors are
  compatible with GeoJSON Point features.
type: object
properties:
  id:
    $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/defs.yaml#/$defs/propertyDefinitions/id
  geometry:
    description: Connector's geometry which MUST be a Point as defined by GeoJSON
      schema.
    unevaluatedProperties: false
    allOf:
    - $ref: https://geojson.org/schema/Point.json
  properties:
    unevaluatedProperties: false
    allOf:
    - $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/defs.yaml#/$defs/propertyContainers/overtureFeaturePropertiesContainer

```

Links to the schema:

* YAML version: [schema.yaml](https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/transportation/connector/schema.json)
* JSON version: [schema.json](https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/transportation/connector/schema.yaml)


# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-overturemaps](https://github.com/ogcincubator/bblocks-overturemaps)
* Path: `_sources/schemas/transportation/connector`

