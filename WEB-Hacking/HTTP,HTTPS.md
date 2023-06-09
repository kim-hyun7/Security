# HTTP (HyperText Tranfer Protocol): 웹 서버와 클라이언트가 리소스를 교환하기 위해 사용하는 프로토콜.

클라이언트가 서버에게 요청하면 서버가 응답하는 메커니즘.

- **HTTP 헤드**

HTTP 헤드의 각 줄은 CRLF로 구분되며, 첫 줄은 시작 줄(Start-line),
나머지 줄은 헤더(Header)라고 부른다.

헤드의 끝은 CRLF 한 줄로 나타낸다.

헤더는 필드와 값으로 구성되며 **HTTP 메시지** 또는 **바디의 속성**을 나타낸다.

- **HTTP 바디**

HTTP 바디는 헤드의 끝을 나타내는 CRLF 뒤, 모든 줄을 말한다.

클라이언트나 서버에게 **전송하려는 데이터**가 바디에 담긴다.

# HTTPS (HTTP Secure)

**HTTP 프로토콜의 보안 버전으로, 인터넷 상에서 데이터를 암호화하여 전송하는 프로토콜이다.**

HTTPS는 HTTP 프로토콜 위에 SSL/TLS 암호화 프로토콜을 추가하여 보안성을 강화하였다.

HTTPS를 사용하면 데이터 전송 과정에서 중간자 공격과 같은 공격으로부터 보호된다.

이는 HTTPS 통신에서 사용되는 SSL/TLS 인증서를 통해 인증되는데, 인증서는 제3자 기관에서 발급되어 인증서의 유효성이 검증되는 것이 일반적이다. 또한 HTTPS를 사용하면 데이터의 암호화를 통해 민감한 정보가 유출되는 것을 방지할 수 있다.
