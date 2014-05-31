### 테이블 조작하기

이 책을 보고 있다면 이미 d3js로 그려진 화려한 시각화 결과물들을 본 적이 있을 것이다. 분명히 d3js는 그러한 화려한 시각화 작업을 할 수 있는 강력한 라이브러리이지만 이 책에서는 표를 다루는 데서 이야기를 시작할 것이다. 다시 한 번 강조하지만 d3js의 주역은 데이터이다. 얼핏 보기에 표와 화려한 시각화 사이에는 메꿀 수 없는 갭이 있는 것처럼 보일지도 모르지만, 두 표현 양식은 모두 데이터에 기반하고 있다. 거꾸로 이야기하는 것이 좀 더 정확할 것이다. 우리가 데이터를 가지고 있다면, 이 데이터를 표 형식으로 표현할 수도 있고, 막대 그래프나 파이 차트로 표현할 수도 있고, 좀 더 복잡한 독자적인 시각화 로직을 사용해서 보여줄 수도 있다. 물론 각 표현양식을 사용하고자 할 때 필요한 데이터 형식도 다르고 잘 표현해낼 수 있는 특성 역시 다르다. 하지만 데이터에서 출발한다는 것은 다르지 않으며, 표는 그 중에서 가장 간단한 표현 양식일 뿐이지, 본질은 다르지 않다.

###

앞 절에서는 데이터를 HTML 요소에 연결하는 방법에 대해서 살펴보았다. 여기서도 같은 방법으로 데이터를 HTML의 표에 연결할 것이다. 먼저 아래와 같이 2013년 프로야구 전적 데이터를 다뤄보자.

```
# baseball_2013.csv

순위,구단,경기수,승,무,패,승차,연승-연패,승률
1,삼성,128,75,2,51,-,-1,0.595
2,LG,128,74,0,54,2,2,0.578
3,넥센,128,72,2,54,3,-1,0.571
4,두산,128,71,3,54,3.5,-1,0.568
5,롯데,128,66,4,58,8,2,0.532
6,SK,128,62,3,63,12.5,-2,0.496
7,NC,128,52,4,72,22,1,0.419
8,KIA,128,51,3,74,23.5,-3,0.408
9,한화,128,42,1,85,33.5,-1,0.331
```



```
d3.csv("baseball_2013.csv", function(data) {
    console.log(data);
});
```

### Data and elements : .enter(), .exit()



### run & test