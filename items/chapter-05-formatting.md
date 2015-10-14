# 5장. 형식 맞추기

코드가 어수선해 보인다면 독자들은 프로젝트의 다른 측면도 똑같이 무성의한 태도로 처리했으리라 생각할 것이다.

## 형식을 맞추는 목적

코드 형식은 의사소통의 일환이다.

원래 코드는 사라질지라도 개발자의 스타일과 규율은 사라지지 않는다

## 세로 형식 맞추기

일반적으로 작은 파일이 이해하기 쉽다.

- 작은 파일들로도 커다란 시스템을 구축할 수 있다.

신문 기사처럼 작성하라

- 이름은 간단하면서도 설명이 가능하게 짓는다.
- 첫 부분은 고차원 개념과 알고리즘을 설명한다.
- 아래로 내려갈수록 의도를 세세하게 묘사한다.

개념은 빈 행으로 분리하라

세로 밀집도

- 세로 밀집도는 연관성을 의미한다.

수직 거리

- 타당한 근거가 없다면 서로 밀접한 개념은 한 파일에 속해야 마땅하다. (protected 변수를 피해야 하는 이유 중 하나)
- 같은 파일에 속할 정도로 밀접한 두 개념은 세로 거리로 연관성을 표현한다.
- 변수는 사용하는 위치에 최대한 가까이 선언한다. 루프를 제어하는 변수는 흔히 루프 문 내부에 선언한다.
- 인스턴스 변수는 클래스 맨 처음에 선언한다.
- 한 함수가 다른 함수를 호출한다면 두 함수는 세로로 가까이 배치한다. 또한 가능하다면 호출하는 함수를 호출되는 함수보다 먼저 배치한다.
- 개념적으로 유사한 코드는 가까이 배치한다.
    - 함수 호출 관계
    - 변수와 그 변수를 사용하는 함수
    - 비슷한 동작을 수행하는 일군의 함수

세로 순서

- 일반적으로 함수 호출 종속성은 아래 방향으로 유지한다.

## 가로 형식 맞추기

프로그래머는 명백하게 짧은 행을 선호한다.

- 개인적으로는 120자 정도로 행 길이를 제한한다.

가로 공백과 밀집도

- 공백을 사용해 밀접한 개념과 느슨한 개념을 표현한다.
- 할당문, 함수와 인수, (우선순위,) ...

가로 정렬

- 유용하지 않음.
- 가로 정렬이 필요할 정도라면 클래스가 너무 큰 것일 수 있음.

들여쓰기

- 프로그래머는 들여쓰기 체계에 크게 의존한다.
- 들여쓰기를 무시하고픈 유혹에 빠지지 마라.

가짜 범위

- 빈 while/for 문 등은 좋은 것은 아니지만 불가피하게 사용할 경우, 반드시 빈 블록을 올바로 들여쓰기 하여 작성한다.

## 팀 규칙

팀은 한 가지 규칙에 합의해야 한다. 그리고 모든 팀원은 그 규칙을 따라야 한다. 그래야 소프트웨어가 일관적인 스타일을 보인다.

한 소스 파일에서 봤던 형식이 다른 소스 파일에도 쓰이리라는 신뢰감을 독자에게 줘야 한다.