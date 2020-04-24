.. _rasterhillshade:

Hillshade
=========

Creates a shaded relief from a surface raster by considering the illumination source angle and shadows.

**Syntax**

RasterHillshade (GridCoverage2D inputCoverage, Double azimuth, Double altitude, Double zFactor) : GridCoverage2D

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

   * - azimuth
     - Azimuth angle of the light source. The default is 315 degrees.
     - Double
     - 315.0
     - 

   * - altitude
     - Altitude angle of the light source above the horizon. The default is 45 degrees.
     - Double
     - 45.0
     - 

   * - zFactor
     - The number of ground x,y units in one surface z unit.
     - Double
     - 1.0
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

