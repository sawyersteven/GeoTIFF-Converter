## GeoTiff Converter Cmdlet

This is a converter from GeoTIFF to STL format (because its easy to write a STL writer).
Its aim is to be very simple to use.

# Usage instructions
1. open powershell in module folder
2. import-module .\GeoTiffConverter.dll
3. convert-geotiff -path path_to_tiff_file

by default, outputs to output.stl in the same directory as the geoTIFF file.
use help convert-geotiff to see additional options.

RenderFaces: render faces, instead of just points.

Scale: scale all values by this amount. Default is 0.1

MaxY: max Y value to convert to. Default is the entire file.

Text: Output text stl file (usually does binary). Much larger, useful for debugging errors but thats about it

Stats: Output a dict containing x,y,z info


