# Data Driven Document(d3 공동집필)

## 1. 정보 시각화와 d3

이 장에서는 정보시각화와 d3가 무엇인지 소개합니다. 우선은 간단히 정보시각화의 역사와 역할에 대해서 살펴봅니다. 다음으로 시각화 작업이 어떤 과정을 통해서 만들어지는 지 살펴보고 프로그래밍으로 어떻게 시각화를 구현하는 지에 대해서 다룹니다. 다음으로 이 책에서 정보시각화 작업에 사용할 d3 라이브러리를 소개하고 실제 사용 예제를 보여주고, 비슷한 라이브러리들에 대한 비교합니다.

### 1.1 정보 시각화(Information visualization)란?

#### 1.1.1 정보시각화란?
- 짧게 보는 시각화의 역사
- 탐색적 분석
- 의사결정
- 스토리텔링
- 데이터 분석가와 프로그래머와 디자이너

### 1.1.2 과정
- 데이터(Acquire, Parse)
- 분석(Filter, Mine)
- 시각화(Filter, Mine, Represent, Refine)
- Interaction

### 1.1.3 시각화와 프로그래밍
- 인포그래픽
- 추상화된 데이터
- 추상화된 그래프
- 인포그래픽과 시각화
- 웹

### 1.2 Data Driven Document(d3)

#### 1.2.1 Data Driven Document란?
- 개요
- 데이터와 시각화

#### 1.2.2 d3 활용예제
- 뉴욕 타임즈

#### 1.2.3 d3와 유사한 라이브러리


## 2. d3 개발 환경의 이해 및 구축

이 장에서 복격적으로 d3 프로그래밍을 시작하기에 앞서 d3를 둘러싸고 있는 기술들에 대해 소개하고, 프로그래밍 작업을 하기 위한 개발 환경 구축 방법에 대해서 다룹니다. 위의 내용들을 전제로 간단한 테이블 조작 다룹니다. 이는 시각화에 앞어서 d3가 데이터와 어떻게 소통하는 지 보여주고 Data Driven Document의 본질적인 의미를 맛배기로 보여줄 것입니다.

### 2.1 d3에서 사용하는 기술들
- WEB
- HTML
- DOM
- Javascript 
- CSS
- SVG

### 2.2 개발 환경
- 텍스트 에디터
  - Sublime
- 브라우저
  - 모던 브라우저(d3에서 지원하는 브라우저)
  - 브라우저 개발자 도구
  - d3에서 지원하지 않는 브라우저
- d3 설치하기
  - CDN 이용하기
  - 공식 사이트에서 다운로드 받기
  - 개발 버전 사용하기
  
### 2.3 간단한 예제
- Data Driven Document의 의미
- 데이터를 HTML 요소에 맵핑하기
- 테이블 조작하기
- Data and elements : .enter(), .exit()
- run & test

## 3. 간단한 그래프 프로그래밍으로 시작하는 시각화

이부분은 최종적으로 더 많은 정리가 필요할 것 같습니다.

제 3장에서는 2장에서 다룬 테이블 조작에 이어서 이러한 데이터가 어떻게 그래프로 만들어지는지 (데이터 수집 단계를 제외한) 과정 하나하나를 자세히 다룹니다. 여기서 만들 그래프는 엑셀로도 금방 만들 수 있는 매우 간단한 막대 그래프입니다. 이 장은 시각화 과정에 대한 이해 및 시각화를 하는 사람, 여기서는 프로그래머가 이해하고 있어야할 지식들에 대해 다룹니다. 특히 데이터와 시각적 요소의 맵핑을 중점적으로 다루며 이러한 과정에서 사용하는 요소와 변환 기법들, 그리고 스케일이라는 개념을 다룹니다. 종합적인 관점에서 복잡한 시각화도 결국에는 이러한 작은 요소들에서 출발한다는 것을 보여줍니다.

### 3.1 d3와 시각화 과정
- 시각화 과정에서 d3의 역할

### 3.2 데이터와 시각적 요소의 맵핑
- 2차원 그래프 / 3차원 그래프
- 그래프의 차원 축소
- interaction을 통한 차원 축소

### 3.3 d3 레이아웃
-  같은 데이터로 다른 그래프 그리기

### 3.4 스케일
- 데이터 변환
- 컬러 스케일

### 3.5 축
- ...

## 4. 여러가지 그래프 그리기

제 4장에서는 3장에서 프로그래밍한 막대 그래프에서 출발해 비슷하거나 일반적으로 익숙한 그래프들을 소개합니다. 특히 3장과 4장에서는 비슷한 데이터를 사용하고 레이아웃을 변경함으로써 데이터와 그래프 형태(구체적으로는 그래프 형식를 구성하는 시각적 요소들)가 어떻게 구성되어있는 지를 좀 더 명확히 보여줍니다. 이를 통해서 각각의 그래프 형식이 어떤 시각적 요소들로 구성되어있는 지를 명확한 보여주고 나아가서 더 복잡한 그래프를 그릴 수 있는 기반을 다집니다.

### 4.1 Bar
### 4.2 Line
### 4.3 Pie
### 4.4 Donut
### 4.5 Stacked

## 5. d3 깊이 살펴보기

제 5장에서는 본격적으로 d3 라이브러리 자체에 대해서 다룹니다. 특히 시각화를 위해 데이터를 어떻게 가져오는가 하는 부분을 다루고 d3의 핵심 기술들인 SVG와 CSS에 대해서 다룹니다. 다음으로는 d3 API를 각 파트에서 중요한 개념들을 뽑아 라이브러리에 대해서 자세히 풀어나갑니다.

### 5.1 데이터 다루기
- 데이터 가져오기
- 데이터 조작하기
- 데이터 변환

### 5.2 SVG의 이해
- Elements

### 5.3 CSS
- Styles

### 5.4 d3
- 요소선택자(d3.selections)
- 레이아웃(d3.layouts)
- 에니메이션(d3.transitions)
- 스케일(d3.scales)
- 시간(d3.times)
- 인터렉션
- 이벤트

## 6. d3를 활용한 데이터 시각화

제 6장에서는 5장까지 배운 내용들을 모두 활용해 좀 더 복잡한 시각화를 프로그래밍으로 구현해봅니다. 각 챕터마다 하나의 시각화를 다룹니다.

### 6.1 Bubble Chart 활용한 예제
### 6.2 Sunburst
### 6.3 Nested Pie Chart
### 6.4 Heatmap
### 6.5 지도 활용한 예제
### 6.6 인터렉션 화려한 예제
### 6.7 에니메이션이 화려한 예제

## 7. 심화 주제

이번 장에서는 시각화 개념이나 d3의 시각화 구조보다는 다른 방향에서 깊은 주제를 다룹니다. 시각화를 위한 데이터 파싱, 소켓.io를 통한 실시간 데이터 주고받기, 부트스트랩을 통한 스타일링, nodejs를 활용한 시각화 이미지 생성, 그리고 좀 더 구조화된 시각화를 위해 angularJs 디렉티브를 시각화에 활용하는 법을 다룹니다.

### 7.1 데이터 파싱
### 7.2 socket.io + d3 => 실시간 대시보드
### 7.3 Bootstrap과 함께 사용하기
### 7.4 d3 시각화 이미지 파일(혹은 다른 형식)로 생성하기
### 7.5 Angular.js directive와 함께 사용하기
### 7.6 모던 Javascript 개발 도구

## 8. d3와 함께 사용가능한 라이브러리

제 8장에서는 앞에서 다루지 못 했던 자잘한 이야기들과 d3와 함께 활용할 수 있는 시각화와 관련된 라이브러리들을 소개합니다.

### nvd3
### dc.js

## 부록
### 관련 정보 사이트
