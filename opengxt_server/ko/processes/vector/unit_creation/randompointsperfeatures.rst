.. _randompointsperfeatures:

피처별 랜덤 포인트 생성
=======================================

폴리곤 피처별로 랜덤 포인트를 생성합니다.

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
     - 랜덤 포인트가 생성될 폴리곤 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - expression
     - 포인트 갯수를 지정하는 필드 또는 계산식 입니다.
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
     - 랜덤 포인트 피처컬렉션
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - Expression 파라미터를 숫자, 필드 또는 수식(여러 공간 및 속성 필드의 연산 조합)으로 입력이 가능하다.
 - 수식을 이용하는 경우 폴리곤 레이어의 각 피처별로 랜덤 포인트의 개수 설정이 가능하다.

**Examples**
