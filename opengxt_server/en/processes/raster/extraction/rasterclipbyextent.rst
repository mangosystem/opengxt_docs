.. _rasterclipbyextent:

Clip By Extent
==============

Extracts the subset of a raster based on an envelope.

**Syntax**

RasterClipByExtent (GridCoverage2D inputCoverage, ReferencedEnvelope cropShape) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - The input raster to be clipped.
     - GridCoverage2D
     - 
     - ✓

   * - cropShape
     - The Reference envelope to clip raster.
     - ReferencedEnvelope
     - 
     - ✓

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

