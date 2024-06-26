# 이상진 학번 202130410
## 6월 14일 강의
자바의 입출력 스트림
입출력 장치와 응용 스트림
*   입력 스트림:입력장치로부터 자바 프로그램으로 데이터를 전달하는 객체
*   출력 스트림: 자바 프로그램에서 출력 장치로 데이터를 보내는 객체

문자 스트림
* 문자만 입출력하는 스트림
* 문자가 아닌 바이너리 데이터는 스트림에서 처리하지 못함
* 문자가 아닌 데이터를 문자 스트림으로 출력하면 깨진 기호가 출력
* 바이너리 파일을 문자 스트림으로 읽으면 읽을수 없는 바이트가 생겨서 오류 발생

바이트 스트림
* 바이트를 단위로 다루는 스트림
* 단순 바이너리로 정보를 다룸
* 문자든이미지 바이트는 상관없이 다룰수있음

IP주소
* 네트워크 상에서 유일하게 식별될 수 있는 컴퓨터 주소
- 숫자로 구성된 주소
- 4개의 숫자가'.'으로 연결
* 숫자로 된 주소는 기억하기 어려워 www.naver.com같은 문자로 구성된 도메인이름을 사용

포트
* 통신하는 프로그램 간에 가상의 연결단 포트 생성
- ip주소는 네트워크 상의 컴ㅍ터 또는 시스템을 식별하는 주소
- 포트 번호를 이용하여 통신할 응용프로그램 식별
* 모든 으용프로그램은 하나 이상의 포트 생성
- 포트를 이용하여 상대방과 통신
## 6월 7일 강의
그래픽 기반 GUI 프로그래밍
스윙 컴포넌트에 의존하지 않고 선,원 이미지 등을 이용하여 직접 화면을 구성하는 방법
그래픽 기반 GUI 프로그래밍의 학습이 필요한 이유
* 컴포넌트의 한계를 극복하고 차트, 게임 등 자유로운 콘텐트 표현
* 그래픽은 컴포넌트에 비해 화면 출력 속도가 빠름
* 스윙 컴포넌트들로 모두 그래픽으로 작성되어 있어, 그래픽에 대한 학습은 자바 GUI의 바탕 기술을 이해하는데 도움
* 그래픽을 이용하여 개발자 자신만의 컴포넌트 개발

Graphics의 기능
1. 색상 선택하기
2. 문자열 그래기
3. 도형 그리기
4. 도형 칠하기 

repaint()
자바 플랫폼에게 컴포넌트의 페인팅을 실행할 것을 간접적으로 지시하는 메소드

멀티태스킹
다수의 작업을처리하는것
스레드와 운영체제
운영체제의 의해 관리되는 하나의 작업 혹은 태스크를 말하며 다수의 스레드를 동시에 실행시키도록 응용프로그램을 작성하는 기법을 멀티스레딩이라고함
* 스레드 코드 - 작업을 실행하기 위해 사용자가 작성한 프로그램 코드
* 스레드 정보 - 스레드 명, 스레드 ID. 스레드 소요시간, 스레드 우선순위 등 운영체제가 관리하는 정보

멀티태스킹과 멀티스래딩
멀티프로세싱은 하나의 응용 프로그램을 여러 개의 프로세스로 구성하여 각 프로세스가 작업(테스크)을 처리하도록 하는 기법
각프로세스는 고유한 메모리 영역을 보유하고 독립적으로 실행됨
- 단점으로 하나의 응용프램에 속하는 프로세스들 사이의 변수공유를 할수없어 통신기법이 어렵고 오버헤드가 크며 
프로세스 사이의 문맥 교환에 따른 과도한 작업량과 시간 소모 문제점이 있음

멀티스래딩
멀티프로세싱을 개선하기위한 방법으로 하나의 응용프로그램을 여러 스레드로 구성하고 각스레드로 하여 하나의 작업을 처리하도록 하는기법
멀티태스킹의 단점을 모두 개선함

자바 스레드
일반 스레드와 거이 차이가 없으면서 자바 가상 기계가 운영체제의 역활을한다.

자바 스레드 만드는방법
1. Thread 클래스 이용
2. Runnable 인터페이스 이용

스레드 동기화

## 5월 31일 강의
GUI 프로그래밍
자바의 GUI 프로그래밍 방법
1. 스윙 컴포넌트들을 이용하기
2. 캔버스 위에 그림을 그리듯 직접 그래픽 화면을 구성하기

JComponent
* 스윙 컴포넌트는 모두 상속받는 슈퍼 클래스, 추상 클래스
* 스윙 컴포넌트들이 상속받는 공동 메소드와 상수 구현
* JComponent의 주요 메소드 사례

JButton
버튼은 JButton 클래스를 이용하여 생성한다
사용자로부터 명령을 입력받기 위한 목적

이미지 버튼만들기  
* normalIcon
    버튼이 보통 상태에 있을 때 출력되는 디폴트 이미지로서, 생성자나 JButton의 setIcon(Icon image)을 통해 설정된다
* rolloverIcon
    버튼 위에 마우스가 올라가면 출력되는 이미지로서 JButton의 setRollover Icon(Icon image)을 호출하여 설정한다
* pressedIcon
    마우스 버튼이 눌려져 있는 동안 출력되는 이미지로서 JButton의 setPressed Icon(Icon image)을 호출하여  설정한다

JCheckBox
JCheckBox를 이용하면 선택과 해제(비선택) 두 상태만가지는 체크박스 컴포넌트를 만들수 있다
체크 박스는 체크박스 문자열과 체크박스 이미지로 구성된다

JRadioButton
라디오 버튼은 체크박스와 동일하지만 한가지, 각 체크박스는 독립적으로 선택/해제가 되지만,라디오버튼은 버튼 그룹에 속한 하나의 라디오버튼만 선택가능하다

JTextField
한줄의 문자열을 입력받는 택스트필드를 만들수있다
택스트필드에 문자열 입력도중 Enter키가 입력되면 Action이벤트가 발생한다
입력가능한 문자 개수와 창의 크기는 서로 다르며 응용프로그램에서 변경할 수 있다

JList<E>
사용자에게 하나 이상의 아이템을 보여주고 아이템을 선택하돍 하는 리스트 컴포넌트를 만들수 있다
E는 리스트에 삽입되는 아이템 타입으로,리스트를 생성할 때 E대신 아이템 타입을 대입하여 구체화 해야한다

JComboBox<E>
텍스트 필드, 버튼 그리고 드롭다운 리스트로 구성되는 콤보박스를 만들 수 있다
E는 콤보박스에 삽입되는 아이템의 타입으로, 콤보박스를 생성할 때 E대신 아이템의 대입하여 구체화해야 한다

메뉴 구성 
메뉴만들기 위한 요소
* 메뉴아이템 -JMenuItem을 이용하여 생성
* 메뉴 - 여러 개의 메뉴 아이템을 가짐. JMenu를 이용하여 생성
* 메뉴바 - 메뉴들이 붙이는 바이며, 프레임에 부착. JMenuBar를 이용하여 생성
* 분리선 - 메뉴아이템 사이의 분리선으로서 separator라고 부르며, JMenu의 addSeparator()메소드를 호출하여 삽입

메뉴반들기 과정
1. 메뉴바를 만든다
2. 메뉴를 만들어 메뉴바에 붙인다
3. 메뉴아이템을 생성하여 메뉴에 붙인다
4. 메뉴바를 프레임에 붙인다


## 5월 24일 강의
이벤트 기반 프로그래밍
이벤트의 발생에 의해 프로그램 실행 흐름이 결정되는 프로그래밍 패러다임

이벤트 객체
현재발생한 이벤트에 관한 여러 정보를 가진 객체이며,이벤트 리스너에게 전달된다
이벤트객체가 담는 정보
1. 이벤트 종류와 이벤트 소스
2. 이벤트가 발생한 화면 좌표 및 컴포넌트 내좌표
3. 클릭된 마우스 버튼 번호 및마우스의 클릭 횟수
4. 입력된 키의 코드값과 문자 값

리스너 이벤트
이벤트를 처리하는 자바 프로그램 코드,클래스코드로 작성
사용자의 이벤트 리스너 작성
자바의 리스너 인터페이스를 상속받아 구현
리스너 인터페이스의 모든 추상 메소드로 구현

이벤트 리스너의 3단계
1. 이벤트와 이벤트 리스너 선택 -목적에 필요한 이벤트와 리스너 인터페이스 선택
2. 이벤트 리스너 클래스 작성 - 리스너 인터페이스를 상속받는 클래스를 작성하고 추상 메소드 모두 구현
3. 이벤트 리스너 등록 - 이벤트를 받을 GUI 컴포넌트에 이벤트 리스너 등록

이벤트와 이벤트 리스너 선택
* 이벤트 : Action 이벤트
* 이벤트 리스너 : ActionListener
* 이벤트 객체 : ActionEvent

어뎁터 클래스
리스너 인터페이스를 상속받아 이벤트 리스너를 구현할떄 모드구현하는 부담이있지만
리스너 언터페이스의 추상 메소드를 단순 리턴하도록 미리 구현해 놓은 클래스를 제공

key 이벤트와 keyListener
사용자가 키를 입력할때 발생하는 이벤트(key 이벤트)
키 이벤트 리스너는 keyListener를 상속받아 구현한다


## 5월 17일 강의
컨테이너 배치
FlowLayout 배치관리자
컴포넌트가 삽입되는 순서대로 왼쪽에서 오른쪽 배치
배치할 공간이없으면 아래로 내려와서 반복한다

BorderLayout 배치관리자
컨테이너의 동 서 남 북 중앙의 5개 영역으로 나눔
5개 영역 중 응용프로그램에서 지정한 영역에 컴포넌트 배치

GridLayout 배치관리자
컨테이너를 프로그램에서 설정한 동일한 크기의 2차원 격자로 나눔
컴포넌트는 삽입순서대로 좌에서 우로 다시위에서 아래로 배치
CardLayout
컴포넌트를 카드배치처럼 배치

컨테이너의 디폴트 배치관리자
컨테이너 생성시 자동으로 생성되는 배치관리자

컨테이너에 새로운 배치관리자 설정
setLayout(LayoutManager lm)메소드 호출
lm을 새로운 배치관리자로 설정
사례
JPanel 컨테이너에 BorderLayout 배치관리자를 설정하는 예
컨텐트팬의 배치관리자를 FlowLayout 배치관리자로 설정

생성자
FlowLayout()
FlowLayout(int alignm int hGap, int vGap)
align 컴포넌트를 정렬하는 방법 지정. 왼쪽정렬(FlowLayout.LEFT),오른쪽 정렬(FlowLayout.RIGHT),중앙 정렬(FlowLayout.CENTER(디폴트))
hGap 좌우 두 컴포넌트 사이의 수평 간격, 픽셀 단위. 디폴트는 5
vGap 상하 두 컴포넌트 사이의 수직 간격, 픽셀 단위. 디폴트는 5

생성자
BorderLayout()
BorderLayout(int hGap, int vGap)
hGap 좌우 두 컴포넌트 사이의 수평 간격, 픽셀단위.디폴트는 0
vGap 상하 두 컴포넌트 사이의 수직 간격, 픽셀단위.디폴트는 0

생성자
GridLayout()
GridLayout(int rows,int cols)
GridLayout(int rows,int cols,int hGap, int vGap)
rows 그리드의 행 수 디폴트는 1
cols 그리드의 열 수 디폴트는 1
hGap 좌우 두 컴포넌트 사이의 수평 간격, 픽셀단위.디폴트는 0
vGap 상하 두 컴포넌트 사이의 수직 간격, 픽셀단위.디폴트는 0

배치관리자 없는 컨테이너
배치관리자가 없는 컨테이너가 필요한경우
컴포넌트의 크기나 위치를 개발자 임의로 결정하고자 하는경우
게임 프로그램과 같이 시간이나 마우스/키보드의 입력에 따라 컴포넌트들의 위치와 크기가 수시로 변하는경우
여러 컴포넌트들이 서로 겹치는 효과를 연출하고자 하는 경우

컨테이너의 배치관리자 제거
setLayout() 메소드로 컨테이너의 배치간리자를 제거할수 있다


## 5월 3일 강의
컬렉션의 개념
컬렉션. 요소라고 불리는 가변 개수의 객체들의 저장소
    :객체들의 컨테이너라고 불림
    :요소의 개수에 따라 크기 자동조절
    :요소의 삽입,삭제에 따른 요소의 위치 자동 이동
고정 크기의 배열을 다루는 어려움 해소
다양한 객체들의 삽입,삭제, 검색 등의 관리 용이

컬랙션은 제네릭(generics) 기법으로 구현
제네릭
    특정 타입만 다루지 않고,여러 종류의 타입으로 변신할 수 있도록 클래스나
    메소드를 일반화시키는 기법
    클래스나 인터페이스 이름에 <E>,<K>,<V>등 타입매개변수 포함

제네릭 컬렉션 사례: 벡터Vector<E>
    <E>에서 E에 구체적인 타입을 주어 구체적인 타입만 다루는 벡터로 활용
    
제네릭
    클래스나 메소드를 형판에서 찍어내듯이 생산할 수 있도록 일반화된 형판을 만드는 기법
    모든 종류의 데이터 타입을 다룰 수 있도록 일반화된 타입 매개 변수로 클래스(인터페이스)나 메소드를 작성하는 기법

벡터Vector<E>의 특성
    <E>에 사용할 요소의 특정 타입을구체화
    배열을 가변 크기로 다룰 수 있게 하는 컨테이너
        배열의 길이 제한 극복
        요소의 개수가 넘치면 자동으로 길이 조절
    요소 객체들을 삽입,삭제, 검색하는 컨테이너
        삽입,삭제에 따라 자동으로 요소의 위치 조정
    Vector에 삽입 가능한 것
        객체,null
        기본 타입타입의 값은 Wrapper객체로 만들어 저장
    Vector에 객체 삽입
        벡터의 맨 뒤,중간에 객체 삽입가능
    Vector에서 객체 삭제
        임의의 위치에 있는 객체 삭제 가능

HashMap<K,V>
키(key)와 값<value>의 쌍으로 구성되는 요소를 다루는 컬렉션
    K: 키로 사용할 요소의 타입
    V: 값으로 사용할 요소의 타입
    키와 값이 한쌍으로 삽입
    값을 검색하기 위해서 반드시 키 이용
삽입 및 검색이 빠른 특징
    요소 삽입:put()메소드
    요소 검색:get()메소드

자바 GUI
GUI 응용프로그램
GUI
    사용자가 편리하게 입출력 할 수 있도록 그래픽으로 화면을 구성하고,마우스나 키보드로 입력받을 수 있도록 지원하는 사용자 인터페이스
Swing 패키지
    AWT 기술을 기반으로 작성된 자바 라이브러리
    모든 AWT기능+추가된 풍부하고 화려한 고급 컴포넌트
    AWT 컴포넌트를 모드 스윙으로 재작성.AWT컴포넌트 이름앞에 J자를 덧붙임
    순수 자바 언어로 구현
    스윙 컴포넌트는 경량 컴포넌트
    현재 자바의 GUI로 사용됨

컨테이너
    다른 컴포넌트를 포함할 수 있는 GUI 컴포넌트
        java.awt.Container를 상속받음
    다른 컨테이너에 포함될 수 있음
        AWT 컨테이너
        Swing 컨테이너

컴포넌트
    컨테이너에 포함되어야 화면에 출력될 수있는 GUI 객체
    다른 컴포넌트를 포함할 수 없는 순수 컴포넌트
    모든 GUI 컴포넌트가 상속받는 클래스
    스윙 컴포넌트가 상속받는 클래스

최상위 컨테이너
    다른 컨테이너에 속하지 않고도 독립적으로 존재하여 출력될 수 있다

스윙 GUI 프로그램 만들기
과정
    1.스윙 프레임 작성
    2.main() 메소드 작성
    3.프레임에 스윙 컴포넌트 붙이기



## 4월 19일 강의
추상 클래스 상속
추상 클래스를 상속받으면 추상클래스가 됨
서브 클래스도 abstract로 선언해야함

추상 클래스 구현
서브 클래스에서 슈퍼 클래스의 추상 메소드 구현(오버라이딩)
추상 클래스의 구현한 서브 클래스는 추상 클래스 아님

추상 클래스의 목적
상속을 위한 슈퍼 클래스로 활용하는 것
서브 클래스에서 추상 메소드 구현
다형성 실현

인터페이스
클래스가 구현해야 할 메소드들이 선언되는 추상형
인터페이스 선언

자바 인터페이스에 대한 변화
java7 까지 
인터페이스는 상수와 추상 메소드로만 구성
java 8부터
상수와 추상메소드 포함
default 메소드 포함(java9)
private 메소드 포함(java9)
static 메소드 포함(java9)
여전히 인터페이스에는 필드(멤버변수) 선언 불가

인터페이스의 구성요소
상수
추상메소드
default메소드
private메소드
static메소드

인터페이스는 인터페이스간 상속가능, 다중상속 가능함

자바의 모듈과 패키지, 클래스 경로명

패키지 - 서로 관련된 클래스와 인터페이스를 컴파일한 클래스 파일을 묶어놓은 디렉토리
하나의 응용프로그램은 한개 이상의 패키지로 작성
패키지는 jar 파일로 압축할 수 있음

모듈 - 여러 패키지와 이미지 등의 자원을 모아 놓은 컨테이너
하나의 모듈을 하나의 .jmod 파일에 저장

JDK 패키지
자바 개발도구인 JDK는 화면 출력 키입력 네트워킹 등 프로그램 개발에 필요한 기본적인 기능과 다양한 응용 기능을 구현한 많은 클래스와 인터페이스들을 포함하는 표준 패키지를 제공
이를 자바 API라함

Object 클래스
object는 java.lang 패키지에 속한 클래스며 모든 클래스는 강제로 oject를 상속받는다
object만이 유일하게 아무 클래스도 상속받지않는, 자바 클래스 계층 구조의 최상위 클래스다

toString() 메소드
object에는 객체를 문자열로 변환하는 toString() 이있으며 각 클래스는 toString() 을 오버라이딩하여 자신만의 문자열을 리턴할 수 있다

equals() 메소드
객체 비교를위해 상ㅇ하는 메소드
☞ == 연산자 
==연산자는 두 객체의 내용물이 같은지를 비교하는 것이 아니라, 두 레퍼런스 값을 비교하는 것을 의미함
☞ boolean equals(object obj)
object의 equals(object obj) 는 자기 자신과 인자로 건내진 객체 obj를 비교하여 객체의 내용이 같은지를 비교하는 메소드이다

Wrapper 클래스

Wrapper 클래스는 기본 타입 값을 문자열로 변환하거나 문자열을 기본값으로 변환하는 메소드들이 주를 이루고 있음
많은 메소드가 static 타입이다

박싱과 언박싱
기본타입의 값을 Wrapper객체로 변환하는 것을 박싱(boxing)이라고 하고,반대의 경우를 언박싱(unboxing)이라고 한다
JDK 1.5 부터 박싱과 언박싱은 자동으로 이루어지며 이를 지동 박싱 자동 언박싱이라고 부른다

String과 StringBuffer 클래스
String 클래스는 문자열을 나타내며 스트링 리터럴은 String객체로 처리딘다
스트링 리터럴과 new String()으로 생성된 스트링은 서로 다르게 관리된다.
스트링 리터럴은 자바 내부에서 리터럴 테이블로 특별히 관리하여, 동일한 리터럴은 공유시킨다
그러나 new String()에 의해 생성된 스트링은 힙 메모리에 별도로 생성한다

스트링 객체는 수정이 불가능하다

스트링 비교, equals()와 compareTo()
스트링 비교에서 ==연산자를 절대 사용해서는 안되며 , 대신 String 클래스의 equals() 메소드를 사용해야한다
equals() 메소드는 스트링이 같으면 ture, 아니면 false를 리턴한다.

compareTO(String anotherString) 메소드는 현재 스트링과 anotherStirng 스트링을 사전 순서로 비교하여 같으면 0, 현재 스트링이 anotherString보다 먼저나오면 음수를 ,뒤에나오면 양수를 리턴한다

공백제거,trim()
trim()은 스트링 앞뒤에 있는 공백 문자를 제거한 스트링을 리턴한다

StringBuffer 클래스
StringBuffer 클래스는 스트링을 다루는 클래스로서,내부에 가변 크기의 버퍼를 가지고 문자의 개수에 따라 버퍼 크기를 자동조절한다
그러므로 String 객체와 달리 생성된 스트링의 수정이 가능하다

StringTokenizer 클래스
StringTokenizer 클래스는 문자열을 분리하기 위해 사용된다, 문자열을 분리할 때 상ㅇ되는 기준 문자를 구분문자(delimiter)라고하고 구분문자로 분리된 문자열을 토큰(token)이라고 한다


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



