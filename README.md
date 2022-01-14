# comento-backend
Comento assignment repository

---

## 1주차 과제 : 개발 환경 셋팅
1. JDK 설치

- JDK 다운로드
- 환경변수 설정
- Path 변수 편집
- javac 실행하여 동작하는지 확인
2. Eclipse, Spring 다운로드 및 설치

- EclipseIDE for Java EE developers 설치
- Eclipse.ini 파일에 -vm C:\Program Files\Java\jdk1.8.0_221\bin\javaw.exe 추가
- 인코딩 UTF-8로 셋팅
- 이클립스에서 STS 설치

3. 톰캣 설정

- Topmcat9 설치
- Eclipse에서 Tomcat 서버 추가

4. Hello World 출력

- Spring MVC Project 생성 후 서버 구동시켜 Hello World 확인

![image](https://user-images.githubusercontent.com/62919440/147928428-721b06cd-faba-441d-9a44-0311b6a480a6.png)


5. mariaDB, mySql WorkBench 설치 및 샘플 DB 구축

- mariaDB 10.6.5 버전 설치
- MySQL Workbench 8.0.27 설치
- 스키마 설정 후 샘플 DB 데이터 삽입, 조회 수행

![image](https://user-images.githubusercontent.com/62919440/147932086-e749e1bb-2b74-470b-8814-3ea11aefd5f5.png)


6. 스프링, Mariadb, MyBatis 연동, 데이터 조회

- POM.xml 수정 (mariadb, mybatis 관련 dependency를 추가)
- root-context.xml 수정
- mybatis-config.xml, logback.xml, log4jdbc.log4j2.properties, test.xml 작성, log4j.xml 코드 root logger 부분 수정
- home.jsp 작성 후 테스트 구동 


---

## 2주차 과제 : 인터페이스 가이드 문서 작성

- API 문서 : https://github.com/ap3334/comento-backend/blob/main/SW%20%ED%99%9C%EC%9A%A9%20%ED%98%84%ED%99%A9%20API.docx

1) HTTP 통신에 관하여 

- Hyper Text Transer Protocol : Hyper Text를 전송하기 위한 프로토콜
- 요청 Request, 응답 Response로 이루어짐
- 클라이언트가 서버에게 요청을 보냄
- 클라이언트 사용자에게 응답 받은 결과를 보여줌
- HTTP 통신은 stateless하다 -> 서로 요청한 것들을 기억하지 않는다

2) 브라우저에 URL을 입력 후 요청하여 서버에서 응답하는 과정까지에 대해 학습한 내용

- 브라우저에서 각각 프로토콜, URL, 포트를 해석하여 분석한다.
- DNS 서버에 요청하여 URL을 IP주소로 변환한다.
- 대상 서버와 통신하기 위해 TCP 소켓 연결을 진행한다. (소켓 연결은 3-way-handshake 과정을 통해 이루어짐)
- 서버에 해당 페이지를 요청한다.
- 서버는 이 요청에 대한 응답을 생성하여 브라우저에게 전달한다.
- 브라우저에서 응답(HTML, CSS, Javascript 등)을 해석해 페이지를 보여준다.
