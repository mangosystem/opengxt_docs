.. _calculatefield:

필드 계산하기
=====================

계산식에 기반하여 새로운 필드값을 계산합니다. 미리 정의된 함수를 사용하여 문자, 숫자, 지오메트리 연산을 수행할 수 있습니다.

**Syntax**

CalculateField (SimpleFeatureCollection inputFeatures, Expression expression, String fieldName) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 계산할 벡터 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - expression
     - 다음 예와 같은 간단한 계산식입니다. 예) [population] / ([geom_area] / 1000000)
     - Expression
     -
     - ✓

   * - fieldName
     - 계산식이 저장될 필드 이름입니다.
     - String
     - evaluated
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

 - Expression 에 의해 반환되는 값이 Geometry인 경우 fieldName은 무시되고 반환되는 데이터의 Geometry값이 적용된다.

**Examples**
