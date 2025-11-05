
# land_use (Schema)

`ogc.overturemaps.schemas.base.land_use` *v0.1*

Land use features from OpenStreetMap

[*Status*](http://www.opengis.net/def/status): Under development

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
title: land_use
description: Land use features from OpenStreetMap
type: object
properties:
  id:
    $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/defs.yaml#/$defs/propertyDefinitions/id
  geometry:
    description: Classifications of the human use of a section of land. Translates
      `landuse` from OpenStreetMap tag from OpenStreetMap.
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
        description: Broad type of land
        type: string
        enum:
        - agriculture
        - aquaculture
        - campground
        - cemetery
        - construction
        - developed
        - education
        - entertainment
        - golf
        - grass
        - horticulture
        - landfill
        - managed
        - medical
        - military
        - park
        - pedestrian
        - protected
        - recreation
        - religious
        - residential
        - resource_extraction
        - transportation
        - winter_sports
      class:
        description: Further classification of the land use
        type: string
        enum:
        - aboriginal_land
        - airfield
        - allotments
        - animal_keeping
        - aquaculture
        - barracks
        - base
        - beach_resort
        - brownfield
        - bunker
        - camp_site
        - cemetery
        - clinic
        - college
        - commercial
        - connection
        - construction
        - danger_area
        - doctors
        - dog_park
        - downhill
        - driving_range
        - driving_school
        - education
        - environmental
        - fairway
        - farmland
        - farmyard
        - fatbike
        - flowerbed
        - forest
        - garages
        - garden
        - golf_course
        - grass
        - grave_yard
        - green
        - greenfield
        - greenhouse_horticulture
        - highway
        - hike
        - hospital
        - ice_skate
        - industrial
        - institutional
        - kindergarten
        - landfill
        - lateral_water_hazard
        - logging
        - marina
        - meadow
        - military
        - military_hospital
        - military_school
        - music_school
        - national_park
        - natural_monument
        - nature_reserve
        - naval_base
        - nordic
        - nuclear_explosion_site
        - obstacle_course
        - orchard
        - park
        - peat_cutting
        - pedestrian
        - pitch
        - plant_nursery
        - playground
        - plaza
        - protected
        - protected_landscape_seascape
        - quarry
        - railway
        - range
        - recreation_ground
        - religious
        - residential
        - resort
        - retail
        - rough
        - salt_pond
        - school
        - schoolyard
        - ski_jump
        - skitour
        - sled
        - sleigh
        - snow_park
        - species_management_area
        - stadium
        - state_park
        - static_caravan
        - strict_nature_reserve
        - tee
        - theme_park
        - track
        - traffic_island
        - training_area
        - trench
        - university
        - village_green
        - vineyard
        - water_hazard
        - water_park
        - wilderness_area
        - winter_sports
        - works
        - zoo
      elevation:
        $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/base/defs.yaml#/$defs/propertyDefinitions/elevation
      surface:
        $ref: https://github.com/OvertureMaps/schema/raw/refs/heads/dev/schema/base/defs.yaml#/$defs/propertyDefinitions/surface

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/base/land_use/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-overturemaps/build/annotated/overturemaps/schemas/base/land_use/schema.yaml)


# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-overturemaps](https://github.com/ogcincubator/bblocks-overturemaps)
* Path: `_sources/schemas/base/land_use`

