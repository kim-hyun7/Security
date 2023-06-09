# Worm (Malware)

웜은 스스로를 **복제** 하는 악성 프로그램이다.  
바이러스가 다른 실행 프로그램에 기생하여 실행되는데 반해 웜은 독자적으로 실행되며 다른 실행 프로그램이 필요하지 않다.

# 매스메일러형 웜

매스메일러형 웜은 **자기 자신을 포함하는 대량 메일을 발송**하여 확산하는 형태이다.

제목이 없는 메일이나 특정 제목의 메일을 전송하고, 사용자가 이런 메일을 읽었을 때 시스템이 감염된다.

매스메일러형의 웜: 베이글, 넷스카이, 두마루, 소빅 등

- 특히 출처나 내용이 확인되지 않은 메일을 읽었을 때 확산된다.
- 베이글 웜은 가짜 메시지 출력.
- 넷스카이 웜은 윈도우 시스템 디렉터리 밑에 CSRSS.exe 실행 파일을 만든다.
- 변형된 종류에 따라 시스템에 임의의 파일을 만든다.

# 시스템 공격형 웜

시스템 공격형 웜은 운영체제 고유의 취약점을 이용하여 내부 정보를 파괴하거나, 컴퓨터를 사용할 수 없는 상태로 만들거나, 외부의 공격자가 시스템 내부에 접속할 수 있도록 악성 코드를 설치하는 형태이다. 패스워드가 취약한 시스템을 공격하는 웜도 있다.

- 전파할때 과다한 트래픽 발생.
- 공격 성공 후 UDP/5599 등의 특정 포트를 열어 외부 시스템과 통신한다.
- 시스템 파일 삭제 또는 정보 유출이 가능하다.

# 네트워크 공격형 웜

네트워크 공격형 웜은 특정 네트워크나 시스템에 대해 Dos 공격을 수행한다. 시스템 공격형 웜과 네트워크 공격형 웜은 시스템 취약점을 이용하여 확산 및 공격하는 경우가 많다.

- 네트워크가 마비되거나 급격히 느려진다.
