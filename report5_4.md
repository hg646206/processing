# 4장
## Processing Tutorials Getting Started 예제

```

void setup() {
  size(600,600); // 화면 가로 세로 크기
}

void draw() {
  if (mousePressed) { //마우스를 클릭하면
    fill(255,214,3); // 노란색
    noStroke(); // 테투리가 없음
  } else { //마우스를 클릭 하지 않으면
    fill(0); // 검은색
  }
  rect(mouseX, mouseY, 80, 80); // 80,80 사이즈의 사각형이 마우스를 따라 움직임
}

```
