# kakao clone site 2021

2021.01.23 ~

---------- 소개 ----------

1.  사용 언어
    -- HTML5, CSS3

2.  소개
    -- keyframe animation 효과를 이용하여 friends창에 들어갈 때 애니메이션
    송출.
    --> 원래는 자바스크립트로 처리해야하지만 html,css만 연습하기위해 사용하지 않음.
    --> 그로 인해서 friends창에 들어갈때 마다 애니메이션 효과를 봐야한다.(element상에서 삭제가 되지 않았기 때문)

    -- css에서 root를 이용하였다.  
     --> 다음 프로젝트때는 전부 완성 후 중복되는 css값을 root로 시켜
    유지 보수하기 용이하게 만들기.

3.  배운점
    -- screen, component로 css를 분리 작업했다.
    --> 기존에는 css를 잘 분리하지 않고 대부분 같은 css에 입력하여 사용했었는데, 분리하여 모듈화 시키니 나중에 수정을 해야할 때 편하다는 것을 느꼈다.

    -- id 사용을 최소화, 변수명 정리
    --> 원래는 id와 class를 마구잡이로 사용했었는데, 보통 html에서는 id의 사용을 자제하고 class를 주로 사용해야한다는 것을 배움(class는 재사용이 가능하여 모듈화시킬 때 편리함)
    --> 변수명도 - \_ 대문자를 마구잡이로 사용하였는데 변수명에 대한 정리를 할 수 있게 되어 나중에도 잘 사용할 수 있을것같다.

    - BEM(Block, Element, Modifier)
      ex) .header\_\_navigation--navi-text
      header --> block
      navigation --> element
      navi-text --> modifier

    ex2) form class = "search-form"
    input class = "search-form**input"
    button class = "search-form**button"
    /form

            .search-form ==> block
            .search-form__input, search-form__button
               ==> element

    BEM은 기본적으로 ID를 사용하지 않고 Class를 사용
    어떤 목적인가에 초점을 두어 사용
    이름을 연결할 때는 하이픈(-)을 하나만 써서 연결

    Block --> 재사용 가능한 기능적으로 독립적인 페이지 컴포넌트

    element --> 블럭을 구성하는 단위, 엘리먼트는 의존적인 형태를 나타냄.(자신이 속한 블럭 내에서만 의미를 가짐)

    modifier --> 블럭이나 엘리먼트의 속성을 담당
