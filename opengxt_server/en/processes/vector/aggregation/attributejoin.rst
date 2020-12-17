.. _attributejoin:

속성 기반 조인
========================

공통 필드를 이용하여 두 레이어를 조인합니다.

**Syntax**

AttributeJoin (SimpleFeatureCollection inputFeatures, String primaryKey, SimpleFeatureCollection joinFeatures, String foreignKey, Type joinType) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 입력 레이어.
     - SimpleFeatureCollection
     -
     - ✓

   * - primaryKey
     - 입력 레이어의 원본 키 필드입니다.
     - String
     -
     - ✓

   * - joinFeatures
     - 조인 대상 레이어.
     - SimpleFeatureCollection
     -
     - ✓

   * - foreignKey
     - 조인 레이어의 키 필드입니다.
     - String
     -
     - ✓

   * - joinType
     - 조인 유형입니다.
     - Type
     - INNER
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

 - joinType: INNER(기본값), OUTER
 - joinType이 INNER인 경우 조인되는 inputFeatures 의 피처만을 반환한다.

**Examples**

대형매장과 시군구 행정경계의 시군구코드를 Join 필드로 사용하여 조인한 결과입니다.

  .. image:: images/attributejoin.png
