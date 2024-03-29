# 이상진 학번 202130410

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



