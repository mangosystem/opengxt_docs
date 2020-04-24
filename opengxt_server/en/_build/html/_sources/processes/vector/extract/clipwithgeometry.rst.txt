.. _clipwithgeometry:

Clip With Polygon Geometry
==========================

Extracts input features that overlay the clip polygon geometry.

**Syntax**

ClipWithGeometry (SimpleFeatureCollection inputFeatures, Geometry clipGeometry) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The features to be clipped.
     - SimpleFeatureCollection
     - 
     - ✓

   * - clipGeometry
     - The polygon geometry used to clip the input features.
     - Geometry
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
     - Output features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

