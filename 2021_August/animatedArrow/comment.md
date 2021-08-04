# CSS Text Wave

### What I Learn

JS 기반의 애니메이션 트릭의 구현

막힐만한 부분은 애니메이션 계산 로직

함수 레벨로 잘 잘려있어서 이해하기 쉽게 코드가 깔끔해서 좋았다.

1. cursor: url(), pointer 에서 이미지의 사이즈는 최대 128px를 넘길 수 없다.

2. arrow 배치를 랜덤하게 하고 사이즈도 랜덤하게 함수 하나로 처리 가능한데 이걸 어떻게 구현해야 할 지 고민하고 있었다.
   이건 간단하게 할 수 있는 내용인데 아직 미숙한 것 같음.
   반성반성

3. 아래는 알자!

- getBoundingClientRect() : ViewPort 기준으로 window내에서 오브젝트의 위치를 파악할 수 있다.
- offset~~ : 부모요소의 시작 지점을 기준으로 오브젝트의 위치를 알 수 있다.

- offsetWidth : margin을 제외한 padding, border까지 계산한 값
- clientWidth : margin, border가 제외된 padding까지의 값만 적용한 내부의 크기
- scrollWidth : scroll 영역에서 스크롤로 감싸진 내용의 전체 크기 (스크롤까지 포함한 값)

이렇게 때문에 getBoundingClientRect + offset/2 를 하면 정확히 중점의 위치를 알 수 있다.

- screenX : 모니터 기준 X좌표
- pageX : 내가 보는 전체 문서 기준 X좌표 (이 경우는 스크롤로 화면 밖으로 나간 범위를 포함한다)
- clientX : 브라우저에서 웹페이지가 보여지는 영역 기준
- offsetX : 이벤트가 걸려있는 돔 엘리먼트 기준. 특정 DIV 내부에서 하는 경우 좌상단 모서리는 (0,0)이 될 것

- atan과 atan2는 두 점의 상대적 위치를 파라미터로 받음.
  대신 atan2는 음수 변수의 입력도 받을 수 있고 결과를 pi ~ -pi까지 표현 범위가 더 넓음

### Improvement

- randomSize 함수가 불필요한 매개변수를 받아서 삭제했다.

### Reference

https://www.youtube.com/watch?v=4IwcqHazkfY&ab_channel=OnlineTutorials
https://hianna.tistory.com/493
