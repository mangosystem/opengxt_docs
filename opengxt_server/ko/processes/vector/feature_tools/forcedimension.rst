.. _forcedimension:

지오메트리 차원 변환
=========================

피처의 지오메트리에 대한 차원(XY, XYZ, XYM, XYZM)을 변환합니다.

**Syntax**

ForceDimension(SimpleFeatureCollection inputFeatures, DimensionType dimension, Expression zField, Expression mField): SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 피처의 지오메트리 차원을 변환할 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - dimension
     - 변환할 지오메트리의 차원(XY, XYZ, XYM, XYZM). 기본값은 XY(2D)입니다.
     - DimensionType
     - XY
     - ✓

   * - zField
     - Z 값을 적용할 표현식입니다. 예) 1000 또는 [field] 또는 [field] * 0.5 등...
     - Expression
     -
     - 

   * - mField
     - M 값을 적용할 표현식입니다. 예) 1000 또는 [field] 또는 [field] * 0.5 등...
     - Expression
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
     - 출력 레이어.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - inputFeatures는 포인트, 라인, 폴리곤 모두 가능하다.
 - dimension: XY(기본값), XYZ, XYM, XYZM
 - zField, mField expression은 숫자, 숫자가 리턴되는 `함수식 <http://docs.geoserver.org/stable/en/user/filter/function_reference.html>`_ 모두 가능하다.


**Examples**
