.. _statisticsgridcoverage:

Summary Statistics for Raster
=============================

Calculates summary statistics(Sum, Minimum, Maximum, Mean, Standard Deviation etc.) in a raster.

**Syntax**

StatisticsGridCoverage (GridCoverage2D inputCoverage, Geometry cropShape, Integer bandIndex) : DataStatisticsResult

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - The input raster to be calculated.
     - GridCoverage2D
     - 
     - ✓

   * - cropShape
     - The Polygon or MultiPolygon to crop raster.
     - Geometry
     - 
     - 

   * - bandIndex
     - The zero-based band index, default index is a 0.
     - Integer
     - 0
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
     - Result Statistics.
     - DataStatisticsResult
     - 
     - ✓

**Constraints**

 

**Examples**

