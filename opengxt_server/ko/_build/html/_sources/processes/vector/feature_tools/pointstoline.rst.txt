.. _pointstoline:

포인트를 라인으로 변환
====================================

포인트의 정렬 필드값을 이용하여 속성이 같은 필드값별로 라인을 생성합니다.

**Syntax**

PointsToLine (SimpleFeatureCollection inputFeatures, String lineField, String sortField, Boolean useBezierCurve, Boolean closeLine, Boolean geodesicLine) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 라인을 생성할 포인트 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - lineField
     - 라인 그룹 필드를 설정하면 그룹별로 각각의 라인을 생성할 수 있습니다.
     - String
     -
     -

   * - sortField
     - 기본값으로 저장된 포인트의 순서대로 라인을 생성합니다. 만약 정해진 정렬 필드가 있다면 이를 설정할 수 있습니다.
     - String
     -
     -

   * - useBezierCurve
     - 선을 생성할 때 베이지어 커브를 사용할 지 여부를 설정합니다.
     - Boolean
     - false
     -

   * - closeLine
     - 생성된 라인의 폐합 여부를 설정합니다.
     - Boolean
     - false
     -

   * - geodesicLine
     - 출력 라인 생성 시 측지선을 사용할 지 여부를 설정합니다. 지리좌표계만 지원합니다.
     - Boolean
     - false
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
     - 입력 포인트로부터 라인을 생성한 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - lineField 파라미터를 설정하면 lineField의 고유값에 따른 각각의 라인을 생성한다.
 - sortField 파라미터를 설정하면 sortField로 정렬한 포인트를 이용하여 라인을 생성한다.
 - closeLine 파라미터가 True인 경우 시작점과 끝점을 연결하여 폴리곤을 생성한다.


**Examples**
