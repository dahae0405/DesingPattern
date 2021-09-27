# DesingPattern
성공적인 설계 방법

#클래스의 인스턴스를 생성하는 여러가지 패턴들

#개념
"자동차를 생산"
객체 : 속성과 기능을 갖춘 것 > 클래스와 인스턴스를 포함하는 개념.
클래스 : 속성과 기능 정의 > 설계도
인스턴스 : 속성과 기능을 갖춘 것 중 실제하는 것 > 자동차 하나 하나.



# 싱글톤 
정적메모리에 올려놓고 쓸 수 있는 객체 > 생성은 1번만 + 호출은 여러번 
 
유형 : 여러 화면의 색을 블랙모드로 샛팅하기.
유형 : A시스템에서 (하나의) 스피커에 접근 할 수 있는 클래스를 만들어 주세요.
유형 : 하나의 커넥션풀에 여러 컨넥션을 만들어 주세요.

구현법
ㄴ 하나의 인스턴스만 생성하도록 -> static으로 정적메모리로 올리고, 멤버변수의 이름은 보통 "instance"라고 한다.
  ㄴ 외부에서 생성 못하도록 -> 생성자 접근자 private
  ㄴ 외부에서 호출 가능하도록 -> static(정적)메모리에 접근자 등록함  
 
개념2
static : 정적 메모리로 시스템 전체의 전역변수로 만들어준다. 동적메모리는 new로 생성한다.
