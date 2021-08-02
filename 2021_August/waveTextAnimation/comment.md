# CSS Text Wave

### What I Learn

간단한 애니메이션 트릭의 구현
조금 더 편하게 생각하면 금방 구현할 수 있을텐데 아쉽다.

1. 같은 Water라는 글자 4개를 겹친다는 생각을 못했다.
   뒤에 다른 컴포넌트를 붙여서 한다고 생각했는데 그럴 필요없이 n-thChild만 잘 써도 가능했다.

2. clip-path maker라는 좋은 사이트가 있다. 이미지를 특정하게 자르거나 할 때 clip-path랑 같이 쓰기 아주 좋다고 생각된다.
   이번에는 파도를 조금 투박하게 만들었는데 실제 쓸 때는 20각형 이상으로 나눠서 하면 편하게 구현이 가능할 듯 하다.

### Improvement

- Clip-path 함수랑 prettier랑 묶이면 되게 이상하게 나온다
- Shadow도 마찬가지. 이건 나중에 Prittier 설정해서 변경해주면 될 것 같다.

### Reference

https://www.youtube.com/watch?v=G4CRBvx-pac&ab_channel=OnlineTutorials
