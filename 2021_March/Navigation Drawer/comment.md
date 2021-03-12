# Navigation Drawer

### What I Learn

### Improvement

아쉬운 점 :

1. 이 튜토리얼의 대부분이 absolute, relative 기반으로 이루어져 있어서 다양한 사이즈에 대한
   responsive한 반응을 보기가 어려움.

flex 구조를 이용하고
중앙 정렬은 margin을 이용했어도 괜찮았을 것 같은데

```
display: block
margin: auto
```

Flex 구조에서 글자 가리는 경우에는 조금 고민
글자가 줄어드는 걸 애니메이션으로 추가해서 보여줄 수 없었을까 싶다가도
글자가 점점 fade-out되게 해도 괜찮을거 같아보임

지금 구조는 글자 되게 잘 가려주는듯함.

2. Font-awesome에 너무 의존적인듯 함.

대부분의 경우 .svg를 쓰는 것과 거의 같아서 크게 무리는 없지만
여기서 css를 부를 때 fontAwesome을 쓰는게 아쉬움.

```
.toggle.active::before {
  content: "\f053";
  font-family: fontAwesome;
  position: absolute;

```

차라리 svg를 부르고 active일때 아닐 때 회전시키는 형식이 조금 더 아름답지 않았을까 싶음
갑자기 방향 바뀌는 것도 약간 아쉬웠음
