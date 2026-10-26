# MadNav map packs

Offline map packs for [MadNav](https://github.com/TheQuiltProject/madnav),
the open-source GPS bike computer and its iOS app: Europe's countries and
territories as MNT1 tile packs (zoom 14 vector tiles: roads and paths by
class, cycleways, railways, water, green areas, buildings).

They are published here as [releases](../../releases), built monthly from
[Geofabrik](https://download.geofabrik.de/)'s OpenStreetMap extracts by a
workflow in MadNav's repository (`tools/mapgen`). Each release has, per
region:

| File | What |
|---|---|
| `<region>.mnt` | the map without buildings |
| `<region>-buildings.mnt` | its buildings (about a third of the size; drawn when zoomed in) |
| `manifest.json` | every pack with its size, SHA-256, bounding box, the data's date and download URL |

The latest manifest is always at
<https://github.com/TheQuiltProject/madnav-maps/releases/latest/download/manifest.json>,
which is where the app looks. The format is described in MadNav's
`firmware/components/madnav_core/include/mnt.h`.

## License

The map data is © [OpenStreetMap contributors](https://www.openstreetmap.org/copyright)
and the packs, being derived from it, are available under the
[Open Data Commons Open Database License (ODbL) 1.0](https://opendatacommons.org/licenses/odbl/1-0/).
Show "© OpenStreetMap contributors" wherever you display them.
