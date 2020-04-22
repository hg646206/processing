# 3장
## processing example translate() 함수를 사용한 예제

```

float x, y; // 실수 변수 선언
float dim = 160.0; // 삼각형의 크기

void setup() {
  size(1000, 325); // 화면 가로 세로 크기
  noStroke(); // 선 없음
}

void draw() {
  background(0); // 배경 없음
  
  x = x + 2; // x보다 +2 빠르게 간다
  
  if (x > width + dim) { // x의 값이 폭+dim의 값을 넘어서면 다시 시작한다
    x = -dim;
  } 
  
  translate(x, height/1-dim/1); //원점을 x,height/1-dim/1로 이동
  fill(255,0,0); // 빨간색 원
  ellipse(-dim/2, -dim/2, dim, dim); //원의 값은 dim
  translate(x, dim); // 원점을 x,dim으로 이동
  fill(0,0,255); // 파란색 원
  ellipse(-dim/2, -dim/2, dim, dim); // 원의 값은 dim
}

```
