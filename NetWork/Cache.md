## Web Cache

    사용자가 웹사이트(client)에 접속할 때, 정적 컨텐츠(JS,이미지, CSS)을 특정 위치에 저장하여, 웹 사이트 서버에 해당 컨텐츠를 매번 요청하여 받는 것이 아닌, 특정 위치에서 불러옴으로서 사이트 응답 시간을 줄이고, 서버 트래픽 감소 효과를 볼 수 있는 것을 말한다.

- Browser Cashes  
   브라우저 또는 HTTP 요청을 하는 Client Appliction에 의해 내부 디스크에 캐쉬
  캐시된 리소스를 공유하지 않는 한 개인에 한정된 캐시
  브라우저의 back버튼 또는 이미 방문한 페이지를 재 방문하는 경우 극대화

2. Proxy Caches
   Browser Cashes와 동일한 원리로 동작하며 Client나 Server가 아닌 네트워크 상에서 동작
   큰 회사나 IPS의 방화벽에 설치 되며 대기시간 & 트래픽 감소, 접근 정책 & 제한 우회, 사용률 기록등을 수행
   한정된 수의 클라이언트를 위해 무한 대의 웹 서버 컨텐츠를 캐시
3. GateWay Caches
   서버 앞 단에 설치되어 요청에 대한 캐시 및 효율적인 분배를 통해 가용성, 신뢰성, 성능등을 향상
   Encryption, SSL acceleration, Load balancing, Server/ cache static content, Compression 등을 수행
   무한 대의 클라이언트들에게 한정된 수의 웹 서버 컨텐츠를 제공
