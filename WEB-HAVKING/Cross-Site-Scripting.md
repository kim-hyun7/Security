# Cross-Site-Scripting(XSS)

Cross-Site-Scripting의 약어가 XSS인 이유

CSS라고 불리는 것이 맞지만, 스타일시트를 정의하는 언어인 CSS와의 중복으로, 혼동되어 사용될 수 있기 때문에 XSS로 명명.

클라이언트 사이드 취약점 중 하나로, 공격자가 웹 리소스에 악성 스크립트를 삽입해 이용자의 웹 브라우저에서 해당 스크립트를 실행할 수 있음.

# Stored XSS

XSS에 사용되는 악성 스크립트가 서버에 저장되고 서버의 응답에 담겨오는 XSS

# Reflected XSS

XSS에 사용되는 악성 스크립트가 URL에 삽입되고 서버의 응답에 담겨오는 XSS

# DOM-based XSS

XSS에 사용되는 악성 스크립트가 URL Fragment에 삽입되는 XSS

Fragment는 서버 요청/응답 에 포함되지 않습니다.

# Universal XSS

클라이언트의 브라우저 혹은 브라우저의 플러그인에서 발생하는 취약점으로 SOP 정책을 우회하는 XSS
