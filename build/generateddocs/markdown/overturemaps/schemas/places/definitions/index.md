
# Shared places properties (Schema)

`ogc.overturemaps.schemas.places.definitions` *v0.1*

Common schema definitions for places theme

[*Status*](http://www.opengis.net/def/status): Under development

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
description: Common schema definitions for places theme
$defs:
  typeDefinitions:
    category:
      description: Category of a place.
      type: string
      minLength: 1
      pattern: ^[a-z0-9]+(_[a-z0-9]+)*$

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/places/definitions/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/places/definitions/schema.yaml)


# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-overturemaps](https://github.com/ogcincubator/bblocks-overturemaps)
* Path: `_sources/schemas/places/definitions`

