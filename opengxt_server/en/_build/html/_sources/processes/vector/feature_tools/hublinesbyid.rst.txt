.. _hublinesbyid:

Hub Lines By ID
===============

Creates a line features representing the shortest distance between hub and spoke features by id.

**Syntax**

HubLinesByID (SimpleFeatureCollection hubFeatures, String hubIdField, SimpleFeatureCollection spokeFeatures, String spokeIdField, Boolean preserveAttributes, Boolean useCentroid, Boolean useBezierCurve, Double maximumDistance) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - hubFeatures
     - Hub Features.
     - SimpleFeatureCollection
     - 
     - ✓

   * - hubIdField
     - Hub id field.
     - String
     - 
     - ✓

   * - spokeFeatures
     - Spoke Features.
     - SimpleFeatureCollection
     - 
     - ✓

   * - spokeIdField
     - Spoke id field.
     - String
     - 
     - ✓

   * - preserveAttributes
     - Preserve spoke feature's attributes.
     - Boolean
     - true
     - 

   * - useCentroid
     - Use centroid of feature.
     - Boolean
     - true
     - 

   * - useBezierCurve
     - Use Bezier Curve.
     - Boolean
     - false
     - 

   * - maximumDistance
     - Maximum distance.
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
     - Result HubLines.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

