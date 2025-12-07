
# Transportation Connector schema (Schema)

`ogc.overturemaps.schemas.transportation.connector` *v0.1*

Connectors create physical connections between segments. Connectors are compatible with GeoJSON Point features.

[*Status*](http://www.opengis.net/def/status): Under development

## Examples

### Example 1
#### json
```json
{
  "id": "timestamp-with-tz-offset",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      0,
      0
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "connector",
    "version": 0
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/connector/context.jsonld",
  "id": "timestamp-with-tz-offset",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      0,
      0
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "connector",
    "version": 0
  }
}
```

#### ttl
```ttl


```


### Example 2
#### json
```json
{
  "id": "overture:transportation:connector:example",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      0,
      0
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "connector",
    "version": 0
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/connector/context.jsonld",
  "id": "overture:transportation:connector:example",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      0,
      0
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "connector",
    "version": 0
  }
}
```

#### ttl
```ttl


```


### Example 3
#### json
```json
{
  "id": "overture:transportation:connector:example",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      0,
      0
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "connector",
    "version": 0
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/connector/context.jsonld",
  "id": "overture:transportation:connector:example",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      0,
      0
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "connector",
    "version": 0
  }
}
```

#### ttl
```ttl


```


### Example 4
#### json
```json
{
  "id": "overture:transportation:example:simple-turn-restriction-connector1",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      -113.57831482025354,
      50.018860947117304
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "connector",
    "version": 0
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/connector/context.jsonld",
  "id": "overture:transportation:example:simple-turn-restriction-connector1",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      -113.57831482025354,
      50.018860947117304
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "connector",
    "version": 0
  }
}
```

#### ttl
```ttl


```


### Example 5
#### json
```json
{
  "id": "overture:transportation:example:simple-turn-restriction-connector2",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      -113.57851814418316,
      50.01923724443006
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "connector",
    "version": 1
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/connector/context.jsonld",
  "id": "overture:transportation:example:simple-turn-restriction-connector2",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      -113.57851814418316,
      50.01923724443006
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "connector",
    "version": 1
  }
}
```

#### ttl
```ttl


```


### Example 6
#### json
```json
{
  "id": "overture:transportation:example:simple-turn-restriction-connector3",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      -113.57816369068271,
      50.01919400284882
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "connector",
    "version": 1
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/connector/context.jsonld",
  "id": "overture:transportation:example:simple-turn-restriction-connector3",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      -113.57816369068271,
      50.01919400284882
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "connector",
    "version": 1
  }
}
```

#### ttl
```ttl


```


### Example 7
#### json
```json
{
  "id": "overture:transportation:example:via-turn-restriction-connector1",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      -71.11234408150312,
      42.30149091145671
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "connector",
    "version": 1
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/connector/context.jsonld",
  "id": "overture:transportation:example:via-turn-restriction-connector1",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      -71.11234408150312,
      42.30149091145671
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "connector",
    "version": 1
  }
}
```

#### ttl
```ttl


```


### Example 8
#### json
```json
{
  "id": "overture:transportation:example:via-turn-restriction-connector2",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      -71.11248901211202,
      42.3013264259736
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "connector",
    "version": 1
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/connector/context.jsonld",
  "id": "overture:transportation:example:via-turn-restriction-connector2",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      -71.11248901211202,
      42.3013264259736
    ]
  },
  "properties": {
    "theme": "transportation",
    "type": "connector",
    "version": 1
  }
}
```

#### ttl
```ttl


```

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
title: connector
description: Connectors create physical connections between segments. Connectors are
  compatible with GeoJSON Point features.
type: object
properties:
  id:
    $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyDefinitions/id
  geometry:
    description: Connector's geometry which MUST be a Point as defined by GeoJSON
      schema.
    unevaluatedProperties: false
    allOf:
    - $ref: https://geojson.org/schema/Point.json
  properties:
    unevaluatedProperties: false
    allOf:
    - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/overtureFeaturePropertiesContainer
    required:
    - theme
    - type
    properties:
      theme:
        const: transportation
      type:
        const: connector

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/connector/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/connector/schema.yaml)


# JSON-LD Context

```jsonld
{
  "@context": {
    "id": {},
    "type": {},
    "coordinates": {},
    "bbox": {},
    "geometry": {},
    "theme": {},
    "version": {},
    "sources": {
      "@context": {
        "between": {},
        "property": {},
        "dataset": {},
        "license": {},
        "record_id": {},
        "update_time": {},
        "confidence": {}
      }
    },
    "properties": {},
    "wikidata": {
      "@id": "rdfs:seeAlso",
      "@type": "@id",
      "@context": {
        "@base": "https://www.wikidata.org/wiki/"
      }
    },
    "address": {
      "@id": "vcard:hasAddress",
      "@type": "@id",
      "@context": {
        "freeform": "rdf:value",
        "locality": "vcard:hasLocality",
        "postCode": "vcard:hasPostalCode",
        "region": "vcard:hasRegion",
        "countryName": "vcard:hasCountryName"
      }
    },
    "allNames": {
      "@id": "@nest",
      "@context": {
        "primary": "skos:prefLabel",
        "common": {
          "@id": "skos:altLabel",
          "@container": "@language"
        }
      }
    },
    "om": "https://w3id.org/ogc/om/",
    "vcard": "http://www.w3.org/2006/vcard/ns#",
    "rdf": "http://www.w3.org/1999/02/22-rdf-syntax-ns#",
    "skos": "http://www.w3.org/2004/02/skos/core#",
    "@version": 1.1
  }
}
```

You can find the full JSON-LD context here:
[context.jsonld](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/transportation/connector/context.jsonld)


# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-overturemaps](https://github.com/ogcincubator/bblocks-overturemaps)
* Path: `_sources/schemas/transportation/connector`

