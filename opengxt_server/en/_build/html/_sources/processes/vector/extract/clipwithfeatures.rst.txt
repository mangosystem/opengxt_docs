.. _clipwithfeatures:

Clip With Polygon Features
==========================

Extracts input features that overlay the clip polygon features.

**Syntax**

ClipWithFeatures (SimpleFeatureCollection inputFeatures, SimpleFeatureCollection clipFeatures) : SimpleFeatureCollection

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

   * - clipFeatures
     - The features used to clip the input features.
     - SimpleFeatureCollection
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

