# HTTP: 웹의 기초

URI (Uniform Resource Identifier, 통합 자원 식별자)
- URL (Uniform Resource Locator, 통합 자원 지시자)
  - 스킴scheme(ex: HTTP 프로토콜, FTP) / 인터넷 주소 / 웹 서버 리소스
- URN (Uniform Resource Name, 유니폼 리소스 이름)

통상적인 관례에 따라 URI와 URL을 같은 의미

웹페이지는 여러 객체로 이루어질 수 있다.
- 웹페이지는 리소스의 모음

TCP/IP
- TCP (Transmission Control Protocol, 전송 제어 프로토콜)
  - 오류 없는 데이터 전송
  - 순서에 맞는 전달 (데이터는 언제나 보낸 순서대로 도착)
  - 조각나지 않는 데이터 스트림(언제든 어떤 크기로든 보낼 수 있다)
  
웹의 구성요소
- 프락시
  - 클라이언트와 서버 사이에 위치한 HTTP 중개자
- 캐시
  - 많이 찾는 웹페이지를  클라이언트 가까이에 보관하는 HTTP 창고
- 게이트웨이
  - 다른 애플리케이션과 연결된 특별한 웹 서버
- 터널
  - 단순히 HTTP 통신을 전달하기만 하는 특별한 프락시
- 에이전트
  - 자동화된 HTTP 요청을 만드는 준지능적(semi-intelligent) 웹 클라이언트

프락시 (Proxy)
  - 사용자를 대신해서 서버에 접근, 주로 보안을 위해 사용, 요청과 응답을 필터링

캐시 (Cache)
  - 자주 찾는것의 사본을 저장해두는 특별한 종류의 HTTP 프락시 서버
  - 다음번에 클라이언트가 같은 문서를 요청하면 그 캐시가 갖고있는 사본을 받을 수 있음

게이트웨이 (Gateway)
  - 다른 서버들의 중개자로 동작하는 특별한 서버
  - 주로 HTTP 트래픽을 다른 프로토콜로 변환하기 위해 사용


스킴의 바다
- http
  - 사용자 이름이나 비밀번호가 없다는것을 제외하고는, 일반 URL 포맷을 지키는 하이퍼텍스트 전송 프로토콜 (Hypertext Transfer Protocol) 스킴이다. 포트값이 생략되어 있으면 기본값은 80이다.
  - 기본형식:
    - http://<호스트>:<포트>/<경로>?<질의>#<프래그먼트>
    - http://www.joes-hardware.com/index.html
    - http://www.joes-hardware.com:80/index.html
- https
  - https 스킴은 http 스킴과 거의 같다. 다른 점이라고는 https는 HTTP의 커넥션의 양 끝단에서 암호화하기 위해
    넷스케이프에서 개발한 보안 소켓 계층(Source Sockets Layer, SSL)을 사용 한다는 것뿐이다. 
  - 문법은 HTTP와 같고 기본 포트 값은 443이다.
    - https://www.joes-hardware.com/secure/index.html
 

