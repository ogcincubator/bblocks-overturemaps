
# Shared divisions properties (Schema)

`ogc.overturemaps.schemas.divisions.definitions` *v0.1*

Common schema definitions for divisions theme

[*Status*](http://www.opengis.net/def/status): Under development

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
description: Common schema definitions for divisions theme
$defs:
  propertyDefinitions:
    placetype:
      description: Category of the division from a finite, hierarchical, ordered list
        of categories (e.g. country, region, locality, etc.) similar to a Who's on
        First placetype.
      type: string
      enum:
      - country
      - dependency
      - macroregion
      - region
      - macrocounty
      - county
      - localadmin
      - locality
      - borough
      - macrohood
      - neighborhood
      - microhood
    hierarchy:
      description: 'A hierarchy of divisions, with the first entry being a country;
        each subsequent entry, if any, being a division that is a direct child of
        the previous entry; and the last entry representing the division that contains
        the hierarchy.

        For example, a hierarchy for the United States is simply [United States].
        A hierarchy for the U.S. state of New Hampshire would be [United States, New
        Hampshire], and a hierarchy for the city of Concord, NH would be [United States,
        New Hampshire, Merrimack County, Concord].'
      type: array
      items:
        $ref: '#/$defs/propertyDefinitions/hierarchyItem'
      minItems: 1
      uniqueItems: true
    hierarchyItem:
      description: One division in a hierarchy
      type: object
      unevaluatedProperties: false
      required:
      - division_id
      - name
      - subtype
      properties:
        division_id:
          description: ID of the division
          allOf:
          - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyDefinitions/id
        subtype:
          $ref: '#/$defs/propertyDefinitions/placetype'
        name:
          description: Primary name of the division
          type: string
          minLength: 1
          pattern: ^(\S.*)?\S$
    perspectives:
      description: Political perspectives from which division is viewed.
      type: object
      unevaluatedProperties: false
      required:
      - mode
      - countries
      properties:
        mode:
          description: Whether perspective holder accept or dispute this division.
          type: string
          enum:
          - accepted_by
          - disputed_by
        countries:
          description: Countries holding the given mode of perspective.
          type: array
          items:
            $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyDefinitions/iso3166_1Alpha2CountryCode
          minItems: 1
          uniqueItems: true
    capitalOfDivisionItem:
      description: One division that has capital
      type: object
      unevaluatedProperties: false
      required:
      - division_id
      - subtype
      properties:
        division_id:
          description: ID of the division
          allOf:
          - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyDefinitions/id
        subtype:
          $ref: '#/$defs/propertyDefinitions/placetype'

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/divisions/definitions/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/divisions/definitions/schema.yaml)


# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-overturemaps](https://github.com/ogcincubator/bblocks-overturemaps)
* Path: `_sources/schemas/divisions/definitions`

