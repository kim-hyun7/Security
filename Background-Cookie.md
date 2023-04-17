Cookie!!!!

클라이언트의 IP 주소와 User-Agent는 매번 변경될 수 있는 고유하지 않은 정보일 뿐만 아니라,
HTTP 프로토콜의 Connectionless와 Stateless 특징 때문에 웹 서버는 클라이언트를 기억할 수 없음.

Connectionless,Stateless 특성을 갖는 HTTP에서 상태를 유지하기 위해 쿠키(Cookie) 가 탄생했다!!!

쿠키(Cookie)는 Key와 Value로 이뤄진 일종의 단위.

Server 는 Client에게 쿠키(Cookie)를 발급.

Client → Server    request(+ Cookie)

Server는 Client의 request에 포함된 Cookie를 확인해 Client를 구분한다.

HTTP 프로토콜 특징
    Connectionless: 하나의 요청을 받고 하나의 응답을 한 후 종료함. 
                    새 요청이 있을 때 마다 항상 새로운 연결을 한다.
    Stateless: 통신이 끝난 후 상태 정보를 저장하지 않음.
                이전 연결에서 사용한 데이터를 다른 연결에서 요구할 수 없다.

