.. _histogramgridcoverage:

Histogram Raster
================

Derives value-frequency pairs from pixels in a raster within crop geometry.

**Syntax**

HistogramGridCoverage (GridCoverage2D inputCoverage, Integer bandIndex, Geometry cropShape) : HistogramProcessResult

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

   * - bandIndex
     - The zero-based band index, default index is a 0.
     - Integer
     - 0
     - 

   * - cropShape
     - The Polygon or MultiPolygon to crop raster.
     - Geometry
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
     - Result histogram data.
     - HistogramProcessResult
     - 
     - ✓

**Constraints**

 

**Examples**

