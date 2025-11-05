
# boundary (Schema)

`ogc.overturemaps.schemas.divisions.division_boundary` *v0.1*

Boundaries represent borders between divisions of the same subtype. Some boundaries may be disputed by the divisions on one or both sides.

[*Status*](http://www.opengis.net/def/status): Under development

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
title: boundary
description: Boundaries represent borders between divisions of the same subtype. Some
  boundaries may be disputed by the divisions on one or both sides.
type: object
properties:
  id:
    $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/defs.yaml#/$defs/propertyDefinitions/id
  geometry:
    description: Boundary's geometry which MUST be a LineString or MultiLineString
      as defined by the GeoJSON schema.
    unevaluatedProperties: false
    oneOf:
    - $ref: https://geojson.org/schema/LineString.json
    - $ref: https://geojson.org/schema/MultiLineString.json
  properties:
    unevaluatedProperties: false
    allOf:
    - $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/defs.yaml#/$defs/propertyContainers/overtureFeaturePropertiesContainer
    - if:
        properties:
          subtype:
            enum:
            - country
      then:
        required:
        - subtype
        - class
        - division_ids
        - is_land
        - is_territorial
        not:
          required:
          - country
      else:
        required:
        - subtype
        - class
        - division_ids
        - is_land
        - is_territorial
        - country
    oneOf:
    - properties:
        is_land:
          const: true
    - properties:
        is_territorial:
          const: true
    properties:
      subtype:
        $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/divisions/defs.yaml#/$defs/propertyDefinitions/placetype
      class:
        type: string
        enum:
        - land
        - maritime
      is_land:
        description: A boolean to indicate whether or not the feature geometry represents
          the land-clipped, non-maritime boundary. The geometry can be used for map
          rendering, cartographic display, and similar purposes.
        type: boolean
      is_territorial:
        description: A boolean to indicate whether or not the feature geometry represents
          Overture's best approximation of this place's maritime boundary. For coastal
          places, this would tend to include the water area. The geometry can be used
          for data processing, reverse-geocoding, and similar purposes.
        type: boolean
      division_ids:
        description: 'Identifies the two divisions to the left and right, respectively,
          of the boundary line. The left- and right-hand sides of the boundary are
          considered from the perspective of a person standing on the line facing
          in the direction in which the geometry is oriented, i.e. facing toward the
          end of the line.

          The first array element is the Overture ID of the left division. The second
          element is the Overture ID of the right division.'
        type: array
        items:
          $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/defs.yaml#/$defs/propertyDefinitions/id
        minItems: 2
        maxItems: 2
        uniqueItems: true
      country:
        description: 'ISO 3166-1 alpha-2 country code of the country or country-like
          entity that both sides of the boundary share.

          This property will be present on boundaries between two regions, counties,
          or similar entities within the same country, but will not be present on
          boundaries between two countries or country-like entities.'
        allOf:
        - $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/defs.yaml#/$defs/propertyDefinitions/iso3166_1Alpha2CountryCode
      region:
        description: 'ISO 3166-2 principal subdivision code of the subdivision-like
          entity that both sides of the boundary share.

          This property will be present on boundaries between two counties, localadmins
          or similar entities within the same principal subdivision, but will not
          be present on boundaries between different principal subdivisions or countries.'
        allOf:
        - $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/defs.yaml#/$defs/propertyDefinitions/iso3166_2SubdivisionCode
      is_disputed:
        description: 'Indicator if there are entities disputing this division boundary.
          Information about entities disputing this boundary should be included in
          perspectives property.

          This property should also be true if boundary between two entities is unclear
          and this is "best guess". So having it true and no perspectives gives map
          creators reason not to fully trust the boundary, but use it if they have
          no other.'
        type: boolean
      perspectives:
        description: "Political perspectives from which this division boundary is
          considered to be an accurate representation.\nIf this property is absent,
          then this boundary is not known to be disputed from any political perspective.
          Consequently, there is only one boundary feature representing the entire
          real world entity.\nIf this property is present, it means the boundary represents
          one of several alternative perspectives on the same real-world entity.\nThere
          are two modes of perspective:\n\n  1. `accepted_by` means the representation
          of the boundary is\n     accepted by the listed entities and would be included
          on\n     a map drawn from their perspective.\n\n  2. `disputed_by` means
          the representation of the boundary is\n     disputed by the listed entities
          and would be excluded\n     from a map drawn from their perspective.\n    \nWhen
          drawing a map from the perspective of a given country, one would start by
          gathering all the undisputed boundary (with no `perspectives` property),
          and then adding to that first all boundary explicitly accepted by the country,
          and second all boundary not explicitly disputed by the country."
        allOf:
        - $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/divisions/defs.yaml#/$defs/propertyDefinitions/perspectives

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/divisions/division_boundary/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/divisions/division_boundary/schema.yaml)


# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-overturemaps](https://github.com/ogcincubator/bblocks-overturemaps)
* Path: `_sources/schemas/divisions/division_boundary`

