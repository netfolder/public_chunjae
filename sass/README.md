### [ < 홈으로](https://github.com/netfolder/public_chunjae)

## sass 문법

* 셀렉터 네스팅

: 특정 선택자 내에는 속성 정의만 들어오는 것이 아니라, nested된 속성 정의 블럭이 들어올 수 있다.

```
.entry-content {
  p { font-size: 9.814rem; }
}

// compiled to
.entry-content p {
  font-size: 9.814rem;
}
```

* 속성 네스팅

: font의 경우 font-family, font-size, font-weight 등이 주로 세트로 정의되는데, 
다음과 같이 하나의 세트(?)인 속성들은 속성의 하위 사전 형태로 작성할 수 있다.

```
.entry-content {
  p {
    font: {
      family: "Noto Serif CJK KR", serif;
      size: 9.814rem;
      weight: 400;
    }
  }
}

```

* 상위요소 참조

: &을 사용하면 블럭이 적용되는 셀렉터를 치환한다.

```
a {
  text-decoration: none
  &:hover { text-decroation: underline; }
}
// compiled to
a { text-decoration: none; }
a:hover { text-decoratino: underline; }

```
```
.widget {
   font-weight: 400;
   &-area { font-weight: 600; }
   &-top_posts { font-weight: 1000; }
}
// compiled to
.widget { font-weight: 400; }
.widget-area { font-weight: 600; }
.widget-top_posts { font-weight: 1000; }
```