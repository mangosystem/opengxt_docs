.. _simplify:

라인 단순화
==================

Douglas-Peucker 단순화 알고리즘을 이용하여 라인 피처를 단순화합니다.

**Syntax**

Simplify (SimpleFeatureCollection inputFeatures, Expression tolerance, Boolean preserveTopology) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 단순화할 라인 또는 폴리곤 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - tolerance
     - 단순화 알고리즘에 사용할 거리 오차 표현식입니다. 예) 10.0 또는 필터 표현식.
     - Expression
     -
     - ✓

   * - preserveTopology
     - 만약 참이면, 단순화된 피처는 유효한 토폴로지를 보장합니다.
     - Boolean
     - true
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

 - tolerance 파라미터는 수 또는 수식을 사용할 수 있으며, Douglas–Peucker 알고리즘을 사용한다.
 - preserveTopology 파라미터 값이 True이면, Tolerance 값에 상관없이 최소한의 토폴로지 규칙은 유지된다.


**Examples**

파란선은 원본, 빨간 선은 Simplify 결과 입니다.

  .. image:: images/simplify.png
