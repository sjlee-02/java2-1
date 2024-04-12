# 이상진 학번 202130410

## 4월 12일 강의
static 멤버
static 멤버는 클레스당 하나만 생성
객체들에 의해 공유된다

static메소드의 제약조건
1.static메소드는 오직 sttiac맴버만 사용가능
2.static메소드는 this 사용불가

final 클래스와 메소드
final이클래스앞에 사용되면 클래스를 상속받을 수 없음을 지정함
final이 메소드앞에 붙으면 이 메소드는 더이상 오버라이딩할수 없음을 지정함

final필드
final로 필드 선언하면 필드는 상수가 된다

상속의 개념
객체지향언어에서의 상속은 부모여전자를 자식이물려받는 유전적상속과 유사
상속은 클래스 사이에 코드중복을 제거하여 클래스를 간결하게 구현가능

상속의 장점
1.클래스 사이의 멤버 중복 선언 불필요-클래스의 간결화
2.클래스들의 계층적 분류로 클래스 관리 용이
3.클래스 재사용과 확장을 통한 소프트에어의 생산성 향상

자바의 상속선언
자바에서는 extends 키워드를 사용하여 상속을 받음
상속하는 부모클래스를 슈퍼클래스(super class)
상속받는 자식 클래스를 서브클래스(sub class)

자바상속의 특징
1.자바에서 클래스의 다중 상속을 지원하지않음
[다중 클래스 상속은 여러가지문제점을 갖고있어서 하지않지만 인터페이스(interface)는 다중상속이 가능]
2.자바의 모든 클래스는 자바에서 제공하는 object클래스를 자동으로 상속받도록 컴파일 된다(object클래스는 유일하게 슈퍼클래스를 갖지않는 클래스임)

슈퍼클래스의 protected 멤버는 두가지 경우에 접근이 가능하다
1.같은 패키지에 속한 모든클래스
2.상속되는 서브 클래스(같은 패키지든 다른패키지든 상관없음.)

슈퍼클래스와 서브클래스
각각 여러개 생성자 작성가능

서브 클래스의객체가 생성될때 슈퍼클래스 생성자 1개와 서브 클래스 생성자1개가 생성

서브 클래스의 생성자와 슈퍼클래스의 생성자가 결정되는방식
1.개발자의 명시적 선택
2.컴파일러가 기본생성자 선택

업캐스팅
서브 클래스의 래퍼런스를 슈퍼클래스 래퍼런스에 대입
슈퍼클래스 래퍼런스로 서브클래스 객체를 가리키게 되는 현상

다운스캐닝
슈퍼클래스레퍼런스를 서브클래스 레퍼런스에 대입
업캐스팅된 것을 다시원래대로 되돌리는것
반드시 명시적 타입 변환 지정

instanceof 연산자 
레퍼런스가 가르키는 객체의 타입 식별

오버라이딩
메소드 오버라이딩은 서브 클래스에서 슈퍼클래스에 선언된 메소드를 
중복작성하여 슈퍼클래스에 작성된 메소드를 무력화 시키고 객체의 주인이되는것
오버라이딩은 동적바인딩을 통해 실현된다

동적바인딩
실행할 메소를 컴파일시에 결정하지않고 실행 시에 결정하는 것
super
정적 바인딩을 통해 슈퍼클래스의 멤버에 접근할수 잇다

오버로딩과 오버라이딩
오버로딩은 한클래스나 상속관계에 있는 클래스에 서로 매개변수의 타입이나 개수가 다른 여러개의 메소드가 같은이름으로 작성되는것을 말함
오버라이딩은  슈퍼클래스에 있는 메소드와 이름,매개변수 타입과 개수,리턴 타입등이 모두 동일한 메소드가 서브클래스에 재정의 되었을 경우를말함

추상메소드
abstract로 선언된 메소드,메소드의 코드는 없고 원형만 선언

추상클래스
추상메소드를 가지며,abstract로 선언된 클래스
추상 메소드없이, abstract로 선언된 클래스
## 4월 5일 강의
<메소드의 배열리턴>
배열 리턴
-배열의 레퍼런스만 리턴(배열 전체가 리턴되는 것은 아님)
메소드의 리턴타입
-리턴하는 배열 타입과 리턴 받는 배열 타입이 일치해야함
-리턴 타입에 배열의 크기를 지정하지않음

<자바의 예외처리>

자바의 예외 클래스
자바 플랫폼은 응용프로그램이 실행 중 오류를 탐지할 수 있도록  많은 예외를 클래스형태로제공

클래스와 객체
자바의 특징
1.캡슐화
2.상속
3.다형성

클레스란
객체의 속성과 행위선언
객체의 설계도 혹은 툴

객체란
클래스의 틀로 찍어낸 실체
프로그램 실행중에 생성되는 실체
메모리 공간을갖는 구체적인실체
인스턴스라고도 부름

생성자란
개체가 생성될 때 초기화를 위해 실행되는 메소드

생성자의 특징
1.생상자 이름은클래스이름과 동일
2.생성자는 여러개 작성가능
3.생성자는 객체 생성시 반드시 한번호출
4.생성자의 목적은 객체생성시 초기화
5.생성자는 리턴 타입을 지정할수 없음

객체배열

메소드

가비지

객체 소멸

패키지
상호 관련 있는 클래스파일을 저장하여 관리하는 디렉토리
자바 응용프로그램은 하나 이상의 패키지로 구성

Staitc 멤버

## 3월 29일 강의
자바는 system.in으로 바이트정보를 프로그램이 문자나 숫자로 변환하는 것에 번거로움이 있어
입력된 키를 문자나,정수,실수,문자열 등 사용자가 원하는 타입으로 변환시켜주는 고수준 스트림 클래스 scanner를 사용함
scanner 객체를 사용할때는 import문을 프로그램 맨앞줄에 써야함(import java.util.scanner;)
그후 마지막 줄에 scanner을 닫아준다(scanner.close();)

{ scanner 클래스의 주요 메소드}

String next() :다음토큰을 문자열로 리턴
byte nextByte() :다음토큰을 byte 타입으로 리턴
short nextShort() :다음토큰을 short 타입으로 리턴
int nextInt() : 다음토큰을 int타입으로 리턴
long nextLong() : 다음토큰을 long타입으로 리턴
float nextFloat() :다음토큰을 Float타입으로 리턴
double nextDouble():다음토큰을 Double타입으로 리턴
boolean nextBoolean() 다음토큰을 boolean 타입으로 리턴
String nextLine() : '\n'을 포함하는 한 라인을 읽고'\n'을 버린 나머지만 문자열로 리턴
void close()  :Scanner의 사용종료
boolean hasNext() 현재 입력된 토큰이 있음ture 아니면 새로운 입력 될때까지 무한정 대기, 새로운 입력이 들어올 때 ture 리턴. crtl-z키가 입력되면 입력 끝이므로 false리턴

>조건문
if문
if-else문
다중 if-else문, 중첩 if-else문
switch문

>반복문
자바는반복 연산프로그래밍은3가지 종류를 제공한다
for문
while문
do-while문
중첩반복문
-반복문안에 다른반복문을 만드는 중첩반복문
for문안에 다른for문이나 while문,while문안에 for,while,do-while문을 둘수있음
반복은 몇번이고 중첩할수 있지만 너무많으면 구조를 복잡하게함으로 2~3개가 적당함

continue문 :반복무을 빠져나가지않으며 즉시다음 반복으로 넘어가게해줌
break문 : 하나의 반복문을 즉시 벗어나게 해줌



## 3월 22일 강의
ctrl+shift+p -> create java project file
자바 기본프그래밍

리터럴
▶프로그램에 직접 표현한 ㄱ밧
▶정수,실수,문자,논리,문자열 타입 모두 리터럴이있음

상수
▶final 키워드 사용
▶선언시 초깃값 지정
▶실행 중 값 변경 불가

var 키워드
▶java 10부터 도입
▶기존의 변수 선언 방식: 변수의 타입 반드시 지정
▶타입을 생략하고 변수 선언 가능
▶컴파일러가 추론하여 변수 타입결정
▶변수선언시 초깃값이 주어지지 않으면 컴파일 오류
▶var는 지역 변수 선언에만 한정


## 3월 15일 강의
내용 정리  



