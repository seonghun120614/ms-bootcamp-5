컴파일 : 프로그래밍에서 사람이 읽을 수 있는 소스 코드를 컴퓨터가 이해할 수 있는 기계어로 변환하는 과정

인터프리터 : 인터프리터는 코드를 한 줄씩 읽어 내려가며 실행하는 프로그램

컴파일과 인터프리터의 차이

컴파일 : 번역을 먼저 끝내고, 그 다음 실행
인터프리터 : 한 줄 번역, 한 줄 실행
Javac로 컴파일을 한 뒤 Class파일이 생기면 Java 명령어로 출력

자연어 : 

예약어 : 코드를 작성할 때 이미 지정되어있는 단어, 변수로 사용할 수 없

식별자 : 

접근 제어자 : 

Class 이름의 규칙 : 파일이름과 같아야한다.

Class가 여러개일 경우 메인 Class의 이름과 파일 명을 동일하게 만들면 된다.

public class Hello {
    public static void main(String[] args) {
        System.out.println("Hello");
    }
}
public class = 예약어, Hello = 식별자

Main Method : 

static : new를 입력하지 않아도 메모리로 올려줌

void : 리턴파일

main : Method 이름, jvm은 main을 찾기 때문에 이름이 바뀌면 출력이 안됨

args : 변수(아무거나 가능)

String[] args: 명령줄에서 전달받는 인자들

System.out.println("") : 콘솔에다가 ""을 출력해줘

; 자바에서 세미콜론(;)은 "명령문(statement)의 끝"을 표시하는 기호

public static void main(String[] args) { // 약속된 것들




public class My {

    public static void main(String[] args) {
        System.out.println("안녕하세요");
        System.out.println("허준형 입니다");
        System.out.println("반갑습니다");
    }

}
1. 중괄호 { } 의 기본 의미
자바에서 중괄호는 "블록(block)"을 만드는 기호

블록은 여러 명령문(statement)을 하나로 묶는 단위
블록 안의 코드는 같은 범위(scope) 에 속하게 됨
즉, { 는 블록 시작, } 는 블록 종료를 의미

2. 세미콜론(;)의 이유
자바에서 세미콜론(;)은 "명령문(statement)의 끝"을 표시하는 기호
System.out.println("안녕하세요"); 는 "이 출력 명령이 여기서 끝난다" 라는 뜻을 가짐
Java는 Class라는 단위로 만들어져야하고 그를 구성하는 Method가 필요.

컴파일 (javac)
javac Hello.java
- .java → .class 파일로 변환 - 컴파일 성공 시 Hello.class 생성

실행 (java)
java Hello
- JVM이 .class 파일을 실행 - 확장자(.class) 생략!

javac: 소스코드를 바이트코드로 변환
java: 바이트코드를 실행
// ================================
// 1️⃣ 클래스 선언 (Class Declaration)
// ================================
public class My {

    // ================================
    // 2️⃣ 메인 메서드 (Main Method)
    // 프로그램 실행의 시작 지점
    // ================================
    public static void main(String[] args) {

        // ================================
        // 3️⃣ 출력문 (Print Statements)
        // 콘솔에 문자열을 출력
        // ================================
        System.out.println("안녕하세요");    // 1번 실행
        System.out.println("허준형 입니다"); // 2번 실행
        System.out.println("반갑습니다");    // 3번 실행

    } // 메인 메서드 끝

} // 클래스 끝
구조 설명
클래스 선언 (public class My)
프로그램의 틀(설계도) 역할
클래스 안에 메서드, 변수 등을 포함
메인 메서드 (public static void main)
프로그램 실행 시작 지점
JVM이 가장 먼저 호출
블록 { ... } 안에 실행할 명령문을 작성
출력문 (System.out.println)
콘솔에 문자열을 출력하는 동작(명령문)
작성한 순서대로 실행