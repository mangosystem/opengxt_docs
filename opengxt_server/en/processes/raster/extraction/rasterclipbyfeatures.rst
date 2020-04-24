.. _rasterclipbyfeatures:

Clip By Features
================

Extracts the subset of a raster based on a polygon features.

**Syntax**

RasterClipByFeatures (GridCoverage2D inputCoverage, SimpleFeatureCollection cropFeatures) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - The input raster to be clipped.
     - GridCoverage2D
     - 
     - ✓

   * - cropFeatures
     - The Polygon or MultiPolygon features to clip raster.
     - SimpleFeatureCollection
     - 
     - ✓

**Process Outputs**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - result
     - Output raster.
     - GridCoverage2D
     - 
     - ✓

**Constraints**

 

**Examples**

