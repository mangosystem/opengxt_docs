.. _rasterradiallos:

Radial Line Of Sight
====================

Determines the visibility a surface within a specified radius and field of view of an observation point.

**Syntax**

RadialLineOfSight (GridCoverage2D inputCoverage, Geometry observerPoint, Double observerOffset, Double radius, Integer sides, Boolean useCurvature, Boolean useRefraction, Double refractionFactor) : SimpleFeatureCollection

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

   * - radius
     - The radius from the observer point, for which the radial visibility will be calculated. The radius unit must be in meters.
     - Double
     - 0.0
     - ✓

   * - sides
     - The number of sides. The default sides is 180.
     - Integer
     - 180
     - 

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

