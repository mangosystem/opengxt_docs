.. _selectfeatures:

공간 및 속성 조건으로 피처 추출
======================================================

공간 및 속성 필터와 속성 필드값을 선택하여 피처를 추출합니다.

**Syntax**

SelectFeatures (SimpleFeatureCollection inputFeatures, Filter filter, String attributes) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 추출할 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - filter
     - 공간 및 속성 조건의 필터 표현식입니다.
     - Filter
     -
     - ✓

   * - attributes
     - 추출에 사용될 쉼표로 구분된 속성 필드 목록을 설정합니다.
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
     - 추출한 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - 필터를 사용하여 특정 조건에 맞는 피처만 선택할 수 있다.
 - 콤마로 분리된 필드를 설정하여 일부 속성정보만 선택하거나 필드 순서를 변경할 수 있다.


**Examples**

서울시 읍면동 경계 데이터에서 강남구만 선택하고 geom, sgg_nm, emd_cd, emd_nm 필드만 추출한 결과입니다.

  .. image:: images/selectfeatures.png
