# Yūgen — open sample of verified places (v0.1)

94 places from the Yūgen atlas where a visitor can directly observe an unusual natural, geological, ecological, archaeological, spatial or historical phenomenon. 37 countries.

This is the first public sample. The full verified layer (≈2,200 places today) will follow, then the rest of the atlas as it is checked.

## Files

- `yugen_places_sample.csv` — one row per place
- `yugen_places_sample.json` — the same data as JSON

## Fields

| Field | Meaning |
|---|---|
| `id` | Stable Yūgen identifier (country code + number) |
| `name` | Place name in English |
| `country_code` | ISO 3166-1 alpha-2 |
| `latitude`, `longitude` | WGS84, decimal degrees |
| `phenomenon_type` | What kind of observation the place offers (see below) |
| `category` | Broad place category |
| `observe` | One line: what you can see there with your own eyes |
| `coordinate_check` | How the coordinate was checked: `osm_verified`, `wikipedia_verified`, `wikidata_verified`, `manual_verified` |
| `coordinate_source` | OpenStreetMap link to the checked position |

`phenomenon_type` values: `phenomenon_point`, `environmental_field`, `movement_experience`, `viewpoint_alignment`, `threshold`, `temporal_window`, `residue`, `panorama`, `street_pressure`, `crowd_cycle`, `terrain`, `concealment`, `landmark`.

## How places are checked

1. A candidate place must answer one question: what can a visitor directly observe here?
2. The coordinate is matched against OpenStreetMap, Wikipedia or Wikidata, or checked by hand.
3. Places whose position or phenomenon cannot be confirmed are left out of this dataset, not guessed.

## Licence

The database is released under the [Open Database License (ODbL) 1.0](https://opendatacommons.org/licenses/odbl/1-0/). Coordinates checked against OpenStreetMap: © OpenStreetMap contributors.

## Contact

Anastasia — anmatlaeva@gmail.com
