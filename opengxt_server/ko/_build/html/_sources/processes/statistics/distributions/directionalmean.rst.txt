.. _directionalmean:

선형 방향 평균
========================

라인들의 지리적 중심점을 기준으로 라인 집합의 평균 방향, 길이를 표시하는 라인을 생성합니다.

**Syntax**

LinearDirectionalMean (SimpleFeatureCollection inputFeatures, Boolean orientationOnly, String caseField) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 선형 방향 평균을 계산하는데 사용될 입력 피처 레이어를 설정합니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - orientationOnly
     - 예(True)인 경우 방향성만, 아니오(False)인 경우 시작 및 끝 노드의 방향성을 고려합니다.
     - Boolean
     - true
     -

   * - caseField
     - 그룹별 중심을 적용하는 경우 그룹을 구분하는데 사용되는 필드를 설정합니다.
     - String
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
     - 저장할 결과 라인 레이어를 설정합니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - inputFeatures는 반드시 라인 피처 타입이어야 한다.

**Examples**

길이와 방향성을 가진 라인 레이어에 대한 Linear Directional Mean 분석을 수행한 결과입니다.

  .. image:: images/directionalmean.png
