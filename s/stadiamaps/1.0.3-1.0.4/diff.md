# Comparing `tmp/stadiamaps-1.0.3.tar.gz` & `tmp/stadiamaps-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stadiamaps-1.0.3.tar", last modified: Wed Jun 14 18:15:46 2023, max compression
+gzip compressed data, was "stadiamaps-1.0.4.tar", last modified: Thu Jun 15 16:36:01 2023, max compression
```

## Comparing `stadiamaps-1.0.3.tar` & `stadiamaps-1.0.4.tar`

### file list

```diff
@@ -1,255 +1,255 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:15:46.029869 stadiamaps-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-14 18:15:46.029869 stadiamaps-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 18:15:46.029869 stadiamaps-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:15:46.001870 stadiamaps-1.0.3/stadiamaps/
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:15:46.005869 stadiamaps-1.0.3/stadiamaps/api/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    97488 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/api/geocoding_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/api/geospatial_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    50673 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/api/routing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:15:46.017869 stadiamaps-1.0.3/stadiamaps/models/
--rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/admin_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/administrative.py
--rw-r--r--   0 runner    (1001) docker     (123)    10457 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/auto_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/auto_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/base_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/base_trace_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/bicycle_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/bicycle_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/bike_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/costing_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/directions_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/distance_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/edge_sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/edge_use.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/end_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/geo_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/geo_json_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/geo_json_geometry_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/geo_json_line_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/geo_json_line_string_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/geo_json_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/geo_json_point_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/geo_json_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/geo_json_polygon_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/geocoding_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/height_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/height_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/highway_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/intersecting_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/isochrone_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/isochrone_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/isochrone_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/isochrone_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/isochrone_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/locate_detailed_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/locate_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/locate_edge_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/locate_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/locate_node_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/locate_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/maneuver_sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/maneuver_sign_element.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/map_match_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/map_match_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/map_match_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/map_match_route_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/map_match_route_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/map_match_trace_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/map_match_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/map_match_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/matched_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/matrix_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/matrix_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/matrix_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/matrix_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11494 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/motor_scooter_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/motor_scooter_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/motorcycle_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/motorcycle_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/nearest_roads_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/node_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/node_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/optimized_route_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/pedestrian_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/pelias_geo_json_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/pelias_geo_json_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/pelias_geo_json_properties_addendum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/pelias_geo_json_properties_addendum_osm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/pelias_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/pelias_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/pelias_response_geocoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/pelias_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/restrictions.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/road_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/route_leg.py
--rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/route_maneuver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/route_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/route_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/route_response_trip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/route_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/routing_response_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/routing_response_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/routing_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/routing_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/routing_waypoint_all_of_search_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/simple_routing_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/simple_routing_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/speeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/trace_attribute_filter_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/trace_attribute_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/trace_attributes_base_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/trace_attributes_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/trace_attributes_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/trace_attributes_request_all_of_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/trace_attributes_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/trace_attributes_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    13690 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/trace_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/travel_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/traversability.py
--rw-r--r--   0 runner    (1001) docker     (123)    11331 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/truck_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/truck_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/tz_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/valhalla_languages.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/valhalla_long_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/models/warning.py
--rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/stadiamaps/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:15:46.005869 stadiamaps-1.0.3/stadiamaps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-14 18:15:45.000000 stadiamaps-1.0.3/stadiamaps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-06-14 18:15:46.000000 stadiamaps-1.0.3/stadiamaps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 18:15:45.000000 stadiamaps-1.0.3/stadiamaps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-14 18:15:45.000000 stadiamaps-1.0.3/stadiamaps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 18:15:45.000000 stadiamaps-1.0.3/stadiamaps.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:15:46.029869 stadiamaps-1.0.3/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:15:46.029869 stadiamaps-1.0.3/test/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/integration/test_eu_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/integration/test_gecoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/integration/test_geospatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/integration/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_admin_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_administrative.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_auto_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_auto_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_base_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_base_trace_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_bicycle_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_bicycle_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_bike_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_directions_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_distance_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_edge_sign.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_edge_use.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_end_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_geo_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_geo_json_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_geo_json_geometry_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_geo_json_line_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_geo_json_line_string_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_geo_json_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_geo_json_point_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_geo_json_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_geo_json_polygon_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_geocoding_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_geocoding_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_geospatial_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_height_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_height_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_highway_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_intersecting_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_isochrone_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_isochrone_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_isochrone_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_isochrone_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_isochrone_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_locate_detailed_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_locate_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_locate_edge_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_locate_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_locate_node_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_locate_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_maneuver_sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_maneuver_sign_element.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_map_match_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_map_match_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_map_match_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_map_match_route_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_map_match_route_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_map_match_trace_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_map_match_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_map_match_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_matched_point.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_matrix_costing_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_matrix_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_matrix_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_matrix_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_motor_scooter_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_motor_scooter_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_motorcycle_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_motorcycle_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_nearest_roads_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_node_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_node_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_optimized_route_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_pedestrian_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_pelias_geo_json_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_pelias_geo_json_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_pelias_geo_json_properties_addendum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_pelias_geo_json_properties_addendum_osm.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_pelias_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_pelias_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_pelias_response_geocoding.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_pelias_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_restrictions.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_road_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_route_leg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_route_maneuver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_route_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_route_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_route_response_trip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_route_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_routing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_routing_response_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_routing_response_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_routing_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_routing_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_routing_waypoint_all_of_search_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_simple_routing_waypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_simple_routing_waypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_speeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_trace_attribute_filter_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_trace_attribute_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_trace_attributes_base_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_trace_attributes_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_trace_attributes_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_trace_attributes_request_all_of_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_trace_attributes_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_trace_attributes_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_trace_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_travel_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_traversability.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_truck_costing_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_truck_costing_options_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_tz_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_valhalla_languages.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_valhalla_long_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-14 18:15:32.000000 stadiamaps-1.0.3/test/test_warning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:36:01.081104 stadiamaps-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-15 16:36:01.081104 stadiamaps-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 16:36:01.081104 stadiamaps-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:36:01.049103 stadiamaps-1.0.4/stadiamaps/
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:36:01.049103 stadiamaps-1.0.4/stadiamaps/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97488 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/api/geocoding_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/api/geospatial_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50673 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/api/routing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:36:01.065104 stadiamaps-1.0.4/stadiamaps/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/admin_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/administrative.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10457 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/auto_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/auto_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/base_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/base_trace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/bicycle_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/bicycle_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/bike_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/directions_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/distance_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/edge_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/edge_use.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/end_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/geo_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/geo_json_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/geo_json_geometry_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/geo_json_line_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/geo_json_line_string_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/geo_json_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/geo_json_point_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/geo_json_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/geo_json_polygon_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/geocoding_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/height_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/height_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/highway_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/intersecting_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/isochrone_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/isochrone_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/isochrone_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/isochrone_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/isochrone_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/locate_detailed_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/locate_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/locate_edge_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/locate_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/locate_node_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/locate_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/maneuver_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/maneuver_sign_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/map_match_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/map_match_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/map_match_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/map_match_route_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/map_match_route_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/map_match_trace_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/map_match_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/map_match_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/matched_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/matrix_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/matrix_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/matrix_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/matrix_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11494 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/motor_scooter_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/motor_scooter_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/motorcycle_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/motorcycle_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/nearest_roads_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/node_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/node_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/optimized_route_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/pedestrian_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/pelias_geo_json_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/pelias_geo_json_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/pelias_geo_json_properties_addendum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/pelias_geo_json_properties_addendum_osm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/pelias_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/pelias_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/pelias_response_geocoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/pelias_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/road_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/route_leg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/route_maneuver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/route_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/route_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/route_response_trip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/route_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/routing_response_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/routing_response_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/routing_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/routing_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/routing_waypoint_all_of_search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/simple_routing_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/simple_routing_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/speeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/trace_attribute_filter_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/trace_attribute_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/trace_attributes_base_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/trace_attributes_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/trace_attributes_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/trace_attributes_request_all_of_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/trace_attributes_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/trace_attributes_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13690 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/trace_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/travel_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/traversability.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11331 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/truck_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/truck_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/tz_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/valhalla_languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/valhalla_long_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/models/warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/stadiamaps/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:36:01.049103 stadiamaps-1.0.4/stadiamaps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-15 16:36:01.000000 stadiamaps-1.0.4/stadiamaps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-06-15 16:36:01.000000 stadiamaps-1.0.4/stadiamaps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:36:01.000000 stadiamaps-1.0.4/stadiamaps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-15 16:36:01.000000 stadiamaps-1.0.4/stadiamaps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 16:36:01.000000 stadiamaps-1.0.4/stadiamaps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:36:01.077104 stadiamaps-1.0.4/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:36:01.077104 stadiamaps-1.0.4/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/integration/test_eu_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/integration/test_gecoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/integration/test_geospatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/integration/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_admin_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_administrative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_auto_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_auto_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_base_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_base_trace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_bicycle_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_bicycle_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_bike_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_directions_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_distance_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_edge_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_edge_use.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_end_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_geo_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_geo_json_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_geo_json_geometry_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_geo_json_line_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_geo_json_line_string_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_geo_json_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_geo_json_point_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_geo_json_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_geo_json_polygon_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_geocoding_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_geocoding_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_geospatial_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_height_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_height_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_highway_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_intersecting_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_isochrone_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_isochrone_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_isochrone_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_isochrone_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_isochrone_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_locate_detailed_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_locate_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_locate_edge_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_locate_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_locate_node_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_locate_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_maneuver_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_maneuver_sign_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_map_match_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_map_match_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_map_match_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_map_match_route_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_map_match_route_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_map_match_trace_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_map_match_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_map_match_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_matched_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_matrix_costing_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_matrix_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_matrix_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_matrix_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_motor_scooter_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_motor_scooter_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_motorcycle_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_motorcycle_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_nearest_roads_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_node_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_node_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_optimized_route_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_pedestrian_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_pelias_geo_json_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_pelias_geo_json_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_pelias_geo_json_properties_addendum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_pelias_geo_json_properties_addendum_osm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_pelias_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_pelias_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_pelias_response_geocoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_pelias_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_road_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_route_leg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_route_maneuver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_route_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_route_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_route_response_trip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_route_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_routing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_routing_response_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_routing_response_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_routing_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_routing_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_routing_waypoint_all_of_search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_simple_routing_waypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_simple_routing_waypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_speeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_trace_attribute_filter_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_trace_attribute_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_trace_attributes_base_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_trace_attributes_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_trace_attributes_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_trace_attributes_request_all_of_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_trace_attributes_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_trace_attributes_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_trace_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_travel_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_traversability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_truck_costing_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_truck_costing_options_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_tz_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_valhalla_languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_valhalla_long_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-15 16:35:51.000000 stadiamaps-1.0.4/test/test_warning.py
```

### Comparing `stadiamaps-1.0.3/LICENSE.txt` & `stadiamaps-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/PKG-INFO` & `stadiamaps-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stadiamaps
-Version: 1.0.3
+Version: 1.0.4
 Summary: Stadia Maps Geospatial APIs
 Home-page: https://github.com/stadiamaps/stadiamaps-api-py
 Author: Stadia Maps Support
 Author-email: support@stadiamaps.com
 Keywords: OpenAPI,OpenAPI-Generator,Stadia Maps Geospatial APIs
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `stadiamaps-1.0.3/README.md` & `stadiamaps-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/pyproject.toml` & `stadiamaps-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stadiamaps"
-version = "1.0.3"
+version = "1.0.4"
 description = "Stadia Maps Geospatial APIs"
 authors = ["Stadia Maps Support <support@stadiamaps.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/stadiamaps/stadiamaps-api-py"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Stadia Maps Geospatial APIs"]
```

### Comparing `stadiamaps-1.0.3/setup.py` & `stadiamaps-1.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -18,15 +18,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "stadiamaps"
-VERSION = "1.0.3"
+VERSION = "1.0.4"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3",
     "python-dateutil",
     "pydantic >= 1.10.5, < 2",
     "aenum"
 ]
```

### Comparing `stadiamaps-1.0.3/stadiamaps/__init__.py` & `stadiamaps-1.0.4/stadiamaps/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 
 # import apis into sdk package
 from stadiamaps.api.geocoding_api import GeocodingApi
 from stadiamaps.api.geospatial_api import GeospatialApi
 from stadiamaps.api.routing_api import RoutingApi
 
 # import ApiClient
```

### Comparing `stadiamaps-1.0.3/stadiamaps/api/geocoding_api.py` & `stadiamaps-1.0.4/stadiamaps/api/geocoding_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/api/geospatial_api.py` & `stadiamaps-1.0.4/stadiamaps/api/geospatial_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/api/routing_api.py` & `stadiamaps-1.0.4/stadiamaps/api/routing_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/api_client.py` & `stadiamaps-1.0.4/stadiamaps/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.3/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.4/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `stadiamaps-1.0.3/stadiamaps/api_response.py` & `stadiamaps-1.0.4/stadiamaps/api_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/stadiamaps/configuration.py` & `stadiamaps-1.0.4/stadiamaps/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -393,16 +393,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 5.0.2\n"\
-               "SDK Package Version: 1.0.3".\
+               "Version of the API: 5.0.3\n"\
+               "SDK Package Version: 1.0.4".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/exceptions.py` & `stadiamaps-1.0.4/stadiamaps/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/__init__.py` & `stadiamaps-1.0.4/stadiamaps/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/access.py` & `stadiamaps-1.0.4/stadiamaps/models/access.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/admin_region.py` & `stadiamaps-1.0.4/stadiamaps/models/admin_region.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/administrative.py` & `stadiamaps-1.0.4/stadiamaps/models/administrative.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/auto_costing_options.py` & `stadiamaps-1.0.4/stadiamaps/models/auto_costing_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/auto_costing_options_all_of.py` & `stadiamaps-1.0.4/stadiamaps/models/auto_costing_options_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/base_costing_options.py` & `stadiamaps-1.0.4/stadiamaps/models/base_costing_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/base_trace_request.py` & `stadiamaps-1.0.4/stadiamaps/models/base_trace_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/bicycle_costing_options.py` & `stadiamaps-1.0.4/stadiamaps/models/bicycle_costing_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/bicycle_costing_options_all_of.py` & `stadiamaps-1.0.4/stadiamaps/models/bicycle_costing_options_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/bike_network.py` & `stadiamaps-1.0.4/stadiamaps/models/bike_network.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/contour.py` & `stadiamaps-1.0.4/stadiamaps/models/contour.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/coordinate.py` & `stadiamaps-1.0.4/stadiamaps/models/coordinate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/costing_model.py` & `stadiamaps-1.0.4/stadiamaps/models/costing_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/costing_options.py` & `stadiamaps-1.0.4/stadiamaps/models/costing_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/directions_options.py` & `stadiamaps-1.0.4/stadiamaps/models/directions_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/distance_unit.py` & `stadiamaps-1.0.4/stadiamaps/models/distance_unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/edge_sign.py` & `stadiamaps-1.0.4/stadiamaps/models/edge_sign.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/edge_use.py` & `stadiamaps-1.0.4/stadiamaps/models/edge_use.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/end_node.py` & `stadiamaps-1.0.4/stadiamaps/models/end_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/geo_attributes.py` & `stadiamaps-1.0.4/stadiamaps/models/geo_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/geo_json_geometry.py` & `stadiamaps-1.0.4/stadiamaps/models/geo_json_geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/geo_json_geometry_base.py` & `stadiamaps-1.0.4/stadiamaps/models/geo_json_geometry_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/geo_json_line_string.py` & `stadiamaps-1.0.4/stadiamaps/models/geo_json_line_string.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/geo_json_line_string_all_of.py` & `stadiamaps-1.0.4/stadiamaps/models/geo_json_line_string_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/geo_json_point.py` & `stadiamaps-1.0.4/stadiamaps/models/geo_json_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/geo_json_point_all_of.py` & `stadiamaps-1.0.4/stadiamaps/models/geo_json_point_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/geo_json_polygon.py` & `stadiamaps-1.0.4/stadiamaps/models/geo_json_polygon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/geo_json_polygon_all_of.py` & `stadiamaps-1.0.4/stadiamaps/models/geo_json_polygon_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/geocoding_object.py` & `stadiamaps-1.0.4/stadiamaps/models/geocoding_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/height_request.py` & `stadiamaps-1.0.4/stadiamaps/models/height_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/height_response.py` & `stadiamaps-1.0.4/stadiamaps/models/height_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/highway_classification.py` & `stadiamaps-1.0.4/stadiamaps/models/highway_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/intersecting_edge.py` & `stadiamaps-1.0.4/stadiamaps/models/intersecting_edge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/isochrone_costing_model.py` & `stadiamaps-1.0.4/stadiamaps/models/isochrone_costing_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/isochrone_feature.py` & `stadiamaps-1.0.4/stadiamaps/models/isochrone_feature.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/isochrone_properties.py` & `stadiamaps-1.0.4/stadiamaps/models/isochrone_properties.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/isochrone_request.py` & `stadiamaps-1.0.4/stadiamaps/models/isochrone_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/isochrone_response.py` & `stadiamaps-1.0.4/stadiamaps/models/isochrone_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/locate_detailed_edge.py` & `stadiamaps-1.0.4/stadiamaps/models/locate_detailed_edge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/locate_edge.py` & `stadiamaps-1.0.4/stadiamaps/models/locate_edge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/locate_edge_info.py` & `stadiamaps-1.0.4/stadiamaps/models/locate_edge_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/locate_node.py` & `stadiamaps-1.0.4/stadiamaps/models/locate_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/locate_node_all_of.py` & `stadiamaps-1.0.4/stadiamaps/models/locate_node_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/locate_object.py` & `stadiamaps-1.0.4/stadiamaps/models/locate_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/maneuver_sign.py` & `stadiamaps-1.0.4/stadiamaps/models/maneuver_sign.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/maneuver_sign_element.py` & `stadiamaps-1.0.4/stadiamaps/models/maneuver_sign_element.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/map_match_costing_model.py` & `stadiamaps-1.0.4/stadiamaps/models/map_match_costing_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/map_match_request.py` & `stadiamaps-1.0.4/stadiamaps/models/map_match_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/map_match_request_all_of.py` & `stadiamaps-1.0.4/stadiamaps/models/map_match_request_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/map_match_route_response.py` & `stadiamaps-1.0.4/stadiamaps/models/map_match_route_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/map_match_route_response_all_of.py` & `stadiamaps-1.0.4/stadiamaps/models/map_match_route_response_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/map_match_trace_options.py` & `stadiamaps-1.0.4/stadiamaps/models/map_match_trace_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/map_match_waypoint.py` & `stadiamaps-1.0.4/stadiamaps/models/map_match_waypoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/map_match_waypoint_all_of.py` & `stadiamaps-1.0.4/stadiamaps/models/map_match_waypoint_all_of.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/matched_point.py` & `stadiamaps-1.0.4/stadiamaps/models/matched_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/matrix_costing_model.py` & `stadiamaps-1.0.4/stadiamaps/models/matrix_costing_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/matrix_distance.py` & `stadiamaps-1.0.4/stadiamaps/models/matrix_distance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/matrix_request.py` & `stadiamaps-1.0.4/stadiamaps/models/matrix_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/matrix_response.py` & `stadiamaps-1.0.4/stadiamaps/models/matrix_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/motor_scooter_costing_options.py` & `stadiamaps-1.0.4/stadiamaps/models/motor_scooter_costing_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/motor_scooter_costing_options_all_of.py` & `stadiamaps-1.0.4/stadiamaps/models/motor_scooter_costing_options_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/motorcycle_costing_options.py` & `stadiamaps-1.0.4/stadiamaps/models/motorcycle_costing_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/motorcycle_costing_options_all_of.py` & `stadiamaps-1.0.4/stadiamaps/models/motorcycle_costing_options_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/nearest_roads_request.py` & `stadiamaps-1.0.4/stadiamaps/models/nearest_roads_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/node_id.py` & `stadiamaps-1.0.4/stadiamaps/models/node_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/node_type.py` & `stadiamaps-1.0.4/stadiamaps/models/node_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/optimized_route_request.py` & `stadiamaps-1.0.4/stadiamaps/models/optimized_route_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/pedestrian_costing_options.py` & `stadiamaps-1.0.4/stadiamaps/models/pedestrian_costing_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/pelias_geo_json_feature.py` & `stadiamaps-1.0.4/stadiamaps/models/pelias_geo_json_feature.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, Field, StrictStr, validator
+from typing import List, Optional, Union
+from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr, conlist, validator
 from stadiamaps.models.geo_json_point import GeoJSONPoint
 from stadiamaps.models.pelias_geo_json_properties import PeliasGeoJSONProperties
 
 class PeliasGeoJSONFeature(BaseModel):
     """
     PeliasGeoJSONFeature
     """
     type: StrictStr = Field(...)
     geometry: GeoJSONPoint = Field(...)
     properties: Optional[PeliasGeoJSONProperties] = None
+    bbox: Optional[conlist(Union[StrictFloat, StrictInt], max_items=4, min_items=4)] = Field(None, description="An array of 4 floating point numbers representing the (W, S, E, N) extremes of the features found.")
     id: Optional[StrictStr] = None
     additional_properties: Dict[str, Any] = {}
-    __properties = ["type", "geometry", "properties", "id"]
+    __properties = ["type", "geometry", "properties", "bbox", "id"]
 
     @validator('type')
     def type_validate_enum(cls, value):
         """Validates the enum"""
         if value not in ('Feature'):
             raise ValueError("must be one of enum values ('Feature')")
         return value
@@ -89,14 +90,15 @@
         if not isinstance(obj, dict):
             return PeliasGeoJSONFeature.parse_obj(obj)
 
         _obj = PeliasGeoJSONFeature.parse_obj({
             "type": obj.get("type"),
             "geometry": GeoJSONPoint.from_dict(obj.get("geometry")) if obj.get("geometry") is not None else None,
             "properties": PeliasGeoJSONProperties.from_dict(obj.get("properties")) if obj.get("properties") is not None else None,
+            "bbox": obj.get("bbox"),
             "id": obj.get("id")
         })
         # store additional fields in additional_properties
         for _key in obj.keys():
             if _key not in cls.__properties:
                 _obj.additional_properties[_key] = obj.get(_key)
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/pelias_geo_json_properties.py` & `stadiamaps-1.0.4/stadiamaps/models/pelias_geo_json_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -43,20 +43,20 @@
     neighbourhood_gid: Optional[StrictStr] = None
     borough: Optional[StrictStr] = None
     borough_gid: Optional[StrictStr] = None
     postalcode: Optional[StrictStr] = None
     street: Optional[StrictStr] = None
     housenumber: Optional[StrictStr] = None
     locality: Optional[StrictStr] = Field(None, description="The city, village, town, etc. that the place / address is part of. Note that values may not always match postal or local conventions perfectly.")
-    lecality_gid: Optional[StrictStr] = None
+    locality_gid: Optional[StrictStr] = None
     county: Optional[StrictStr] = Field(None, description="Administrative divisions between localities and regions. Useful for disambiguating nearby results with similar names.")
     region: Optional[StrictStr] = Field(None, description="Typically the first administrative division within a country. For example, a US state or a Canadian province.")
     region_a: Optional[StrictStr] = Field(None, description="The abbreviation for the region.")
     additional_properties: Dict[str, Any] = {}
-    __properties = ["gid", "source_id", "label", "layer", "name", "accuracy", "addendum", "continent", "continent_gid", "country", "country_gid", "neighbourhood", "neighbourhood_gid", "borough", "borough_gid", "postalcode", "street", "housenumber", "locality", "lecality_gid", "county", "region", "region_a"]
+    __properties = ["gid", "source_id", "label", "layer", "name", "accuracy", "addendum", "continent", "continent_gid", "country", "country_gid", "neighbourhood", "neighbourhood_gid", "borough", "borough_gid", "postalcode", "street", "housenumber", "locality", "locality_gid", "county", "region", "region_a"]
 
     @validator('accuracy')
     def accuracy_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
@@ -124,15 +124,15 @@
             "neighbourhood_gid": obj.get("neighbourhood_gid"),
             "borough": obj.get("borough"),
             "borough_gid": obj.get("borough_gid"),
             "postalcode": obj.get("postalcode"),
             "street": obj.get("street"),
             "housenumber": obj.get("housenumber"),
             "locality": obj.get("locality"),
-            "lecality_gid": obj.get("lecality_gid"),
+            "locality_gid": obj.get("locality_gid"),
             "county": obj.get("county"),
             "region": obj.get("region"),
             "region_a": obj.get("region_a")
         })
         # store additional fields in additional_properties
         for _key in obj.keys():
             if _key not in cls.__properties:
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/pelias_geo_json_properties_addendum.py` & `stadiamaps-1.0.4/stadiamaps/models/pelias_geo_json_properties_addendum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/pelias_geo_json_properties_addendum_osm.py` & `stadiamaps-1.0.4/stadiamaps/models/pelias_geo_json_properties_addendum_osm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/pelias_layer.py` & `stadiamaps-1.0.4/stadiamaps/models/pelias_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/pelias_response.py` & `stadiamaps-1.0.4/stadiamaps/models/pelias_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/pelias_response_geocoding.py` & `stadiamaps-1.0.4/stadiamaps/models/pelias_response_geocoding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/pelias_source.py` & `stadiamaps-1.0.4/stadiamaps/models/pelias_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/restrictions.py` & `stadiamaps-1.0.4/stadiamaps/models/restrictions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/road_class.py` & `stadiamaps-1.0.4/stadiamaps/models/road_class.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/route_leg.py` & `stadiamaps-1.0.4/stadiamaps/models/route_leg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/route_maneuver.py` & `stadiamaps-1.0.4/stadiamaps/models/route_maneuver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/route_request.py` & `stadiamaps-1.0.4/stadiamaps/models/route_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/route_response.py` & `stadiamaps-1.0.4/stadiamaps/models/route_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/route_response_trip.py` & `stadiamaps-1.0.4/stadiamaps/models/route_response_trip.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/route_summary.py` & `stadiamaps-1.0.4/stadiamaps/models/route_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/routing_response_waypoint.py` & `stadiamaps-1.0.4/stadiamaps/models/routing_response_waypoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/routing_response_waypoint_all_of.py` & `stadiamaps-1.0.4/stadiamaps/models/routing_response_waypoint_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/routing_waypoint.py` & `stadiamaps-1.0.4/stadiamaps/models/routing_waypoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/routing_waypoint_all_of.py` & `stadiamaps-1.0.4/stadiamaps/models/routing_waypoint_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/routing_waypoint_all_of_search_filter.py` & `stadiamaps-1.0.4/stadiamaps/models/routing_waypoint_all_of_search_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/simple_routing_waypoint.py` & `stadiamaps-1.0.4/stadiamaps/models/simple_routing_waypoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/simple_routing_waypoint_all_of.py` & `stadiamaps-1.0.4/stadiamaps/models/simple_routing_waypoint_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/speeds.py` & `stadiamaps-1.0.4/stadiamaps/models/speeds.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/trace_attribute_filter_options.py` & `stadiamaps-1.0.4/stadiamaps/models/trace_attribute_filter_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/trace_attribute_key.py` & `stadiamaps-1.0.4/stadiamaps/models/trace_attribute_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/trace_attributes_base_response.py` & `stadiamaps-1.0.4/stadiamaps/models/trace_attributes_base_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/trace_attributes_request.py` & `stadiamaps-1.0.4/stadiamaps/models/trace_attributes_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/trace_attributes_request_all_of.py` & `stadiamaps-1.0.4/stadiamaps/models/trace_attributes_request_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/trace_attributes_request_all_of_filters.py` & `stadiamaps-1.0.4/stadiamaps/models/trace_attributes_request_all_of_filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/trace_attributes_response.py` & `stadiamaps-1.0.4/stadiamaps/models/trace_attributes_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/trace_attributes_response_all_of.py` & `stadiamaps-1.0.4/stadiamaps/models/trace_attributes_response_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/trace_edge.py` & `stadiamaps-1.0.4/stadiamaps/models/trace_edge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/travel_mode.py` & `stadiamaps-1.0.4/stadiamaps/models/travel_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/traversability.py` & `stadiamaps-1.0.4/stadiamaps/models/traversability.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/truck_costing_options.py` & `stadiamaps-1.0.4/stadiamaps/models/truck_costing_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/truck_costing_options_all_of.py` & `stadiamaps-1.0.4/stadiamaps/models/truck_costing_options_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/tz_response.py` & `stadiamaps-1.0.4/stadiamaps/models/tz_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/valhalla_languages.py` & `stadiamaps-1.0.4/stadiamaps/models/valhalla_languages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/valhalla_long_units.py` & `stadiamaps-1.0.4/stadiamaps/models/valhalla_long_units.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/models/warning.py` & `stadiamaps-1.0.4/stadiamaps/models/warning.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps/rest.py` & `stadiamaps-1.0.4/stadiamaps/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Stadia Maps Geospatial APIs
 
     The Stadia Maps Geospatial APIs provide you with the data you need to build awesome applications.  # noqa: E501
 
-    The version of the OpenAPI document: 5.0.2
+    The version of the OpenAPI document: 5.0.3
     Contact: support@stadiamaps.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `stadiamaps-1.0.3/stadiamaps.egg-info/PKG-INFO` & `stadiamaps-1.0.4/stadiamaps.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stadiamaps
-Version: 1.0.3
+Version: 1.0.4
 Summary: Stadia Maps Geospatial APIs
 Home-page: https://github.com/stadiamaps/stadiamaps-api-py
 Author: Stadia Maps Support
 Author-email: support@stadiamaps.com
 Keywords: OpenAPI,OpenAPI-Generator,Stadia Maps Geospatial APIs
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `stadiamaps-1.0.3/stadiamaps.egg-info/SOURCES.txt` & `stadiamaps-1.0.4/stadiamaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/integration/test_eu_endpoint.py` & `stadiamaps-1.0.4/test/integration/test_eu_endpoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/integration/test_gecoding.py` & `stadiamaps-1.0.4/test/integration/test_gecoding.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/integration/test_geospatial.py` & `stadiamaps-1.0.4/test/integration/test_geospatial.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/integration/test_routing.py` & `stadiamaps-1.0.4/test/integration/test_routing.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_access.py` & `stadiamaps-1.0.4/test/test_access.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_admin_region.py` & `stadiamaps-1.0.4/test/test_admin_region.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_administrative.py` & `stadiamaps-1.0.4/test/test_administrative.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_auto_costing_options.py` & `stadiamaps-1.0.4/test/test_auto_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_auto_costing_options_all_of.py` & `stadiamaps-1.0.4/test/test_auto_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_base_costing_options.py` & `stadiamaps-1.0.4/test/test_base_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_base_trace_request.py` & `stadiamaps-1.0.4/test/test_base_trace_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_bicycle_costing_options.py` & `stadiamaps-1.0.4/test/test_bicycle_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_bicycle_costing_options_all_of.py` & `stadiamaps-1.0.4/test/test_bicycle_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_bike_network.py` & `stadiamaps-1.0.4/test/test_bike_network.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_contour.py` & `stadiamaps-1.0.4/test/test_contour.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_coordinate.py` & `stadiamaps-1.0.4/test/test_coordinate.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_costing_model.py` & `stadiamaps-1.0.4/test/test_costing_model.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_costing_options.py` & `stadiamaps-1.0.4/test/test_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_directions_options.py` & `stadiamaps-1.0.4/test/test_directions_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_distance_unit.py` & `stadiamaps-1.0.4/test/test_distance_unit.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_edge_sign.py` & `stadiamaps-1.0.4/test/test_edge_sign.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_edge_use.py` & `stadiamaps-1.0.4/test/test_edge_use.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_end_node.py` & `stadiamaps-1.0.4/test/test_end_node.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_geo_attributes.py` & `stadiamaps-1.0.4/test/test_geo_attributes.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_geo_json_geometry.py` & `stadiamaps-1.0.4/test/test_geo_json_geometry.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_geo_json_geometry_base.py` & `stadiamaps-1.0.4/test/test_geo_json_geometry_base.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_geo_json_line_string.py` & `stadiamaps-1.0.4/test/test_geo_json_line_string.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_geo_json_line_string_all_of.py` & `stadiamaps-1.0.4/test/test_geo_json_line_string_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_geo_json_point.py` & `stadiamaps-1.0.4/test/test_geo_json_point.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_geo_json_point_all_of.py` & `stadiamaps-1.0.4/test/test_geo_json_point_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_geo_json_polygon.py` & `stadiamaps-1.0.4/test/test_geo_json_polygon.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_geo_json_polygon_all_of.py` & `stadiamaps-1.0.4/test/test_geo_json_polygon_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_geocoding_api.py` & `stadiamaps-1.0.4/test/test_geocoding_api.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_geocoding_object.py` & `stadiamaps-1.0.4/test/test_geocoding_object.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_geospatial_api.py` & `stadiamaps-1.0.4/test/test_geospatial_api.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_height_request.py` & `stadiamaps-1.0.4/test/test_height_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_height_response.py` & `stadiamaps-1.0.4/test/test_height_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_highway_classification.py` & `stadiamaps-1.0.4/test/test_highway_classification.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_intersecting_edge.py` & `stadiamaps-1.0.4/test/test_intersecting_edge.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_isochrone_costing_model.py` & `stadiamaps-1.0.4/test/test_isochrone_costing_model.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_isochrone_feature.py` & `stadiamaps-1.0.4/test/test_isochrone_feature.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_isochrone_properties.py` & `stadiamaps-1.0.4/test/test_isochrone_properties.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_isochrone_request.py` & `stadiamaps-1.0.4/test/test_isochrone_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_isochrone_response.py` & `stadiamaps-1.0.4/test/test_isochrone_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_locate_detailed_edge.py` & `stadiamaps-1.0.4/test/test_locate_detailed_edge.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_locate_edge.py` & `stadiamaps-1.0.4/test/test_locate_edge.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_locate_edge_info.py` & `stadiamaps-1.0.4/test/test_locate_edge_info.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_locate_node.py` & `stadiamaps-1.0.4/test/test_locate_node.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_locate_node_all_of.py` & `stadiamaps-1.0.4/test/test_locate_node_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_locate_object.py` & `stadiamaps-1.0.4/test/test_locate_object.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_maneuver_sign.py` & `stadiamaps-1.0.4/test/test_maneuver_sign.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_maneuver_sign_element.py` & `stadiamaps-1.0.4/test/test_maneuver_sign_element.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_map_match_costing_model.py` & `stadiamaps-1.0.4/test/test_map_match_costing_model.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_map_match_request.py` & `stadiamaps-1.0.4/test/test_map_match_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_map_match_request_all_of.py` & `stadiamaps-1.0.4/test/test_map_match_request_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_map_match_route_response.py` & `stadiamaps-1.0.4/test/test_map_match_route_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_map_match_route_response_all_of.py` & `stadiamaps-1.0.4/test/test_map_match_route_response_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_map_match_trace_options.py` & `stadiamaps-1.0.4/test/test_map_match_trace_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_map_match_waypoint.py` & `stadiamaps-1.0.4/test/test_map_match_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_map_match_waypoint_all_of.py` & `stadiamaps-1.0.4/test/test_map_match_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_matched_point.py` & `stadiamaps-1.0.4/test/test_matched_point.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_matrix_costing_model.py` & `stadiamaps-1.0.4/test/test_matrix_costing_model.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_matrix_distance.py` & `stadiamaps-1.0.4/test/test_matrix_distance.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_matrix_request.py` & `stadiamaps-1.0.4/test/test_matrix_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_matrix_response.py` & `stadiamaps-1.0.4/test/test_matrix_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_motor_scooter_costing_options.py` & `stadiamaps-1.0.4/test/test_motor_scooter_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_motor_scooter_costing_options_all_of.py` & `stadiamaps-1.0.4/test/test_motor_scooter_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_motorcycle_costing_options.py` & `stadiamaps-1.0.4/test/test_motorcycle_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_motorcycle_costing_options_all_of.py` & `stadiamaps-1.0.4/test/test_motorcycle_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_nearest_roads_request.py` & `stadiamaps-1.0.4/test/test_nearest_roads_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_node_id.py` & `stadiamaps-1.0.4/test/test_node_id.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_node_type.py` & `stadiamaps-1.0.4/test/test_node_type.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_optimized_route_request.py` & `stadiamaps-1.0.4/test/test_optimized_route_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_pedestrian_costing_options.py` & `stadiamaps-1.0.4/test/test_pedestrian_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_pelias_geo_json_feature.py` & `stadiamaps-1.0.4/test/test_pelias_geo_json_feature.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_pelias_geo_json_properties.py` & `stadiamaps-1.0.4/test/test_pelias_geo_json_properties.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_pelias_geo_json_properties_addendum.py` & `stadiamaps-1.0.4/test/test_pelias_geo_json_properties_addendum.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_pelias_geo_json_properties_addendum_osm.py` & `stadiamaps-1.0.4/test/test_pelias_geo_json_properties_addendum_osm.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_pelias_layer.py` & `stadiamaps-1.0.4/test/test_pelias_layer.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_pelias_response.py` & `stadiamaps-1.0.4/test/test_pelias_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_pelias_response_geocoding.py` & `stadiamaps-1.0.4/test/test_pelias_response_geocoding.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_pelias_source.py` & `stadiamaps-1.0.4/test/test_pelias_source.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_restrictions.py` & `stadiamaps-1.0.4/test/test_restrictions.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_road_class.py` & `stadiamaps-1.0.4/test/test_road_class.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_route_leg.py` & `stadiamaps-1.0.4/test/test_route_leg.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_route_maneuver.py` & `stadiamaps-1.0.4/test/test_route_maneuver.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_route_request.py` & `stadiamaps-1.0.4/test/test_route_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_route_response.py` & `stadiamaps-1.0.4/test/test_route_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_route_response_trip.py` & `stadiamaps-1.0.4/test/test_route_response_trip.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_route_summary.py` & `stadiamaps-1.0.4/test/test_route_summary.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_routing_api.py` & `stadiamaps-1.0.4/test/test_routing_api.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_routing_response_waypoint.py` & `stadiamaps-1.0.4/test/test_routing_response_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_routing_response_waypoint_all_of.py` & `stadiamaps-1.0.4/test/test_routing_response_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_routing_waypoint.py` & `stadiamaps-1.0.4/test/test_routing_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_routing_waypoint_all_of.py` & `stadiamaps-1.0.4/test/test_routing_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_routing_waypoint_all_of_search_filter.py` & `stadiamaps-1.0.4/test/test_routing_waypoint_all_of_search_filter.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_simple_routing_waypoint.py` & `stadiamaps-1.0.4/test/test_simple_routing_waypoint.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_simple_routing_waypoint_all_of.py` & `stadiamaps-1.0.4/test/test_simple_routing_waypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_speeds.py` & `stadiamaps-1.0.4/test/test_speeds.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_trace_attribute_filter_options.py` & `stadiamaps-1.0.4/test/test_trace_attribute_filter_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_trace_attribute_key.py` & `stadiamaps-1.0.4/test/test_trace_attribute_key.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_trace_attributes_base_response.py` & `stadiamaps-1.0.4/test/test_trace_attributes_base_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_trace_attributes_request.py` & `stadiamaps-1.0.4/test/test_trace_attributes_request.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_trace_attributes_request_all_of.py` & `stadiamaps-1.0.4/test/test_trace_attributes_request_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_trace_attributes_request_all_of_filters.py` & `stadiamaps-1.0.4/test/test_trace_attributes_request_all_of_filters.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_trace_attributes_response.py` & `stadiamaps-1.0.4/test/test_trace_attributes_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_trace_attributes_response_all_of.py` & `stadiamaps-1.0.4/test/test_trace_attributes_response_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_trace_edge.py` & `stadiamaps-1.0.4/test/test_trace_edge.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_travel_mode.py` & `stadiamaps-1.0.4/test/test_travel_mode.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_traversability.py` & `stadiamaps-1.0.4/test/test_traversability.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_truck_costing_options.py` & `stadiamaps-1.0.4/test/test_truck_costing_options.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_truck_costing_options_all_of.py` & `stadiamaps-1.0.4/test/test_truck_costing_options_all_of.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_tz_response.py` & `stadiamaps-1.0.4/test/test_tz_response.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_valhalla_languages.py` & `stadiamaps-1.0.4/test/test_valhalla_languages.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_valhalla_long_units.py` & `stadiamaps-1.0.4/test/test_valhalla_long_units.py`

 * *Files identical despite different names*

### Comparing `stadiamaps-1.0.3/test/test_warning.py` & `stadiamaps-1.0.4/test/test_warning.py`

 * *Files identical despite different names*

