.. _tininterpolation:

Triangulated Irregular Network(TIN) Interpolation
===========================================================================

Interpolates a raster surface from points using an Triangulated Irregular Network(TIN) technique.

**Syntax**

TINInterpolation (SimpleFeatureCollection inputFeatures, Expression inputField, RasterPixelType pixelType, Double cellSize, ReferencedEnvelope extent) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The input features for which to calculate the interpolation.
     - SimpleFeatureCollection
     -
     - ✓

   * - inputField
     - The field that holds a height or magnitude value for each point.
     - Expression
     -
     - ✓

   * - pixelType
     - The pixel type for the output raster.
     - RasterPixelType
     - Float
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
     - The output TIN Interpolation raster.
     - GridCoverage2D
     -
     - ✓

**Constraints**

- pixelType: BYTE, SHORT, INTEGER, FLOAT(default), DOUBLE

**Examples**
