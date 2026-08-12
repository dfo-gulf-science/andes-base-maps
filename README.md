# andes-base-maps
XYZ base map tiles for andes


The maps used for the Andes base layers are the Carto (Vector Tiles), accessed through the NextGIS QMS QGIS plugin. 

<img width="638" height="482" alt="image" src="https://github.com/user-attachments/assets/295e2e91-01f3-4c96-82cc-e8c0ef60d698" />

The tiles were generated using the following routine: `Processing Toolbox > Generate XYZ tiles (Directory)`

For each map (Dark Matter without labels and Voyager without labels), the following parameters were used:

For extents 0 to 8:
```
{
    'ANTIALIAS': True,
    'BACKGROUND_COLOR': QColor(0, 0, 0, 0),
    'DPI': 95,
    'EXTENT': '-20037508.3428,20037508.3428,-20037508.3428,20037508.3428 [EPSG:3857]',
    'HTML_ATTRIBUTION': '',
    'HTML_OSM': False,
    'HTML_TITLE': '',
    'METATILESIZE': 4,
    'OUTPUT_DIRECTORY' : '/path/to/repo/[light|dark]', 
    'OUTPUT_HTML': 'TEMPORARY_OUTPUT',
    'QUALITY': 75,
    'TILE_FORMAT': 0,
    'TILE_HEIGHT': 256,
    'TILE_WIDTH': 256, 
    'TMS_CONVENTION': False, 
    'ZOOM_MAX': 13,
    'ZOOM_MIN': 9
}
```

For extents 9 to 13:
```
{ 
    'ANTIALIAS' : True, 
    'BACKGROUND_COLOR' : QColor(0, 0, 0, 0), 
    'DPI' : 95, 
    'EXTENT' : '-8281424.621100000,-4887836.935600000,5116015.812200000,7015644.781000000 [EPSG:3857]', 
    'HTML_ATTRIBUTION' : '', 
    'HTML_OSM' : False, 
    'HTML_TITLE' : '', 
    'METATILESIZE' : 4, 
    'OUTPUT_DIRECTORY' : '/path/to/repo/[light|dark]', 
    'OUTPUT_HTML' : 'TEMPORARY_OUTPUT', 
    'QUALITY' : 75, 
    'TILE_FORMAT' : 0, 
    'TILE_HEIGHT' : 256, 
    'TILE_WIDTH' : 256, 
    'TMS_CONVENTION' : False, 
    'ZOOM_MAX' : 13, 
    'ZOOM_MIN' : 9 
}
```
