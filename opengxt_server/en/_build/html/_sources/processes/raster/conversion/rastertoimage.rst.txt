.. _rastertoimage:

Raster To Image
===============

Retrieves a map from raster and map parameters.

**Syntax**

RasterToImage (GridCoverage2D coverage, String bbox, CoordinateReferenceSystem crs, Style style, Integer width, Integer height, String format, Boolean transparent, String bgColor) : MapToImageParam

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - coverage
     - The input raster to be converted.
     - GridCoverage2D
     - 
     - ✓

   * - bbox
     - Bounding box corners (lower left, upper right): minx,miny,maxx,maxy.
     - String
     - 
     - 

   * - crs
     - CRS for Bounding Box.
     - CoordinateReferenceSystem
     - 
     - 

   * - style
     - Styled Layer Descriptor (SLD) style containing a raster symbolizer.
     - Style
     - 
     - 

   * - width
     - Image width in pixels of resulting map.
     - Integer
     - 
     - ✓

   * - height
     - Image height in pixels of resulting map.
     - Integer
     - 
     - ✓

   * - format
     - Output format of map. Valid values are image/jpeg, image/png, and image/gif.
     - String
     - image/png
     - 

   * - transparent
     - Map background transparency. Default is True.
     - Boolean
     - true
     - 

   * - bgColor
     - Hexidecimal red-blue-green color value for the map background color. Default is 0xFFFFFF (white).
     - String
     - 0xFFFFFF
     - 

**Process Outputs**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - result
     - Result image.
     - MapToImageParam
     - 
     - ✓

**Constraints**

 

**Examples**

