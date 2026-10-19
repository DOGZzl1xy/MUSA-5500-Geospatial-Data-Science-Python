# Week 8A classroom snapshot

Source: OpenStreetMap contributors, https://www.openstreetmap.org/copyright (ODbL).
Prepared from the existing lab OSMnx response cache, dated October 16, 2025, using OSMnx 2.0.6. These are historical classroom data, not a current inventory.

- drive.graphml.gz / walk.graphml.gz: graph_from_address("Center City, Philadelphia, PA", dist=2000, network_type="drive" / "walk").
- classroom.gpkg, layer philadelphia: geocode_to_gdf("Philadelphia, PA").
- classroom.gpkg, layer amenities: features_from_place("Philadelphia, PA", tags={"amenity": True}), restricted to the walking graph bounding box, retaining feature IDs, amenity, name, and geometry.

The notebook reads these snapshots by default. Set REFRESH_FROM_OSM=True to query OSM services in memory; the supplied snapshots are not overwritten.
