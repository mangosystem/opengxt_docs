.. _concealment:

은폐 분석
====================================
공중 관측으로부터 보호되는 지역을 식생특성에 따라 분류하여 은폐정도를 표출
  - 기본 원리: 식생도 조건에 의한 분류
  - 상세 원리: 식생도(산림): 양호/보통/불량 구분 공중 관측으로부터 보호되는 지역을 식생특성에 따라 분류하여 은폐정도 표출


**Syntax**

Concealment(SimpleFeatureCollection forestFeatures, Filter goodFilter, Filter normalFilter, Filter poorFilter, Geometry maskArea): SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 식생도(산림) 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - goodFilter
     - 은폐가 양호한 식생도의 조건식입니다.
     - Filter
     -
     - ✓

   * - normalFilter
     - 은폐가 보통인 식생도의 조건식입니다.
     - Filter
     -
     - ✓

   * - poorFilter
     - 은폐가 불량한 식생도의 조건식입니다.
     - Filter
     -
     - ✓

   * - maskArea
     - 분석 영역 폴리곤 지오메트리입니다. 최대 분석 범위는 10km * 10km를 넘을 수 없습니다.
     - Geometry
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
     - 분석 결과입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - maskArea의 최대 분석 범위는 10km * 10km를 넘을 수 없습니다.
