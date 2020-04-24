.. _ols:

Ordinary Least Squares (OLS)
============================

Performs Ordinary Least Squares (OLS) linear regression.

**Syntax**

OrdinaryLeastSquares (SimpleFeatureCollection inputFeatures, String dependentVariable, String explanatoryVariables) : SimpleFeatureCollection, OLSResult

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The features containing the dependent and independent variables for analysis.
     - SimpleFeatureCollection
     - 
     - ✓

   * - dependentVariable
     - The numeric field containing values for what you are trying to model.
     - String
     - 
     - ✓

   * - explanatoryVariables
     - The comma separated fields representing explanatory variables in your regression model.
     - String
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

   * - olsFeatures
     - The output features to receive dependent variable estimates and residuals.
     - SimpleFeatureCollection
     - 
     - 

   * - report
     - Output OLS results.
     - OLSResult
     - 
     - ✓

**Constraints**

 

**Examples**

