# Position

요소를 원하는 위치에 자유롭게 이동시키기 위해 사용하는 속성



### 종류

static, relative, absolute, fixed, (sticky)



### 생각해야할 부분

- Type (어떤 종류의 Position을 사용하고 있는지)
- 기준점 (내가 사용할 Position은 무엇을 기준으로 위치시켜야 하는지)





## static

- 모든 요소의 기본 Position값



## relative

- (이동의) 기준점 : 요소가 원래 있던 자리
- float와 달리 형제요소, 부모요소가 원래 있던 자리를 기억해 영향을 받지 않음



## absolute

- position: absolute는 float와 비슷
  - 떠다님 (부모의 height 변화)
  - display 속성이 block으로 바뀜
  - block이지만 자동으로 margin을 채우지는 않음
  - float와 달리 inline 컨텐츠가 position 영역을 완전히 무시
- absolute는 기준점을 골라서 선정 가능 (float는 부모에 종속적으로 갇혀있었음)
  - 단 기준점은 position: static이 아닌 조상 요소
  - 조상 요소에 가장 안전하게 사용할 수 있는 게 position: relative
  - 조상 요소의 top, left, bottom, right을 기준으로 움직일 수 있음



## fixed

- position: absolute와 비슷한 현상, 결과를 보여줌
- 기준점은 항상 viewport (보고있는 브라우저 창의 전체 크기)



## z-index



