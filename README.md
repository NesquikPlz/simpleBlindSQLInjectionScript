# simpleBlindSQLInjectionScript
simple blind SQL injection automation python script
<br><br>
간단한 블라인드 SQL 인젝션 자동화 파이썬 스크립트
<br>
웹사이트 로그인 페이지를 대상으로 공격을 수행함
<br><br>
과제때매 만든거니까 실제 웹사이트에 쓰면 안됨요
<br><br>
코드 설명 : binary search 이용해서 비번 한글자씩 찾음
<br>
이정도면 semy brute force 인듯함
<br><br>
![image](https://user-images.githubusercontent.com/77532413/130666746-ddebc182-94ca-451a-b075-5886ac2be69a.png)
<br>
이 사이트를 대상으로 공격 수행 (내 사이트 아니라서 공개 못함)
<br><br>
해당 사이트로 말할 것 같으면 . . .
<br>
* 입력값 검증 안함<br>
* 입력 크기 제한 없음<br>
* 존재하지 않는 아이디라면 "등록되지 않은 아이디입니다", 비밀번호가 틀렸다면 "비밀번호가 틀립니다!" 라는 경고문이 뜸<br>
* 비밀번호는 ascii code로 표현 가능함<br>
<br><br>
위와 같은 특징을 기반으로 파이썬 자동화 스크립트를 작성함
<br>
코드 잘 읽어보고 대상 웹페이지에 맞게 알아서 수정해서 쓰면 됨
<br>
binary search 부분은 case 고려할게 많아서 잘못 수정하면 귀찮아 질 수 있음
<br><br>
사용방법은 다음과 같음
<br>
* 코드 다운받아서 cmd로 실행시킴 (Python3 기반이고 numpy랑 requests 라이브러리 필요)<br>
* 웹페이지 URL이랑 비번 알고싶은 아이디 시키는 대로 입력하면 됨<br>
* 결과는 다음과 같다.<br>
<br>
![image](https://user-images.githubusercontent.com/77532413/130668949-a1391416-ad45-4c01-9e80-9065166a85f7.png)
<br><br>
다음과 같이 비밀번호가 나옴(비번이 길다면 좀 기다려야 함)
