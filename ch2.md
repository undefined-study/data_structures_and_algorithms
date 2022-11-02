# 알고리즘이 중요한 까닭

사용할 알고리즘을 적절하게 선택해야 코드의 효율성에 중요한 영향을 미친다.

컴퓨팅 관점에서 알고리즘은 특정 과제를 달성하기 위해 컴퓨터에 제공되는 명령어 집함을 뜻한다.

## 정렬된 배열에 값을 삽입하는 예시
항상 실제 삽입 전에 검색을 먼저 수행해서 삽입할 올바른 위치를 정해야 함을 알 수 있다.
이것이 전형적인 배열과 정렬된 배열의 성능 차이 중 하나이다.

 ex) 정렬된 배열 [1,3,5,7]에 6 이라는 값을 넣는다고 치면 인덱스0부터 값을 확인하며 
 값 1, 3, 5를 확인하고 맞는 자리를 찾으면 7을 옆으로 옮기고 6을 넣는다. 
 그러므로 단계 수는 1,3,5 값 확인 3단계, 값 7 오른쪽으로 이동 1단계 총 4단계가 걸린다.

정렬된 원소가 N개이면 N + 2단계라고 할 수 있다.

만약 정렬된 배열에 새로운 값이 가장 마지막에 들어가게 된다면 기존 N값 모두 비교 + 1단계 삽입 단계가 걸리므로 N + 1단계이다.

이 검색 방법을 선형검색이라고 한다.


## 이진 검색 방법

### ex) 정렬된 배열에서 이진 검색 방법

- 배열 중 가운데 셀에 접근하여 값을 확인한다.
- 만일 찾으려는 값보다 크다면 왼쪽의 셀들을 검색, 크다면 반대 셀들을 검색한다.
- 다시 또 반으로 나눠서 값을 확인한다.
- 반복하여 값을 찾는다.

이진 검색은 정렬된 배열에서만 쓸수 있고 이것은 정렬된 배열의 장점 중 하나이다.


## 선형검색과 이진검색 비교
먼저 100개의 값을 갖는 배열에서 각 검색에 필요한 단계 수는 다음과 같다 
- 선형검색: 100단계
- 이진검색: 7단계

선형검색은 모든 원소를 다 확인해야 되므로 100단계 이고,

이진검색은 절반씩 잘라나가므로 7단계가 된다.

##마무리

모든 상황에 완벽한 단 하나의 자료구조나 알고리즘은 없다..
