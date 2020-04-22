# 5장
## PShape 예제

```

PShape star; // pshape 별 모양 만들기

void setup() {
  size(640,360); // 화면 가로 세로 크기
  star = createShape(); // 별모양 만들기
  star.beginShape(); 
  star.endShape(CLOSE); 
}
void draw() {
  background(40,250,196); // 배경은 밝은 연두색
  translate(mouseX, mouseY); // 원점을 마우스로 이동
  fill(255,0,0); //빨간색 별
  stroke(255); // 흰색 선
  strokeWeight(7); //선의 굵기 7
  beginShape(); // 점의 기록 시작
  vertex(0, -50); //
  vertex(14, -20);
  vertex(47, -15);
  vertex(23, 7);
  vertex(29, 40);
  vertex(0, 25);
  vertex(-29, 40);
  vertex(-23, 7);
  vertex(-47, -15);
  vertex(-14, -20);
  endShape(CLOSE); // 점의 기록 중지
}

```
