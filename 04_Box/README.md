## box model

html의 모든 요소는 box 형태로 구성되어 있는데

css에서는 이 형태, 구조을 box model이라고 함.



box model은 Margin, Border, Padding, Content로 구성됨.



Content - width, height

Padding - Border와 Content 사이의 안쪽 여백

Border

Margin - 바깥쪽 여백, 요소와 요소 사이의 간격





## box sizing

box-sizing: content-box 가 default

border-box: padding, border 두께까지 포함

```css
* {
    box-sizing: border-box;
}
```





## Box

Box Type: block, inline, inline-block, flex

Box Type을 결정짓는 속성 => display





## Block

- width 값을 넣지 않을 경우 부모의 content만큼 width를 늘림
- width 값을 넣었을 경우 남는 공간은 margin으로 채워짐
- height 값을 넣지 않았을 경우 자식의 total height로
- width, height, border, margin, padding 값 조절 가능





## Inline

block vs inline => 면(영역) vs 선(흐름)

- width, height, padding-top, padding-bottom, border-top, border-bottom, margin-top, margin-bottom 사용 불가





## Inline-block

