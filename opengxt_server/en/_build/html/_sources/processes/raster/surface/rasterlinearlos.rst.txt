.. _rasterlinearlos:

Linear Line Of Sight
====================

Determines the visibility a surface within a specified radius and field of view of an observation point.

**Syntax**

LinearLineOfSight (GridCoverage2D inputCoverage, Geometry observerPoint, Double observerOffset, Geometry targetPoint, Boolean useCurvature, Boolean useRefraction, Double refractionFactor) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - The input surface raster.
     - GridCoverage2D
     - 
     - ✓

   * - observerPoint
     - The observer's coordinate.
     - Geometry
     - 
     - ✓

   * - observerOffset
     - The observer's offset above the surface rater. The default is 0.0 units.
     - Double
     - 0.0
     - ✓

   * - targetPoint
     - The target's coordinate.
     - Geometry
     - 
     - ✓

   * - useCurvature
     - Indicates whether the earth's curvature should be taken into consideration for the line-of-sight analysis. 
     - Boolean
     - false
     - 

   * - useRefraction
     - Indicates whether atmospheric refraction should be taken into consideration when generating a line of sight from a functional surface.
     - Boolean
     - false
     - 

   * - refractionFactor
     - The refraction factor. The default refraction factor is 0.13.
     - Double
     - 0.13
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
     - Output features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

