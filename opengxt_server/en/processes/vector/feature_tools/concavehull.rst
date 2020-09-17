.. _concavehull:

Concave Hull - Alpha Shapes
=================================

Creates a concave hull using the alpha shapes algorithm.

**Syntax**

ConcaveHull (SimpleFeatureCollection features, Expression group, Double alpha, Boolean removeHoles, Boolean splitMultipart): SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - features
     - Input features to be processed.
     - SimpleFeatureCollection
     -
     - ✓

   * - group
     - The field or expression used to group features for separate concave hull computations.
     - Expression
     - 
     -

   * - alpha
     - Threshold (0-1, where 1 is equivalent with Convex Hull).
     - Double
     - 0.3
     -

   * - removeHoles
     - Removes the holes from the concave polygon.
     - Boolean
     - false
     -

   * - splitMultipart
     - Split multipart geometry into singleparts geometries.
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
     - Output features.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**


**Examples**
