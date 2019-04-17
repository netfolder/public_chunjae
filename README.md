
# public_chunjae
지속성있는 내용 유지공간


## CSS
- reset.css[(보기)](https://github.com/netfolder/study/blob/master/menu_content/submenu/css/default.css)
- Airbnb CSS / Sass Styleguide 방법론[(보기)](https://github.com/airbnb/css#oocss-and-bem)

|:---|:---:|---:|
| 순서 | 속성 | 의미 |
|1	|display	|표시
|2	|overflow	|넘침
|3	|float	|흐름
|4	|position	|위치
|5	|z-index	|정렬
|6	|width & height	|크기
|7	|margin & padding	|간격
|8	|border	|보더
|9	|font	|폰트
|10	|background	|배경
|11	|etc(기타)	|color,text-decoration,text-indent,clear...


## Sample

- bxSlider[(보기)](https://github.com/netfolder/public_chunjae/tree/master/bxSlider)
	+ [(git)](https://github.com/stevenwanderski/bxslider-4)

- slick[(보기)](https://github.com/netfolder/public_chunjae/tree/master/slick)
	+ [(git)](https://github.com/kenwheeler/slick)
 
## Comment
```
/*common*/ (x)
/* common */ (o)  CSS 주석 기호( /*, */ )와 내용 사이에는 반드시 공백 한 칸이 있어야 한다.

/* 20190401 GNB 수정 시작 */
.gnb_comm {overflow:hidden;width:978px;clear:both}
.gnb_comm li {float:left;height:38px}
.gnb_comm .menu {display:block;overflow:hidden;height:38px}
.gnb_comm .home {width:79px}
.gnb_comm .roadmap {width:98px}
.gnb_comm .on .menu {margin:0 -1px}
/* 20190401 GNB 수정 끝 */
```