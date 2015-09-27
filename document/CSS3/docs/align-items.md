# align-items

작성자 : 송지은

작성일 : 2015-09-27

css 레퍼런스 설명: 
- align-items : flex로 지정된 부모 요소 내에서 기본 정렬을 지정하는 속성이다.
- 속성 값 : stretch, center, flex-start, flex-end, baseline, initial, inherit

`sample code` : 

```html
<!DOCTYPE html>
<html>
<head>
<style>
#main {
    width: 220px;
    height: 300px;
    border: 1px solid black; 
    display: -webkit-flex; /* Safari */
    -webkit-align-items: center; /* Safari 7.0+ */
    display: flex;
    align-items: center;
}

#main div {
   -webkit-flex: 1; /* Safari 6.1+ */
   flex: 1;
}
</style>
</head>
<body>
<div id="main">
  <div style="background-color:coral;">RED</div>
  <div style="background-color:lightblue;">BLUE</div>  
  <div style="background-color:lightgreen;">Green div with more content.</div>
</div>
</body>
</html>
```

[결과보기](http://www.w3schools.com/cssref/tryit.asp?filename=trycss3_align-items)


참고 : 
- 인터넷 익스플로러 10 및 이하 버전에서는 align-content 속성을 지원하지 않는다.
- 사파리 7.0 및 최신 버전에서는 -webkit-align-content 속성을 지원한다.