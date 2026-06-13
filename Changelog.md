# Changelog

All notable changes to this dataset are documented here.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/). See the
[Versioning](README.md#versioning) section of the README for what MAJOR / MINOR /
PATCH mean for this dataset.

## [1.0.0] - 2026-06-13

First tagged release of the Open Climbing Center Dataset.

### Summary

- **105 climbing centers** across **12 countries** (Austria, Belgium, Czech
  Republic, Denmark, Finland, France, Germany, Ireland, Italy, Netherlands,
  Spain, Sweden), all in Europe.
- **85** records have an Instagram handle; **103** have a `last_verified` date.

### Added

- `instagram` column — official Instagram handle for each center (per-location
  where a center runs its own account, otherwise the shared chain handle).
  Appended after `homepage`.
- `last_verified` column — date each record was last checked against a primary
  source. Appended as the final column.
- Major European bouldering chains, one row per location, including Boulders,
  Beta Boulders, Bison Boulders (Denmark); Boulderwelt, Stuntwerk, einstein,
  Kletterfabrik (Germany); boulderbar (Austria); Arkose, Vertical'Art, Climb Up,
  Block'Out (France); Monk, Beest, Sterk, Mountain Network (Netherlands); Bleau,
  Klimzaal Blok (Belgium); Sharma Climbing, Sputnik Climbing, Indoorwall (Spain);
  Rockspot, B-Side (Italy); Klätterverket (Sweden); Boulderkeskus (Finland);
  SmíchOFF (Czech Republic); Gravity (Ireland).
- Independent Danish centers verified from their own websites: Aalborg
  Klatreklub, Nørrebro Klatreklub, OBK – Odense Boulderklub.
- `README.md` documenting the full 21-column schema, data guidelines,
  `grading_type` values, and the versioning policy.
- This `CHANGELOG.md`.

### Verified

- All 11 Boulders locations confirmed (existence, address, and per-location
  Instagram handles) against the official `boulders.dk` site and Boulders
  Linktree.
- All non-Denmark chain rows researched and dated `2026-06-13`.

### Notes

- Coverage is currently weighted toward major multi-location chains in Western
  and Northern Europe; it is **not** an exhaustive list of every center.

[1.0.0]: https://github.com/aNorrah/OpenClimbingDatasets/releases/tag/v1.0.0
