
# Global Entity Reference System identifier (Schema)

`ogc.overturemaps.schemas.gers` *v0.1*

The Global Entity Reference System (GERS) is a universal framework for structuring and matching map data across systems.

[*Status*](http://www.opengis.net/def/status): Under development

## Description

The Global Entity Reference System (GERS) is a universal framework for structuring and matching map data across systems.
GERS, coupled with Overture datasets, is a potential standard for identifying and referencing the physical and
conceptual entities we've defined in our world. It's also a mechanism that can simplify the integration and exchange of
data layers.

GERS provides stable identifiers called GERS IDs for real-world geospatial entities across data releases and maintains
consistency when entities appear in multiple source datasets.
## Schema

```yaml
type: string
description: "A feature ID. This may be an ID associated with the Global Entity Reference
  System (GERS) if\u2014and-only-if the feature represents an entity that is part
  of GERS."
minLength: 1
pattern: ^(\S.*)?\S$

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/gers/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/gers/schema.yaml)

## Sources

* [GERS documentation](https://docs.overturemaps.org/gers/)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-overturemaps](https://github.com/ogcincubator/bblocks-overturemaps)
* Path: `_sources/schemas/gers`

