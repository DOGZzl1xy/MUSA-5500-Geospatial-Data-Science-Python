# Week 8A classroom data

The refined notebook retains the original query demonstrations. The lab cache contains historical OpenStreetMap responses from October 2025. Uncached queries may retrieve newer data.

Files used by the current notebook:

- planning-districts.geojson: City of Philadelphia planning districts, retrieved for the polygon example from https://opendata.arcgis.com/datasets/0960ea0f38f44146bb562f2b212075aa_0.geojson.
- tourism.gpkg (layer tourism): Philadelphia tourism features retrieved from OpenStreetMap using OSMnx 2.0.6; source response timestamp 2026-09-25T01:05:47Z. Fields preserve element type, OSM ID, name, tourism tag, and geometry. The original live query remains in the notebook as a fallback.

Previously prepared supplementary snapshots retained for reference:

- drive.graphml.gz and walk.graphml.gz: networks from graph_from_address("Center City, Philadelphia, PA", dist=2000, network_type="drive" / "walk"), using the October 2025 cache.
- classroom.gpkg: the Philadelphia boundary and amenities within the walking network bounding box, also prepared from the October 2025 cache.

OpenStreetMap data: © OpenStreetMap contributors, ODbL, https://www.openstreetmap.org/copyright. Historical and refreshed datasets have different observation dates; this is classroom demonstration data, not a current unified inventory.
