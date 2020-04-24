.. _snappointstolines:

Snap Points To Lines
====================

Snaps each point in the point features to the closest point on the nearest line in the line features, provided it is within the user defined snap tolerance.

**Syntax**

SnapPointsToLines (SimpleFeatureCollection pointFeatures, SimpleFeatureCollection lineFeatures, Double tolerance) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - pointFeatures
     - Point features to be snapped.
     - SimpleFeatureCollection
     - 
     - ✓

   * - lineFeatures
     - Line features that can be Line or polygon boundary.
     - SimpleFeatureCollection
     - 
     - ✓

   * - tolerance
     - Snap tolerance. if tolerance is 0, nearest line feature will be used.
     - Double
     - 0.0
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

