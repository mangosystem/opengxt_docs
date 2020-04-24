.. _pointdensity:

Point Density
=============

Calculates a magnitude per unit area from point features that fall within a neighborhood around each cell.

**Syntax**

PointDensity (SimpleFeatureCollection inputFeatures, String populationField, String neighborhood, Double cellSize, ReferencedEnvelope extent) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The input point features for which to calculate the density.
     - SimpleFeatureCollection
     - 
     - ✓

   * - populationField
     - The field denoting population values for each feature.
     - String
     - 
     - 

   * - neighborhood
     - Neighborhood: Circle + Radius, Rectangle + width + height, default = Circle + Radius
     - String
     - 
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
     - The output raster.
     - GridCoverage2D
     - 
     - ✓

**Constraints**

 

**Examples**

