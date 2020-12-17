.. _mergefeatures:

피처 레이어 병합
===========================

같은 지오메트리 유형을 가진 여러 레이어를 하나의 레이어로 병합합니다.

**Syntax**

MergeFeatures (SimpleFeatureCollection features) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - features
     - 병합할 피처 레이어 목록입니다.
     - SimpleFeatureCollection
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
     - 병합된 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - features 파라미터는 동일한 피처 타입이어야 한다.
 - features 파라미터는 컬렉션 타입이므로 1개 이상의 피처 레이어를 사용할 수 있으며, 아래의 요청문을 참조한다.
 - 출력 레이어의 스키마는 features 파라미터의 첫번째 레이어 스키마를 따른다.


**Examples**

3개의 폴리곤 레이어를 하나의 레이어로 병합한 결과입니다.

  .. image:: images/mergefeatures.png
