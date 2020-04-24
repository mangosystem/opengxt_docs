.. _tps:

Thin Plate Spline(TPS) Interpolation
====================================

Interpolates a surface from points using a Thin Plate Spline(TPS) interpolation technique.

**Syntax**

TPS (SimpleFeatureCollection inputFeatures, String inputField, Double cellSize, ReferencedEnvelope extent) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The input point features for which to calculate the interpolation.
     - SimpleFeatureCollection
     - 
     - ✓

   * - inputField
     - The field that holds a height or magnitude value for each point.
     - String
     - 
     - ✓

   * - cellSize
     - The cell size for the output raster.
     - Double
     - 0.0
     - 

   * - extent
     - The extent for the output raster.
     - ReferencedEnvelope
     - 
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
     - The output raster.
     - GridCoverage2D
     - 
     - ✓

**Constraints**

 

**Examples**

