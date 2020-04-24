.. _delaunaytriangulation:

Delaunay Triangulation Polygons
===============================

Creates delaunay triangulation polygons from input point features.

**Syntax**

DelaunayTriangulation (SimpleFeatureCollection inputFeatures, Geometry clipArea) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The point input features from which delaunay Triangulations will be generated.
     - SimpleFeatureCollection
     - 
     - ✓

   * - clipArea
     - Clip area polygon.
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
     - Result Polygons.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

