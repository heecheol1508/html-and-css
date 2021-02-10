# Transition



스르륵



#### 설정해야할 속성

- property
  - all | font-size | background-color 등 어디에 transition을 적용할 지
- duration
  - millisecond | second
- [timing-function]
  - ease-in | ease-out | ease-in-out | cubic-besizer() | ...
  - ease-in : 천천히 바뀌다가 점점 빠르게
  - cubic-besier.com 참고 (Custom timing function)
- [delay]





# Animation

animation 은 animation-property 로 쪼개서 사용하는 게 편리함



#### animation 정의

```css
@keyframes name {
    from {
        /* Rules */
    }
    
    to {
        /* Rules */
    }
}
```

```css
@keyframes name {
    0% {
        /* Rules */
    }
    
    50% {
        /* Rules */
    }
    
    100% {
        /* Rules */
    }
}
```



#### animation 적용

- animation-name
- animation-duration
- animation-timing-function
- animation-delay
- animation-iteration-count
- animation-direction (alternate!!)
- ...



animation 이 끝나면 다시 원래 상태로 돌아옴

