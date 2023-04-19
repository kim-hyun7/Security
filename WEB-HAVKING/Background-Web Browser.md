# 웹 브라우저

HTML 문서와 그림, 멀티미디어 파일등 월드 와이드 웹을 기반으로 한 인터넷의 컨텐츠를 검색 및 열람하기 위한 응용 프로그램.

# 웹 브라우저의 기본적인 동작

1. 웹 브라우저의 주소창에 입력된 주소(dreamhack.io) 해석(URL 분석)

2. dreamhack.io 에 해당하는 주소 탐색(DNS 요청)

3. HTTP를 통해 dreamhack.io 에 요청

4. dreamhack.io의 HTTP 응답 수신

5. 리소스 다운로드 및 웹 렌더링(HTML, CSS, Javascript)

# URL(Uniform Resource Locator): 웹에 있는 리소스의 위치 표현

http:// example.com /path ?search=1 #fragment

(http://) Scheme: 웹 브라우저가 어떤 프로토콜을 사용할지 지정.

(example.com) Host: 웹 브라우저가 어디에 연결할지 정하는 호스트 주소. 도메인이나 IP Address가 호스트로써 사용될 수 있음.

(/Path) path: 웹 브라우저가 연결하려고 하는 리소스에 대한 경로.

?search=1 Query: 웹 브라우저가 서버에게 전달하는 파라미터.

#fragment Fragment: 웹 브라우저만 가지고 있는 데이터입니다. 메인 리소스 (페이지) 내에서 서브 리소스를 식별.

# Domain Name

불규칙한 숫자로 이루어진 IP Address는 사람이 외우기 어려우므로,
일반적으로는 도메인의 특성을 담은 이름을 정의하여 IP 대신 사용.

# 웹 렌더링(Web Rendering)

서버로부터 받은 리소스를 이용자에게 시각화하는 행위.

서버의 응답을 받은 웹 브라우저는 리소스의 타입을 확인, 적절한 방식으로 이용자에게 전달함.

서버로부터 HTML과 CSS를 받으면 브라우저는 HTML을 파싱하고 CSS를 적용하여 이용자에게 보여줌.
