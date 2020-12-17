.. _verticestopoints:

버텍스를 포인트로 변환
====================================

라인, 폴리곤 피처의 버텍스(모두, 시작점, 종점, 중점 등)를 포인트로 변환합니다.

**Syntax**

VerticesToPoints (SimpleFeatureCollection inputFeatures, PointLocationType location) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 라인 또는 폴리곤 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - location
     - 출력 포인트의 유형을 설정합니다. All(기본값), Mid, Start, End, BothEnds
     - PointLocationType
     - All
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
     - 출력 포인트 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - location: All(기본값), Mid, Start, End, BothEnds
 - inputFeatures 파라미터는 라인 또는 폴리곤 레이어 이어야 한다.
 - location 파라미터는 다음과 같이 5개의 옵션을 사용할 수 있다.

 .. list-table::
    :widths: 20 60

    * - **옵션**
      - **설명**

    * - All
      - 라인 또는 폴리곤 지오메트리의 모든 버텍스, 기본값

    * - Mid
      - 라인 또는 폴리곤 지오메트리의 중간점

    * - Start
      - 라인 또는 폴리곤 지오메트리의 시작점

    * - End
      - 라인 또는 폴리곤 지오메트리의 끝점

    * - BothEnds
      - 라인 도는 폴리곤 지오메트리의 시작점과 끝점

**Examples**

라인 피처의 Mid(중간점)을 포인트로 변환한 결과입니다.

  .. image:: images/verticestopoints.png
