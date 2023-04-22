# HTTP Method

**HTTP 메서드란 클라이언트와 서버 사이에 이루어지는 요청(Request)과 응답(Response) 데이터를 전송하는 방식을 일컫는다.**

# GET 메서드

**GET 메서드는 주로 데이터를 읽거나(Read) 검색할때 사용되는 메소드이다.**

- GET 요청은 idempotent 하기 때문에 호출로 인하여 데이터가 변형되지 않는다.

- GET 요청은 데이터가 주소 입력란에 표시되기 때문에 최소한의 보안도 유지되지 않는다.

# POST 메서드

**POST 메서드는 주로 새로운 리소스를 생성(Create)하는 메소드이다.**

- POST 요청은 URL에 요청 데이터를 기록하지 않고 HTTP 바디에 데이터를 전송하기 때문에 GET보다 안전하다.

- POST 요청은 idempotent 하지 않다.

# PUT 메소드

**PUT 메소드는 리소스를 수정하는(Update) 메서드이다.**

# DELETE 메서드

**DELETE 메서드는 리소스를 삭제(Delete)하는 메서드이다.**
