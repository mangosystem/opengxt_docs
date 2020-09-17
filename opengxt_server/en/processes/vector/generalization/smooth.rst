.. _smooth:

Smooth
==================

Smooths the geometries in a line or polygon layer. The smoothing algorithm inserts new vertices which are positioned using Bezier splines.

**Syntax**

Smooth (SimpleFeatureCollection features, Double fit): SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - features
     - Input line or polygon features to be processed.
     - SimpleFeatureCollection
     -
     - ✓

   * - fit
     - The value between 0 and 1 (inclusive) specifying the tightness of fit of the smoothed boundary (0 is loose)
     - Double
     - 0.3
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

 - The fit parameter uses a Double value between 0 and 1.


**Examples**

