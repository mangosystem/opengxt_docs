.. _removeholes:

폴리곤 홀 제거
========================

설정된 면적 기준으로 폴리곤의 홀(Hole, Interior Ring)을 제거합니다.

**Syntax**

RemoveHoles (SimpleFeatureCollection inputFeatures, Expression minimumArea) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 홀을 제거할 입력 폴리곤 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - minimumArea
     - 이 면적 필터 표현식의 값보다 작은 홀은 삭제합니다. 예) 10.0 또는 필터 표현식
     - Expression
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
     - 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - minimumArea는 숫자 또는 필드값 등을 조합하여 숫자를 반환하는 Expression이 가능하다.
 - minimumArea 파라미터의 값이 0이면 폴리곤의 모든 Hole(Interior Ring)이 삭제되고, 0보다 크면 해당 값보다 면적이 작은 Hole만 삭제된다.


**Examples**
