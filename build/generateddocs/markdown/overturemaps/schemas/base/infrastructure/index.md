
# Infrastructure Schema (Schema)

`ogc.overturemaps.schemas.base.infrastructure` *v0.1*

Various features from OpenStreetMap such as bridges, airport runways, aerialways, or communication towers and lines.

[*Status*](http://www.opengis.net/def/status): Under development

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
title: Infrastructure Schema
description: Various features from OpenStreetMap such as bridges, airport runways,
  aerialways, or communication towers and lines.
type: object
properties:
  id:
    $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/defs.yaml#/$defs/propertyDefinitions/id
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
    - $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/defs.yaml#/$defs/propertyContainers/overtureFeaturePropertiesContainer
    - $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/defs.yaml#/$defs/propertyContainers/namesContainer
    - $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/defs.yaml#/$defs/propertyContainers/levelContainer
    - $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/base/defs.yaml#/$defs/propertyContainers/osmPropertiesContainer
    required:
    - subtype
    - class
    properties:
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
        $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/base/defs.yaml#/$defs/propertyDefinitions/height
      surface:
        $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/base/defs.yaml#/$defs/propertyDefinitions/surface

```

Links to the schema:

* YAML version: [schema.yaml](https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/base/infrastructure/schema.json)
* JSON version: [schema.json](https://raw.githubusercontent.com/ogcincubator/bblocks-overturemaps/undefined/build/annotated/overturemaps/schemas/base/infrastructure/schema.yaml)


# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-overturemaps](https://github.com/ogcincubator/bblocks-overturemaps)
* Path: `_sources/schemas/base/infrastructure`

