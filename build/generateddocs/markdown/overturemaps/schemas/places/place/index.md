
# place (Schema)

`ogc.overturemaps.schemas.places.place` *v0.1*

A Place is a point representation of a real-world facility, service, or amenity. Place features are compatible with GeoJSON Point features.

[*Status*](http://www.opengis.net/def/status): Under development

## Examples

### Example 1
#### json
```json
{
  "id": "timestamp-utc",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      0,
      0
    ]
  },
  "properties": {
    "categories": {
      "primary": "some_category"
    },
    "theme": "places",
    "type": "place",
    "version": 1,
    "operating_status": "open"
  }
}
```


### Example 2
#### json
```json
{
  "id": "overture:places:place:1",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      0,
      0
    ]
  },
  "properties": {
    "categories": {
      "primary": "the1_category_you_want_first",
      "alternate": [
        "another_category"
      ]
    },
    "confidence": 0.9,
    "websites": [
      "https://www.example.com"
    ],
    "emails": [
      "info@example.com"
    ],
    "socials": [
      "https://www.twitter.com/example"
    ],
    "phones": [
      "+32 1207"
    ],
    "brand": {
      "names": {
        "primary": "My Sweet POI Brand"
      },
      "wikidata": "Q1000"
    },
    "addresses": [
      {
        "freeform": "770 Broadway, Floor 8",
        "locality": "New York"
      },
      {
        "freeform": "770 Broadway, #802",
        "locality": "New York",
        "region": "US-NY",
        "country": "US"
      }
    ],
    "theme": "places",
    "type": "place",
    "version": 1,
    "names": {
      "primary": "My Sweet POI",
      "common": {
        "es": "Something in Spanish"
      },
      "rules": [
        {
          "variant": "short",
          "value": "MSPOI"
        }
      ]
    },
    "operating_status": "open"
  }
}
```


### Example 3
#### json
```json
{
  "id": "overture:places:place:1",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      0,
      0
    ]
  },
  "properties": {
    "categories": {
      "primary": "some_category"
    },
    "confidence": 0.9,
    "brand": {
      "names": {
        "primary": "My Sweet POI Brand"
      },
      "wikidata": "Q1000"
    },
    "addresses": [
      {
        "freeform": "770 Broadway, Floor 8",
        "locality": "New York"
      },
      {
        "freeform": "770 Brodway, #802",
        "locality": "New York",
        "region": "US-NY",
        "country": "US"
      }
    ],
    "theme": "places",
    "type": "place",
    "version": 1,
    "sources": [
      {
        "property": "",
        "dataset": "metaPlaces",
        "record_id": "10101"
      },
      {
        "property": "/properties/brand",
        "dataset": "msftPlaces",
        "record_id": "10df72b8"
      }
    ],
    "names": {
      "primary": "My Sweet POI",
      "common": {
        "es": "Something in Spanish"
      },
      "rules": [
        {
          "variant": "short",
          "value": "MSPOI"
        }
      ]
    },
    "operating_status": "open"
  }
}
```


### Example 4
#### json
```json
{
  "geometry": {
    "coordinates": [
      0,
      0
    ],
    "type": "Point"
  },
  "id": "overture:places:place:1",
  "properties": {
    "addresses": [
      {
        "freeform": "770 Broadway, Floor 8",
        "locality": "New York"
      },
      {
        "country": "US",
        "freeform": "770 Broadway #802",
        "locality": "New York",
        "region": "US-NY"
      }
    ],
    "brand": {
      "names": {
        "primary": "Example"
      },
      "wikidata": "Q1000"
    },
    "emails": [
      "info@example.com"
    ],
    "phones": [
      "+32 1207"
    ],
    "socials": [
      "https://www.twitter.com/example"
    ],
    "theme": "places",
    "type": "place",
    "version": 1,
    "websites": [
      "https://www.example.com"
    ],
    "operating_status": "open"
  },
  "type": "Feature"
}
```


### Example 5
#### json
```json
{
  "id": "overture:places:place:66",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      0,
      0
    ]
  },
  "properties": {
    "basic_category": "casual_eatery",
    "categories": {
      "primary": "gas_station_sushi",
      "alternate": [
        "just_for_fun"
      ]
    },
    "confidence": 0.9,
    "websites": [
      "https://www.example.com"
    ],
    "emails": [
      "info@example.com"
    ],
    "socials": [
      "https://www.twitter.com/example"
    ],
    "phones": [
      "+32 1207"
    ],
    "brand": {
      "names": {
        "primary": "11-7"
      },
      "wikidata": "Q1000"
    },
    "addresses": [
      {
        "freeform": "1 Wasserman Way",
        "locality": "District 11"
      }
    ],
    "theme": "places",
    "type": "place",
    "version": 1,
    "names": {
      "primary": "11-7",
      "common": {
        "en": "Eleven Seven"
      },
      "rules": [
        {
          "variant": "short",
          "value": "MSPOI"
        }
      ]
    },
    "operating_status": "open"
  }
}
```


### Example 6
#### json
```json
{
  "id": "overture:places:place:1",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      0,
      0
    ]
  },
  "properties": {
    "categories": {
      "primary": "some_category"
    },
    "confidence": 0.9,
    "websites": [
      "https://www.example.com/"
    ],
    "emails": [
      "info@example.com"
    ],
    "socials": [
      "https://www.twitter.com/example"
    ],
    "phones": [
      "+32 1207"
    ],
    "brand": {
      "names": {
        "primary": "My Sweet POI Brand"
      },
      "wikidata": "Q1000"
    },
    "addresses": [
      {
        "freeform": "770 Broadway, Floor 8",
        "locality": "New York"
      },
      {
        "freeform": "770 Broadway, #802",
        "locality": "New York",
        "region": "US-NY",
        "country": "US"
      }
    ],
    "theme": "places",
    "type": "place",
    "version": 1,
    "sources": [
      {
        "property": "",
        "dataset": "metaPlaces",
        "record_id": "10101"
      },
      {
        "property": "/properties/brand",
        "dataset": "msftPlaces",
        "record_id": "10df72b8"
      }
    ],
    "names": {
      "primary": "My Sweet POI",
      "common": {
        "es": "Something in Spanish"
      },
      "rules": [
        {
          "variant": "short",
          "value": "MSPOI"
        }
      ]
    },
    "operating_status": "permanently_closed"
  }
}
```


### Example 7
#### json
```json
{
  "id": "overture:places:place:1",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      0,
      0
    ]
  },
  "properties": {
    "categories": {
      "primary": "some_category"
    },
    "confidence": 0.9,
    "websites": [
      "https://www.example.com"
    ],
    "emails": [
      "info@example.com"
    ],
    "socials": [
      "https://www.twitter.com/example"
    ],
    "phones": [
      "+32 1207"
    ],
    "brand": {
      "names": {
        "primary": "My Sweet POI Brand"
      },
      "wikidata": "Q1000"
    },
    "operating_status": "open",
    "addresses": [
      {
        "freeform": "770 Broadway, Floor 8",
        "locality": "New York"
      },
      {
        "freeform": "770 Brodway, #802",
        "locality": "New York",
        "region": "US-NY",
        "country": "US"
      }
    ],
    "theme": "places",
    "type": "place",
    "version": 1,
    "sources": [
      {
        "property": "",
        "dataset": "metaPlaces",
        "record_id": "10101"
      },
      {
        "property": "/properties/brand",
        "dataset": "msftPlaces",
        "record_id": "10df72b8"
      }
    ],
    "names": {
      "primary": "My Sweet POI",
      "common": {
        "es": "Something in Spanish"
      },
      "rules": [
        {
          "variant": "short",
          "value": "MSPOI"
        }
      ]
    }
  }
}
```


### Example 8
#### json
```json
{
  "geometry": {
    "coordinates": [
      0,
      0
    ],
    "type": "Point"
  },
  "id": "overture:places:place:1",
  "properties": {
    "addresses": [
      {
        "freeform": "770 Broadway, Floor 8",
        "locality": "New York"
      },
      {
        "country": "US",
        "freeform": "770 Broadway #802",
        "locality": "New York",
        "region": "US-NY"
      }
    ],
    "brand": {
      "names": {
        "primary": "Example"
      },
      "wikidata": "Q1000"
    },
    "categories": {
      "primary": "some_category"
    },
    "emails": [
      "info@example.com"
    ],
    "phones": [
      "+32 1207"
    ],
    "socials": [
      "https://www.twitter.com/example"
    ],
    "theme": "places",
    "type": "place",
    "version": 1,
    "websites": [
      "https://www.example.com"
    ],
    "operating_status": "open"
  },
  "type": "Feature"
}
```

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
title: place
description: A Place is a point representation of a real-world facility, service,
  or amenity. Place features are compatible with GeoJSON Point features.
type: object
properties:
  id:
    $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyDefinitions/id
  geometry:
    description: Place's geometry which MUST be a Point as defined by GeoJSON schema.
    unevaluatedProperties: false
    oneOf:
    - $ref: https://geojson.org/schema/Point.json
  properties:
    unevaluatedProperties: false
    allOf:
    - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/overtureFeaturePropertiesContainer
    - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/namesContainer
    required:
    - operating_status
    properties:
      theme:
        const: places
      type:
        const: place
      categories:
        description: 'The categories of the place. Complete list is available on

          GitHub: https://github.com/OvertureMaps/schema/blob/main/docs/schema/concepts/by-theme/places/overture_categories.csv

          '
        type: object
        required:
        - primary
        properties:
          primary:
            description: The primary or main category of the place. This can be empty.
            $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/places/definitions/schema.yaml#/$defs/typeDefinitions/category
          alternate:
            description: Alternate categories of the place. Some places might fit
              into two categories, e.g. a book store and a coffee shop. In such a
              case, the primary category can be augmented with additional applicable
              categories.
            type: array
            items:
              $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/places/definitions/schema.yaml#/$defs/typeDefinitions/category
            uniqueItems: true
      basic_category:
        description: The basic level category of a place. At present this is a mapping
          of the categories.primary entry to a new, simplified name. This mapping
          can be 1:1 or M:1 from the existing primary.categories entry. If the entry
          is currently empty in categories.primary, this entry will be empty.  This
          type of categorization is a cognitive science model that is relevant for
          taxonomy and ontology development that shows the most broadest and general
          category name that is most often found in the middle of a general-to-specific
          hierarchy, with generalization proceeding upward and specialization proceeding
          downward.  The full list of basic level categories is available at:(todo)
        type: string
        $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/places/definitions/schema.yaml#/$defs/typeDefinitions/category
      confidence:
        description: The confidence of the existence of the place. It's a number between
          0 and 1. 0 means that we're sure that the place doesn't exist (anymore).
          1 means that we're sure that the place exists. If there's no value for the
          confidence, it means that we don't have any confidence information. Places
          with operating_status set to 'closed' will have a confidence score of 0
        type: number
        minimum: 0
        maximum: 1
      websites:
        description: The websites of the place.
        type: array
        items:
          type: string
          format: uri
        uniqueItems: true
        minItems: 1
      socials:
        description: The social media URLs of the place.
        type: array
        items:
          type: string
          format: uri
        uniqueItems: true
        minItems: 1
      emails:
        description: The email addresses of the place.
        type: array
        items:
          type: string
          format: email
        uniqueItems: true
        minItems: 1
      phones:
        description: The phone numbers of the place.
        type: array
        items:
          type: string
        uniqueItems: true
        minItems: 1
      brand:
        description: The brand of the place. A location with multiple brands is modeled
          as multiple separate places, each with its own brand.
        type: object
        allOf:
        - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/namesContainer
        properties:
          wikidata:
            $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyDefinitions/wikidata
      addresses:
        description: The addresses of the place.
        type: array
        items:
          $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyDefinitions/address
        uniqueItems: true
        minItems: 1
      operating_status:
        description: Indicates the operating status of a place, can be one of ["open",
          "permanently_closed", "temporarily_closed"].  This is not an indication
          of 'opening hours' or that the place is open/closed at the current time-of-day
          or day-of-week.
        type: string
        enum:
        - open
        - permanently_closed
        - temporarily_closed

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/places/place/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/places/place/schema.yaml)


# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-overturemaps](https://github.com/ogcincubator/bblocks-overturemaps)
* Path: `_sources/schemas/places/place`

