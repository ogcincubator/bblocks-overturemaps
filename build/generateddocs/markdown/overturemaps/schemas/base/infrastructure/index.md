
# Infrastructure Schema (Schema)

`ogc.overturemaps.schemas.base.infrastructure` *v0.1*

Various features from OpenStreetMap such as bridges, airport runways, aerialways, or communication towers and lines.

[*Status*](http://www.opengis.net/def/status): Under development

## Examples

### Example 1
#### json
```json
{
  "id": "08b2748cc1383fff0001b38438099b73",
  "type": "Feature",
  "geometry": {
    "type": "Polygon",
    "coordinates": [
      [
        [
          -85.6743541,
          42.9676009
        ],
        [
          -85.6743623,
          42.9674649
        ],
        [
          -85.6744114,
          42.9674803
        ],
        [
          -85.6744559,
          42.9674919
        ],
        [
          -85.6745302,
          42.9675058
        ],
        [
          -85.6746036,
          42.9675151
        ],
        [
          -85.6746959,
          42.9675171
        ],
        [
          -85.675835,
          42.9674967
        ],
        [
          -85.6758985,
          42.9674915
        ],
        [
          -85.6759656,
          42.967483
        ],
        [
          -85.6760399,
          42.9674711
        ],
        [
          -85.676099,
          42.9674566
        ],
        [
          -85.6761817,
          42.9674324
        ],
        [
          -85.676227,
          42.9674184
        ],
        [
          -85.6762149,
          42.9675911
        ],
        [
          -85.6761726,
          42.9675857
        ],
        [
          -85.676106,
          42.9675781
        ],
        [
          -85.6760499,
          42.9675741
        ],
        [
          -85.6759947,
          42.9675723
        ],
        [
          -85.6743541,
          42.9676009
        ]
      ]
    ]
  },
  "properties": {
    "theme": "base",
    "type": "infrastructure",
    "subtype": "bridge",
    "class": "bridge",
    "names": {
      "primary": "Gillett Bridge",
      "rules": [
        {
          "variant": "alternate",
          "value": "Interurban Bridge"
        }
      ]
    },
    "sources": [
      {
        "property": "",
        "record_id": "w556368546@3",
        "dataset": "OpenStreetMap"
      }
    ],
    "version": 0
  }
}
```


### Example 2
#### json
```json
{
  "id": "08b4035ac1518fff0001a9e45d5e1c9d",
  "type": "Feature",
  "geometry": {
    "type": "Point",
    "coordinates": [
      111.5341723,
      25.1110193
    ]
  },
  "properties": {
    "theme": "base",
    "type": "infrastructure",
    "subtype": "power",
    "class": "generator",
    "height": 160.0,
    "names": {
      "primary": "DEW-G5000-195"
    },
    "sources": [
      {
        "property": "",
        "record_id": "n10707323715@5",
        "dataset": "OpenStreetMap"
      }
    ],
    "version": 0
  }
}
```

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
title: Infrastructure Schema
description: Various features from OpenStreetMap such as bridges, airport runways,
  aerialways, or communication towers and lines.
type: object
properties:
  id:
    $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyDefinitions/id
  geometry:
    unevaluatedProperties: false
    oneOf:
    - $ref: https://geojson.org/schema/Point.json
    - $ref: https://geojson.org/schema/LineString.json
    - $ref: https://geojson.org/schema/Polygon.json
    - $ref: https://geojson.org/schema/MultiPolygon.json
  properties:
    unevaluatedProperties: false
    allOf:
    - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/overtureFeaturePropertiesContainer
    - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/namesContainer
    - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/definitions/schema.yaml#/$defs/propertyContainers/levelContainer
    - $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/base/definitions/schema.yaml#/$defs/propertyContainers/osmPropertiesContainer
    required:
    - theme
    - type
    - subtype
    - class
    properties:
      theme:
        const: base
      type:
        const: infrastructure
      subtype:
        description: Further description of the type of infrastructure.
        type: string
        enum:
        - aerialway
        - airport
        - barrier
        - bridge
        - communication
        - emergency
        - manhole
        - pedestrian
        - pier
        - power
        - quay
        - recreation
        - tower
        - transit
        - transportation
        - utility
        - waste_management
        - water
      class:
        description: Further classification of the infrastructure type
        type: string
        enum:
        - aerialway_station
        - airport
        - airport_gate
        - airstrip
        - apron
        - aqueduct
        - artwork
        - atm
        - barrier
        - bell_tower
        - bench
        - bicycle_parking
        - bicycle_rental
        - block
        - boardwalk
        - bollard
        - border_control
        - breakwater
        - bridge
        - bridge_support
        - bump_gate
        - bus_route
        - bus_station
        - bus_stop
        - bus_trap
        - cable
        - cable_barrier
        - cable_car
        - cable_distribution
        - camp_site
        - cantilever
        - catenary_mast
        - cattle_grid
        - chain
        - chair_lift
        - charging_station
        - city_wall
        - communication_line
        - communication_pole
        - communication_tower
        - connection
        - cooling
        - covered
        - crossing
        - cutline
        - cycle_barrier
        - dam
        - defensive
        - ditch
        - diving
        - drag_lift
        - drain
        - drinking_water
        - entrance
        - fence
        - ferry_terminal
        - fire_hydrant
        - fountain
        - full-height_turnstile
        - gasometer
        - gate
        - generator
        - give_way
        - gondola
        - goods
        - guard_rail
        - hampshire_gate
        - handrail
        - hedge
        - height_restrictor
        - heliostat
        - helipad
        - heliport
        - hose
        - information
        - insulator
        - international_airport
        - j-bar
        - jersey_barrier
        - kerb
        - kissing_gate
        - launchpad
        - lift_gate
        - lighting
        - lightning_protection
        - magic_carpet
        - manhole
        - milestone
        - military_airport
        - minaret
        - minor_line
        - mixed_lift
        - mobile_phone_tower
        - monitoring
        - motorcycle_parking
        - motorway_junction
        - movable
        - municipal_airport
        - observation
        - parking
        - parking_entrance
        - parking_space
        - pedestrian_crossing
        - picnic_table
        - pier
        - pipeline
        - plant
        - planter
        - platform
        - platter
        - portal
        - post_box
        - power_line
        - power_pole
        - power_tower
        - private_airport
        - pylon
        - quay
        - radar
        - railway_halt
        - railway_station
        - recycling
        - regional_airport
        - reservoir_covered
        - retaining_wall
        - roller_coaster
        - rope_tow
        - runway
        - sally_port
        - seaplane_airport
        - sewer
        - silo
        - siren
        - stile
        - stop
        - stop_position
        - stopway
        - storage_tank
        - street_cabinet
        - street_lamp
        - substation
        - subway_station
        - swing_gate
        - switch
        - t-bar
        - taxilane
        - taxiway
        - terminal
        - toilets
        - toll_booth
        - traffic_signals
        - transformer
        - trestle
        - utility_pole
        - vending_machine
        - viaduct
        - viewpoint
        - wall
        - waste_basket
        - waste_disposal
        - watchtower
        - water_tower
        - weir
        - zip_line
      height:
        $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/base/definitions/schema.yaml#/$defs/propertyDefinitions/height
      surface:
        $ref: https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/base/definitions/schema.yaml#/$defs/propertyDefinitions/surface

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/base/infrastructure/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/base/infrastructure/schema.yaml)


# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-overturemaps](https://github.com/ogcincubator/bblocks-overturemaps)
* Path: `_sources/schemas/base/infrastructure`

