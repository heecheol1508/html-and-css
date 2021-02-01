### 김버그의 HTML&CSS는 재밌다

2021-02-01



**문서의 구조와 정보 위계가 명확하게 보이는 HTML 코드를 작성해야 함.**

(Semantic Markup)



### Anchor tag

```html
<a href="http:naver.com">네이버</a>
<a href="mailto:qwer@gmail.com">qwer@gmail.com에게 이메일 보내기</a>
<a href="tel:01012345678">010-1234-5678로 전화걸기</a>
<a href="#chap8">아이디 chap8으로 이동하기</a>

<a href="http:naver.com" target="_blank">새탭으로 네이버</a>
```



### Image

```html
<img src="#" alt="" />
```

alternative text : 로딩 또는 음성으로 이미지를 확인할 때를 위해 필요



### List

```html
<ol>
    <!-- ordered list -->
    <li>list item</li>
    <li>list item</li>
</ol>

<ul>
    <!-- unordered list list -->
    <li>list item</li>
</ul>
```

**ul**과 **ol**의 자식요소는 무조건 **li**만 가능



### Description List (정의리스트)

- 용어를 정의할 때, key-value로 정보를 제공할 때 주로 사용
- dl의 자식요소로 dt, dd, div만 가능

`<dl>` description list

`<dt>` description term - key

`<dd>` description data - value

`<dfn>` 



### Quotations 인용

```html
<blockquote cite="https://bit.ly/2mvSYrT">
    <p>
        The study is the first to project the long-term outlook for Antarctica's largest penguins, which can grow 1.2 meters (four ft) tall, seeking to fill a gap in understanding climate change and wildlife in one of the remotest parts of the planet.
    </p>
    <p>
        Overall, numbers were set to fall by at least 19 percent from current levels by 2100 as sea ice melts. And two-thirds of colonies of the birds, which have distinctive golden head patches, would decline by more than half, it said.
        <q>It's not happy news for the emperor penguin,</q> said Hal Castellan of the U.S. Woods Hole Oceanographic Institution, a co-author of the study in the journal Nature Climate Change.
    </p>

    <cite>“Emperor Penguin Population to Slide Due to Climate Change”, Scientific American, June 29, 2014, https://bit.ly/2mvSYrT</cite>
</blockquote>
```



### Form : 사용자로부터 인풋Input을 받기 위한 태그

```html
<form action="주소" method="GET|POST">
    ...
</form>
```

`action="주소" ` form을 처리할 로직이 있는 url



### input, 타입 및 속성

```html
<input type="text" />
<input type="email" />
<input type="password" />
<input type="url" />
<input type="number" />
<input type="file" accept=".png, .jpg" />
```

- placeholder
- minlength, maxlength
- min, max
- required
- disabled
- value (초기값)



### label

```html
<label for="인풋id">라벨</label>
<input id="인풋id" type="text"/>
```



### Radio & Checkbox

```html
<input type="radio" id="apple" name="fruit" value="apple">
<label for="apple">APPLE</label>
<input type="radio" id="banana" name="fruit" value="banana">
<label for="banana">BANANA</label>
```

label, id, name, value 등 주의



### Table

`<table>`, `<thead>`, `<th>`, `<tr>`, `<tbody>`, `<td>`

`<td rowspan="2">`, `<tr colspan="5">` : 테이블 병합을 위해

`<th scope="col|row">` : browser가 th의 성격/속성에 대해 명확하게 알 수 있도록



### Media 파일

```html
<audio src="foo.mp3" controls></audio>
```

```html
<audio autoplay>
	<source src="foo.mp3" type="audio/mpeg"/>
    <source src="foo.wav" type="audio/wav"/>
    <source src="foo.ogg" type="audio/ogg"/>
    <p>
        해당 브라우저에 오디오가 지원되지 않습니다. 크롬을 사용하세요.
    </p>
</audio>
```

```html
<video src="foo.mov" controls></video>
```

```html
<iframe src="임베드 하고싶은 html문서의 주소"></iframe>
```

iframe의 경우 보통 youtube share -> embed(퍼가기)에서 쉽게 가져올수있음



### 기타 tag

`<abbr>` 약자

`<address>` 연락처 - 물리적인 주소, URL, email, 전화번호, SNS 등

`<pre>` preformatted text

`<code>`



### Doctype & Document Structure

```html
<!DOCTYPE html>
<html>
  <head>
    <!--웹 문서에 대한 메타 데이터-->
  </head>
  <body>
	<!--웹 문서에 들어갈 내용-->
  </body>
</html>
```

`<title>` 검색 최적화(SEO)에 매우 중요. 페이지마다 무엇에 관한 내용인지 잘 써주는 게 좋음.

`link:css + 탭` 



**Spoqa Han Sans** <- Good!!!



### Meta tag

```html
<meta name="메타데이터 종류" content="메타데이터 값">
```

```html
<!-- 화면 크기 -->
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<!-- 작성자 -->
<meta name="author" content="heecheol">

<!-- 그 외에 keywords, description 등이 있음 -->
```





