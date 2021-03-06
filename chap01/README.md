# 자바 시작하기

## 01-1 프로래밍 언어와 자바

**기계어 = 이진코드** : 컴퓨터가 이해할 수 있는 언어

**프로그래밍 언어 = 소스파일** : 사람이 이해할 수있는 언어 

**컴파일** : 소스파일을 기계어로 번역하는 과정

**JDK** : (java development kit) 자바로 프로그램을 개발할 수 있는 실행환경 (JVM)과 개발도구(complier) 제공

OpenJDK, OracleJDK( 상업용으로 쓰는건 유료이나 LTS, 즉 장기 지원 서비스가 제공되므로 버그 개선 업데이트 버전을 꾸준히 받을 수 있다.) 

```
Java SE 11.0.2 (LTS)
```

차례대로 주버전, 개선 버전, 업데이트 버전을 나타내는 숫자이다.

**JDK 설치 경로 = JAVA_HOME**

```
C:\Program Files\Java\jdk...
```

***JAVA_HOME 환경변수에 설치 폴더 경로 등록***

​	시스템 속성-고급-환경변수-새로만들기

**JAVA bin 폴더**

​	자바 소스 파일을 컴파일 해주는 javac, 컴파일된 파일을 실행해주는 java 명령어 등 존재

​	다른 폴더에서 실행하기 위해 환경변수 PATH에 bin 폴더 등록

***환경변수 PATH에 bin 폴더 등록***

​	시스템 속성 - 고급 - 환경변수 - 시스템변수 - PATH 선택 - 편집 - 

​	환경변수편집 - 새로만들기 - *%JAVA_HOME%\bin* 입력 - 위로 이동 - 확인눌러 설정 마침



## 01-2 이클립스 개발 환경 구축

**Eclipse** : 무료 사용 가능한 오픈소스 통합 개발환경 IDE

**IDE** : 프로젝트 생성, 자동 코드 완성, 디버깅 등과 같이 개발에 필요한 여러 기능 통합적으로 제공하는 툴



## 01-3 자바 프로그램 개발 과정

자바 소스 파일(.java) -> (컴파일, javac) -> 바이트 코드 파일(.class) -> ~~(JVM이 java 명령어 실행)-> 기계어 -> 실행~~

**JVM** : 바이트 코드 파일을 해당 OS에서 실행 가능한 기계어로 번역하는 소프트웨어, JDK에 포함

```diff
+ 바이트 코드 파일을 다양한 OS에서 수정하지않고 사용 가능
```

**패키지 선언**

```
package sec03.exam01;
```

**클래스 선언**

```
public class Hello { <= 클래스 선언
		--클래스 블록--
}
```

**메소드 선언**

```
public static void main(String[]args) { <= 메소드 이름
		--메소드 블록--
}
```

**메인 메소드**

바이트 코드 파일 실행 시 main 메소드를 찾아 블록 내부를 실행함

프로그램 실행 진입점

**주석**

컴파일 과정에서 무시되고 실행문(변수 선언, 값 저장, 메소드 호출)만 바이트 코드로 번역됨



***

***