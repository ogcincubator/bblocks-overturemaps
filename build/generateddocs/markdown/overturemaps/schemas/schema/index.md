
# Overture Maps Schema (Schema)

`ogc.overturemaps.schemas.schema` *v0.1*

A JSON Schema for the canonical GeoJSON form of Overture Maps Features.

[*Status*](http://www.opengis.net/def/status): Under development

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
title: Overture Maps Schema
description: A JSON Schema for the canonical GeoJSON form of Overture Maps Features.
type: object
unevaluatedProperties: false
allOf:
- $ref: https://opengeospatial.github.io/bblocks/annotated-schemas/geo/common/data_types/geojson/schema.yaml
  $comment: Every Overture feature IS A GeoJSON feature
oneOf:
- if:
    properties:
      properties:
        properties:
          theme:
            enum:
            - addresses
          type:
            enum:
            - address
  then:
    $ref: https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/addresses/address/schema.yaml
  else:
    propertyNames: false
- if:
    properties:
      properties:
        properties:
          theme:
            enum:
            - base
          type:
            enum:
            - bathymetry
  then:
    $ref: https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/base/bathymetry/schema.yaml
  else:
    propertyNames: false
- if:
    properties:
      properties:
        properties:
          theme:
            enum:
            - base
          type:
            enum:
            - infrastructure
  then:
    $ref: https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/base/infrastructure/schema.yaml
  else:
    propertyNames: false
- if:
    properties:
      properties:
        properties:
          theme:
            enum:
            - base
          type:
            enum:
            - land
  then:
    $ref: https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/base/land/schema.yaml
  else:
    propertyNames: false
- if:
    properties:
      properties:
        properties:
          theme:
            enum:
            - base
          type:
            enum:
            - land_cover
  then:
    $ref: https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/base/land_cover/schema.yaml
  else:
    propertyNames: false
- if:
    properties:
      properties:
        properties:
          theme:
            enum:
            - base
          type:
            enum:
            - land_use
  then:
    $ref: https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/base/land_use/schema.yaml
  else:
    propertyNames: false
- if:
    properties:
      properties:
        properties:
          theme:
            enum:
            - base
          type:
            enum:
            - water
  then:
    $ref: https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/base/water/schema.yaml
  else:
    propertyNames: false
- if:
    properties:
      properties:
        properties:
          theme:
            enum:
            - buildings
          type:
            enum:
            - building
  then:
    $ref: https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/buildings/building/schema.yaml
  else:
    propertyNames: false
- if:
    properties:
      properties:
        properties:
          theme:
            enum:
            - buildings
          type:
            enum:
            - building_part
  then:
    $ref: https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/buildings/building_part/schema.yaml
  else:
    propertyNames: false
- if:
    properties:
      properties:
        properties:
          theme:
            enum:
            - divisions
          type:
            enum:
            - division_boundary
  then:
    $ref: https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/divisions/division_boundary/schema.yaml
  else:
    propertyNames: false
- if:
    properties:
      properties:
        properties:
          theme:
            enum:
            - divisions
          type:
            enum:
            - division
  then:
    $ref: https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/divisions/division/schema.yaml
  else:
    propertyNames: false
- if:
    properties:
      properties:
        properties:
          theme:
            enum:
            - divisions
          type:
            enum:
            - division_area
  then:
    $ref: https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/divisions/division_area/schema.yaml
  else:
    propertyNames: false
- if:
    properties:
      properties:
        properties:
          theme:
            enum:
            - places
          type:
            enum:
            - place
  then:
    $ref: https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/places/place/schema.yaml
  else:
    propertyNames: false
- if:
    properties:
      properties:
        properties:
          theme:
            enum:
            - transportation
          type:
            enum:
            - connector
  then:
    $ref: https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/transportation/connector/schema.yaml
  else:
    propertyNames: false
- if:
    properties:
      properties:
        properties:
          theme:
            enum:
            - transportation
          type:
            enum:
            - segment
  then:
    $ref: https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/transportation/segment/schema.yaml
  else:
    propertyNames: false

```

Links to the schema:

* YAML version: [schema.yaml](https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/schema/schema.json)
* JSON version: [schema.json](https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/schema/schema.yaml)


# JSON-LD Context

```jsonld
{
  "@context": {
    "Feature": "geojson:Feature",
    "FeatureCollection": "geojson:FeatureCollection",
    "GeometryCollection": "geojson:GeometryCollection",
    "LineString": "geojson:LineString",
    "MultiLineString": "geojson:MultiLineString",
    "MultiPoint": "geojson:MultiPoint",
    "MultiPolygon": "geojson:MultiPolygon",
    "Point": "geojson:Point",
    "Polygon": "geojson:Polygon",
    "features": {
      "@container": "@set",
      "@id": "geojson:features"
    },
    "type": "@type",
    "id": "@id",
    "properties": "@nest",
    "geometry": {
      "@context": {
        "coordinates": {
          "@container": "@list",
          "@id": "geojson:coordinates"
        }
      },
      "@id": "geojson:geometry"
    },
    "bbox": {
      "@container": "@list",
      "@id": "geojson:bbox"
    },
    "geojson": "https://purl.org/geojson/vocab#",
    "@version": 1.1
  }
}
```

You can find the full JSON-LD context here:
[context.jsonld](https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/schema/context.jsonld)


# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-overturemaps](https://github.com/ogcincubator/bblocks-overturemaps)
* Path: `_sources/schemas/schema`

