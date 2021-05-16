# CSS Animation Effects

### What I Learn

공부할게 이번에 많다!
오랜만에 애니메이션 되게 흥미로웠다

막상 도로 흰색 점선 어떻게 표현할지 생각했었는데
background-size를 조정하고 repeat하면서 생각보다 더 쉽게 구현이 가능했음.

1. 애니메이션에 대해서 공부할게 되게 많구나 (특히 3D 표현은 거의 본 적이 없어서 관련 property들은 이번이 찾아보는게 처음)

2. transform-origin, transform-style, transform: perspective() 는 이번이 처음 보는 함수들

- transform-origin : 말 그대로 transform을 할 때 어디를 기준으로 transform을 실행할지에 대해서 결정
  예를 들어 이번 .square의 경우 transform-origin: bottom right; 이기 때문에 우측 하단 꼭짓점을 기준으로 rotate를 실행할 수 있었음.

- transform-style : .infinite에서 쓰인 스타일. 3D공간에 배치할지 말지를 결정할 수 있음

이 세팅을 바탕으로 road가 어떻게 기울어질지 정할 수 있음

perspective로 보는 관점을, rotateX를 통해서 얼마나 rotate시킬지를 정함.

transform-style: flat인 경우 3D화면에서 2D 평면 운동을 할 수 있음.

- transform: perspective() :

// 아래 Reference에서 인용

여기서 말하는 숫자는 Z축을 기준으로 관찰자가 요소로 부터 얼마나 떨어져서 관찰하는가를 명시하는 숫자
간략하게 설명하면 숫자가 커질수록 멀리 떨어져서 보이게 된다는 것
기본적으로 멀리 떨어져 있어야 하는 사물은 작게 만들고 가까운 곳에 있어야 하는 사물은 크게 만들어서 원근감을 부여하는 것으로 이해해도 무방

- 내가 z축 방향으로 멀어지니까 rotateZ가 안 되는것처럼 보이는듯.
- perspective가 작을수록 가까워지니 다른 rotate의 효과가 더 커져서 보임.

3. -webkit-box-reflect 는 참고 정도로만 보면 될듯

### Improvement

### Reference

https://grace-go.tistory.com/49
https://developer.mozilla.org/en-US/docs/Web/CSS/transform-style
https://poiemaweb.com/css3-transform
https://ossam5.tistory.com/85
