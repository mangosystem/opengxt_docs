.. _featuretoline:

피처를 라인으로 변환
=================================

폴리곤 경계를 라인으로 변환하거나 라인, 폴리곤간 교차점으로 분할한 라인 피처를 생성합니다.


**Syntax**

FeatureToLine (SimpleFeatureCollection inputFeatures, Boolean preserveAttributes) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 변환할 라인 또는 폴리곤 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - preserveAttributes
     - 출력 레이어에 입력 레이어의 속성값을 유지할 지 여부를 설정합니다.
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
     - 라인으로 변환한 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - inputFeatures 레이어는 라인 또는 폴리곤 타입이어야 한다.
 - preserveAttributes 파라미터의 기본값을 True이며, True인 경우 원본 피처의 속성값을 유지한다.

**Examples**

폴리곤 레이어를 라인으로 변환한 결과입니다. 
변환된 라인은 다음 그림과 같이 폴리곤을 공유하는 세그먼트 단위로 분할됩니다.

  .. image:: images/featuretoline.png
