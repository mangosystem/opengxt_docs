.. _linedensity:

Line Density
============

Calculates the density of linear features in the neighborhood of each output raster cell.

**Syntax**

LineDensity (SimpleFeatureCollection inputFeatures, String populationField, Double searchRadius, Double cellSize, ReferencedEnvelope extent) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The input line features for which to calculate the density.
     - SimpleFeatureCollection
     - 
     - ✓

   * - populationField
     - The field denoting population values for each feature.
     - String
     - 
     - 

   * - searchRadius
     - The search radius within which to calculate density.
     - Double
     - 0.0
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
     - The output density raster.
     - GridCoverage2D
     - 
     - ✓

**Constraints**

 

**Examples**

