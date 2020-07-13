.. _rastercutfill:

Cut Fill
===========

Calculates the volume change between two surfaces.

**Syntax**

RasterCutFill(GridCoverage2D inputDEM, Geometry cropShape, Double baseHeight): SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - The input surface raster to be processed.
     - GridCoverage2D
     -
     - ✓

   * - cropShape
     - The Polygon or MultiPolygon to clip raster.
     - Geometry
     -
     - ✓

   * - baseHeight
     - The default height of Crop Geometry, Default is -9999.
     - Double
     - -9999
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
     - Output features.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**


**Examples**
