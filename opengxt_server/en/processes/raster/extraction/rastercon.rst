.. _rastercon:

Conditional Evaluation
======================

Performs a conditional if/else evaluation on each of the input cells of an input raster.

**Syntax**

RasterCon (GridCoverage2D inputCoverage, Integer bandIndex, Filter filter, Integer trueValue, Integer falseValue) : GridCoverage2D

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
     - A logical expression that determines which of the input cells are to be true or false. ex> Value > 250
     - Filter
     - 
     - ✓

   * - trueValue
     - The input whose values will be used as the output cell values if the condition is true.
     - Integer
     - 1
     - ✓

   * - falseValue
     - The input whose values will be used as the output cell values if the condition is false.
     - Integer
     - -2147483648
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

