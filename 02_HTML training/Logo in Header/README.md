# img 요소 

https://developer.mozilla.org/ko/docs/Web/HTML/Element/img#%EC%9D%B4%EB%AF%B8%EC%A7%80_%EB%A7%81%ED%81%AC



`<img src="" alt="">`

alt 특성이 중요한 이유, 활용

- 이미지를 가져올 수 없을 때

- 이미지 링크

  이 예제는 이전 코드에 더해 이미지를 링크로 바꾸는 법을 보입니다. 단순히 `<img>` 태그를 [``](https://developer.mozilla.org/ko/docs/Web/HTML/Element/a) 안에 넣기만 하면 됩니다. 다만 고려할 점 하나는, 해당 링크가 가리키는 곳을 설명하는 대체 텍스트를 포함해야 한다는 것입니다.

  ```html
  <a href="https://developer.mozilla.org">
    <img src="https://developer.mozilla.org/static/img/favicon144.png"
         alt="Visit the MDN site">
  </a>
  ```

- 적합한 대체 설명을 작성해야 함. 무의미한 이미지일 경우 빈칸으로라도 남겨두기

