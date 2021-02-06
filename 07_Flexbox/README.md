# Flexbox



### step1

정렬을 하고자하는 요소들의 부모에 `display: flex;`



### step2

어느 방향으로 정렬을 할 건지

`flex-direction: row; /* row-reverse | column | column-reverse */`



Flex-direction에 따라 두 개의 Axis가 결정되는데 

Flex-direction과 같은 방향이 Main axis이고 수직 방향으로 Cross axis가 생긴다.



### step3

`flex-wrap: nowrap;` (default) 요소들의 크기를 줄여서라도 한 줄로

`flex-wrap: wrap;` 공간이 넉넉하지 않으면 여러줄로



### step4

Main axis 방향의 정렬 => justify-content

Cross axis 방향의 정렬 => align-items 또는 align-content



justify-content의 value: flex-start, center, flex-end, space-between, space-around





**align-items와 align-content 차이**

`flex-wrap: wrap`로 여러 줄이 생기게 되었을 때 align-items의 경우 flex line도 여러 개가 생긴다.

그래서 정렬 시 각각의 flex line 안에서 정렬이 된다.

반면 align-content의 경우 하나의 flex line으로 정렬이 되면서

space-between, space-around까지 사용 가능하다.



**order**

flex box 내 요소들의 순서를 order: 2, order: 1 이런식으로 바꿀 수 있다.