# WanderPing catalog

The catalog of cities, attractions and trips used by the WanderPing app (Android and iOS), published as required by the
[Open Database License (ODbL) 1.0](https://opendatacommons.org/licenses/odbl/1-0/).

Download: the `catalog-<version>` releases of this repository, one `.zip` per app version that changes the catalog
(first: [`catalog-0.6.20`](https://github.com/sebastianmazilu91-cpu/wanderping-maps/releases/tag/catalog-0.6.20)).

## Contents

| File | What it holds |
|------|---------------|
| `cities.json` | The cities: name, country, region (with translations), position, map zoom, offline map file |
| `attractions/<city>.json` | The attractions of one city: name, category, position, visit time, short and long description, hours, tickets, source |
| `attractions/<city>.<lang>.json` | Translations of the texts above (`en`, `de`, `fr`, `es`, `it`), by attraction id |
| `places.json` | Trips outside the walkable cities: name, category, area, country, region, position, texts, source |

All files are UTF-8 JSON. Positions are WGS 84 latitude and longitude.

## License

The catalog is a database derived from [OpenStreetMap](https://www.openstreetmap.org) and is made available under the
**Open Database License (ODbL) 1.0**: © [OpenStreetMap contributors](https://www.openstreetmap.org/copyright) and
WanderPing. You may copy, adapt and share it, provided you attribute it, keep any adapted database under the ODbL and
offer it in the same way (see the license).

The individual contents keep the license of their source, named in each entry's `source` field:

- **OpenStreetMap** (`openstreetmap.org` links, and positions checked against OpenStreetMap): ODbL 1.0.
- **Wikipedia and Wikivoyage** (`wikipedia.org`, `wikivoyage.org` links): the descriptions are excerpts (the first
  sentences) of the linked article, under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). Attribute
  them to the linked article and its authors.
- **Wikidata** (short descriptions): [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/).
- **Entries without a source** (a few attractions in Iași): texts written by WanderPing.
