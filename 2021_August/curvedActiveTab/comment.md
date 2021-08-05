# CSS Text Wave

배운게 많은 내용

이건 따로 시간내서 다시 안 보고 만들 수 있으면 좋을듯하다
물론 만들기 전에 최초 상태의 html (list랑 Icon만 추가해둔)을 가지고 만들면 좋을 듯

주말에 해보기 좋을 것 같다

### What I Learn

HTML CSS JS를 모두 활용한 Active tab 만들기!

1. <b> 태그를 이용해서 위 아래로 덮어쓰기 할 때 background:#fff를 설정하고 border-radius를 설정했는데
   왜 다른 li의 배경이랑 충돌이 안나는거지? 파란색으로 나올거 같은데 흰색이 잘 나오네?
   더 깊은 레벨의 엘리먼트가 더 우선적용 되는건가?
   -> 테스트를 해보자 <div><div>... 하면서 백그라운드 설정하고
   아 적다 보니까 그렇네!
   안쪽에 있는게 우선 적용되겠지 그치 파란색 위에 흰색을 덮어서 다른 배경이랑 위화감 없이 됐던거였다!

2. 임의의 태그 (여기서는 <b>)를 이용해서 위 아래에 border-radius를 설정해서 굽은 형태를 만들어 낼 줄은 몰랐다.
   되게 괜찮은 css 트릭인듯하다.
   다만 돔이 불필요하게 많아지는건 아닌가 싶다
   조금 더 활용하면 dom을 필요할 때만 추가하는 방식은 어떨까?
   뭐가 더 실용성이 높은지는 잘 모르겠다

3. transition이 css property에 따라서 앞에 붙여주는게 다르구나
   transition: width 2s,
   transition: height 2s 처럼 내가 적용하고 싶은 속성에 대해서만 할 수 있음!

### Improvement

-

### Reference

https://www.youtube.com/watch?v=P_A2kNpyQBs&ab_channel=OnlineTutorials
https://developer.mozilla.org/ko/docs/Web/CSS/CSS_Transitions/Using_CSS_transitions
