# Same Origin Policy (SOP)

브라우저는 웹 리소스를 통해 간접적으로 타 사이트에 접근할 때도 인증 정보인 쿠키를 함께 전송하는 특징을 가지고 있음.

이 특징 때문에 악의적인 페이지가 클라이언트의 권한을 이용해 대상 사이트에 HTTP 요청을 보내고, HTTP 응답 정보를 획득 하는 코드를 실행할 수 있다.

이를 브라우저의 보안 메커니즘인 Same Origin Policy을 이용하여 방어.

# Same Origin Policy의 오리진 (Origin) 구분 방법

오리진은 프로토콜 (Protocol, Scheme), 포트(Port), 호스트(Host)로 구성.

구성 요소가 모두 일치해야 동일한 오리진(Origin)!

# Cross Origin Resource Sharing (CORS)

Same-Origin Policy(SOP)의 제약을 넘어 서로 다른 출처(origin) 간의 자원 공유를 가능하게 하는 메커니즘.

일반적으로 웹 브라우저에서 스크립트를 사용하여 다른 출처의 API를 호출하거나, 이미지나 폰트 등의 리소스를 가져오는 등의 작업을 수행하는데, 이때 CORS를 사용하면 보안성을 유지하면서도 자원 공유가 가능하다.

CORS는 서버 측에서 구현하고, 브라우저와 서버 간에 이루어지는 통신에서 사용한다. 클라이언트(브라우저)가 다른 출처의 자원을 요청하면 서버는 응답에 CORS 관련 헤더를 추가하여 클라이언트에게 자원 공유 여부를 알린다.

# Access-Control-Allow-Origin

헤더 값에 해당하는 Origin에서 들어오는 요청만 처리.

# Access-Control-Allow-Methods

헤더 값에 해당하는 메소드의 요청만 처리.

# Access-Control-Allow-Credentials

쿠키 사용 여부를 판단.

# Access-Control-Allow-Headers

헤더 값에 해당하는 헤더의 사용 가능 여부를 표시..
