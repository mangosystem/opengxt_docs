.. _rastersetnull:

Set Null
========

Sets identified cell locations to NoData based on a specified filter expression.

**Syntax**

RasterSetNull (GridCoverage2D inputCoverage, Integer bandIndex, Filter filter, Boolean replaceNoData, Double newValue) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - The input raster to be evaluated.
     - GridCoverage2D
     - 
     - ✓

   * - bandIndex
     - The zero-based band index, default index is a 0.
     - Integer
     - 0
     - 

   * - filter
     - A logical expression that determines which of the input cells are to be nodata. ex> Value > 250
     - Filter
     - 
     - ✓

   * - replaceNoData
     - If true, nodata value will be replaced as a newValue parameter. Default is False.
     - Boolean
     - false
     - 

   * - newValue
     - The new valid value to replace nodata.
     - Double
     - 0.0
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
     - Output raster.
     - GridCoverage2D
     - 
     - ✓

**Constraints**

 

**Examples**

