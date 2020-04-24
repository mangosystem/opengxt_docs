.. _reproject:

Reproject
=========

Reprojects features into a supplied coordinate reference system.

**Syntax**

Reproject (SimpleFeatureCollection inputFeatures, CoordinateReferenceSystem forcedCRS, CoordinateReferenceSystem targetCRS) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - Input features that will be reprojected.
     - SimpleFeatureCollection
     - 
     - ✓

   * - forcedCRS
     - Coordinate reference system to use for input features.
     - CoordinateReferenceSystem
     - 
     - 

   * - targetCRS
     - Target coordinate reference system to use for reprojection.
     - CoordinateReferenceSystem
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
     - Output Features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

