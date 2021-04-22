# Navigation Drawer

### What I Learn

### Improvement

아쉬운 점 :

1. 처음 로딩 시 말풍선 모양을 만들기 위해 사용한 ::before가 실제 말풍선보다 앞에서 나옴.

부자연스러운 사각형 2개가 처음 로딩될 때 보임.
해결해주기 위해서 ::before에 z-index를 주어 실제 말풍선 글자가 위치할 부분보다 뒤로 보냄.

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
