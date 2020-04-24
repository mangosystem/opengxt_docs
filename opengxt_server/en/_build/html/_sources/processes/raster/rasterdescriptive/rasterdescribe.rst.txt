.. _rasterdescribe:

Raster Description
==================

Describes the metadata of raster.

**Syntax**

RasterDescribe (GridCoverage2D inputCoverage, Boolean detailed) : RasterDescribeResult

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - The input raster to be described.
     - GridCoverage2D
     - 
     - ✓

   * - detailed
     - Specify whether to calculate statistics. default is false.
     - Boolean
     - false
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
     - Output result.
     - RasterDescribeResult
     - 
     - ✓

**Constraints**

 

**Examples**

