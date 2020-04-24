.. _featurestoraster:

Features To Raster
==================

Converts features to a raster dataset.

**Syntax**

FeaturesToRaster (SimpleFeatureCollection inputFeatures, String inputField, Double cellSize, ReferencedEnvelope extent) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The input feature to be converted to a raster dataset.
     - SimpleFeatureCollection
     - 
     - ✓

   * - inputField
     - The field used to assign values to the output raster.
     - String
     - 
     - 

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

