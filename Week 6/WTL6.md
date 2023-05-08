GDSC 6주차 ( Box Model & FLEX BOX )

Box Model ( 1, 블록 레벨 요소 / 2. 인라인 레벨 요소 )
div 박스의 테두리 : border 
예
div{
border : 3px solid red;
}


1. 블록 레벨 요소
div, p, h5 > 한 줄을 차지하는 박스 (부모 요소의 전체 칸을 차지한다.)

2. 인라인 레벨 요소
자신만을 감싸는 박스




contents: 내용
border : 테두리 
padding : contents와 border 사이의 간격
margin : border와 다른 요소 사이의 여백 ( 어떤 요소와 어떤 요소 사이의 여백 ) 

순서 : top > right > bottom > left 
예 margin : 10px 30px 0px 20px ( top right bottom left 순서로 적용된다 )
예 margin : 10px 30px (top,bottom 10px 적용, / left, right : 30px 적용된다 ) 


FLEX Box Layout
아이템이 배열될 방향인 주축을 정할 수 있다.

예
flex-box{
display : flex;
flex-direction: row;
}

main axis 

cross axis


column 과 row

아이템이 특정 축에서 어떻게 정렬될 지를 지정할 수 있다.

justify-content :main axis 
align-item :cross axis

저주 콘서트
크로스 라인

reference 사이트 참고하기!

css grid layouts
can I use
