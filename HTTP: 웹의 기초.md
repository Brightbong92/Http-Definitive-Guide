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
