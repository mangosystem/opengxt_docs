.. _ringmap:

Ring Map 생성
=================================

시계열 속성값 등 피처의 여러 필드를 이용하여 Ring Map을 생성합니다.

**Syntax**

RingMap (SimpleFeatureCollection inputFeatures, String fields, String targetField, Integer ringGap) : SimpleFeatureCollection, SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 포인트, 라인, 폴리곤 등 시계열 속성을 가진 입력 레이어 입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - fields
     - 쉼표로 구분된 필드 목록 또는 링 개수입니다.
     - String
     -
     - ✓

   * - targetField
     - 링의 값이 저장될 대상 필드입니다.
     - String
     - ring_val
     -

   * - ringGap
     - 링 사이의 간격입니다.
     - Integer
     - 1
     -

**Process Outputs**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - anchor
     - 원본 레이어와 Ring Map을 연결하는 지시선 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - ringmap
     - 출력 Ring Map 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - fields 파라미터는 콤마로 분리된 연도별 시계열 필드와 같은 연속적인 필드 또는 Ring의 개수를 사용한다.
 - targetField가 Null인 경우 ring_val 필드가 기본값이다.
 - ringGap 파라미터는 1 ~ 9까지 가능하며 1이 기본값이다.
 - Output은 지시선을 표시하는 anchor 라인과 Ring Map을 생성한 ringmap 폴리곤 2개의 레이어를 반환한다.

**Examples**

서울시의 2000년부터 2005년까지의 인구자연증가율 속성을 이용하여 Ring Map을 생성한 결과입니다.

  .. image:: images/ringmap.png
