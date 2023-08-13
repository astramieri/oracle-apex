# APEX Maps

Oracle APEX has a region type called Maps using which you can visualize location data, real coordinates which are available in the database table in your APEX application. 

Using Maps region, the developer can show a world map on a page and can add one or more layers or data points on top of this map. These data points can be coming from a table in your database or through a SQL query, using which you can show features on this map. The background map is a static map, and it is coming from the **Oracle Elocation Services**. And these background maps are ready to use and do not require any API keys.

Developers can also add Faceted Search on top of a map, using which you can filter the data in the map based on the filter criteria applied by the user using the facets. 

Supported spatial geometry objects include:
- **Points** (for example, customer or supplier locations) display as markers. 
- **Lines** represent features like roads or paths.
- **Polygons** represent areas like parcels, states or countries.
- **Heat Maps** are used to visualize the point density. The more points that are clustered together, the more intense the color becomes. Use this option to visualize the spatial distribution of population or incidents.
- **Extruded Polygons** - Display as three-dimensional, extruded, objects. The height of the 3D object visualizes a column value.

You can source spatial geometry objects from either:

- **Geometry Column** - Supported datatypes include SDO_GEOMETRY, VARCHAR2, or CLOB. VARCHAR2 and CLOB columns must contain geometry information in GeoJSON format.
- **Two Numeric Columns** - These columns must contain longitude and latitude values. This option only applies to Point and Heat Map objects.