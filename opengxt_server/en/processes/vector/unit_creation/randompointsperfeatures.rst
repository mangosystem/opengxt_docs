.. _randompointsperfeatures:

Create random points per polygon features
=========================================

Create random points per polygon features.

**Syntax**

RandomPointsPerFeatures (SimpleFeatureCollection polygonFeatures, Expression expression) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - polygonFeatures
     - The features which contains the features into which the random points will be placed.
     - SimpleFeatureCollection
     - 
     - ✓

   * - expression
     - Field or Expression representing Number of Points.
     - Expression
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
     - Generated random point features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

