# Getting Started

## Basic
  ### 1. 프로그래밍이란?
  - 프로그래밍 언어를 사용하여 어떠한 프로그램을 만드는 행위
  - 프로그래밍을 통해 컴퓨터 프로그램, 모바일 프로그램(앱)...등 다양한 프로그램 제작

  ### 2. 프로그래밍 언어
  - 컴퓨터는 0과 1만 이해할 수 있음
  - 인간과 컴퓨터 사이의 효율적인 통신 방법을 위해 만들어진 언어가 프로그래밍 언어.
  - 인간의 언어와 가까우면 High Level 언어
  - 컴퓨터의 언어(0, 1)에 가까울 수록 Low Level 언어
  - 고수준(High Level) 언어를 저수준(Low Level) 언어를 바꿀 때 사용하는 프로그램을 컴파일러(Compiler)라고 하며, 바꾸는 작업을 컴파일링(Compiling)이라고 함.

  ### 3. Web browser
  - 웹 페이지를 탐색하고 상호작용 하는데 사용되는 소프트웨어
  - 월드 와이드 웹을 기반으로 한 인터넷으로 연결되어 있음
  - 웹 문서(HTML, CSS, JavaScript)를 해석하고 화면에 표시하는 기능으로 웹 페이지를 보여줌

  ### 4. DataBase
  - 체계적으로 구조화된 데이터의 집합을 저장하고 관리하는 시스템
  - 예시
    - 인스타그램의 피드에 포함되어 있는 데이터
      - 피드
        - 사진
        - 내용
        - 위치
        - 사용자
          - 사용자 아이디
          - 사용자 비밀번호(로그인을 위한 데이터)
          - 사용자 연락처
        - Like
          - 좋아요를 누른 "사용자" 정보
          - 좋아요의 수
        - 댓글
          - 댓글을 쓴 "사용자" 정보
          - 댓글 내용
          - 댓글을 쓴 시간
          - 댓글에 달린 "Like" 정보
          - 댓글의 수
    - 위 예시와 같은 데이터들을 체계적으로 구조화한 뒤 관리

  ### 5. 이런저런 용어들
  - HTTP
    - HyperText Transfer Protocol
    - WWW에서 정보를 전달하기 위한 프로토콜
    - 프로토콜이란, 정보를 전달할 때 어떻게 전달할지 서로 합의한 하나의 양식
    - 예를 들면 어떤 물건을 전달하고 싶다고 가정했을 때 아래와 같은 것들이 필요
      - 어떤 물건을 전달할지?
      - 물건을 어떻게 전달할지
      - 언제 물건을 전달할지
    - 위와 같은 요소를 합의하는 것이 프로토콜
  - HTTPS
    - HyperText Transfer Protocol Secure
    - HTTP에서 보안 요소를 추가한 프로토콜
    - 통신과 통신 사이에 보안 인증서를 추가하여 해당 연결이 안전한지 확인함과 데이터를 암호화하여 전달하는 역할 수행
    - 프로세스
      1. 브라우저를 이용해 웹 사이트(네이버, 구글 등...)에 접속
      2. 해당 사이트가 가지고 있는 암호화된 인증서를 브라우저에 전달
      3. 브라우저가 해당 인증서를 해독하여 인증서 확인(공개키)
      4. 브라우저는 3번의 인증서로 새로운 열쇠(대칭키)를 만들고 해당 열쇠를 암호화 하여 웹 사이트에 전달
      5. 웹사이트는 인증서를 이용하여 암호화한 열쇠를 해독
      6. 이후 4번에서 만든 열쇠로 통신
         - 이를 세션이라 함
      7. 통신이 끊어지면 4번의 열쇠는 폐기
      - 쉽게 설명하면 OTP같은 느낌
  - DNS
    - Domain Name System
    - 원래 인터넷 통신은 IP 주소라는 숫자를 통해서 연결함
    - 그러나 IP 주소를 외워서 웹 사이트에 접속하는 것은 비효율적이므로, 사람이 읽을 수 있는 문자로 대체해주는 시스템
    - 예시
      - 강남역에서 만나고 싶음
      - 강남역의 주소는 "서울 강남구 강남대로 396"
      - '우리 서울특별시 강남구 강남대로 396에서 만나자!' 라고 하는것은 비효율적
      - '우리 강남역에서 만나자' 라고 하는것과 비슷한 개념
  - URI
    - Uniform Resource Identifier
    - 웹 사이트의 주소
    - DNS와 비슷해보이지만, URI의 영역이 좀 더 큼
    - 예시
      - https://www.youtube.com/shorts/CbauMbMVebc?feature=share
        - 위와 같은 주소가 있을 때
        - DNS
          - www.youtube.com
          - 해당 주소값에 유튜브의 IP 주소가 매핑되어 있음
        - URI
          - https://www.youtube.com/shorts/CbauMbMVebc?feature=share
          - 위와 같이 웹 사이트 전체 주소가 URI
  - URL
    - Uniform Resource Locator
    - URI의 한 종류
    - URI와 URL의 차이
      ![URI](./URI.png)
      > https://developer.mozilla.org/ko/docs/Learn/Common_questions/Web_mechanics/What_is_a_URL
        - 이 주소는 URL
      > https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Web_mechanics/What_is_a_URL#basics_anatomy_of_a_url
        - 이 주소는 URI
  - API
    - Application Programming Interface
    - 서로 다른 소프트웨어에 정보나 신호를 주고받는 시스템
    - UI는 사용자와 컴퓨터간의 정보를 연결하지만, API는 컴퓨터나 소프트웨어끼리의 정보를 연결한다는 차이가 있음
    - 다양한 API 프로토콜이 있으나 대표적인 REST API 하나만 보도록 하자..
  - REST API
    - Representational State Transfer
    - HTTP를 기반으로 통신하는 다양한 API 프로토콜 중 하나
    - 구성 요소
      - 자원
        - Resource
        - API를 통해 가져오는 서비스를 구별하는 요소
        - 대부분 URL를 이용하여 구별
        - 어디에서 해당 API를 가져올지에 대한 주소값
      - 행위
        - Verb
        - 클라이언트가 서버를 통해 어떤 행동을 할 것인지 요청하는 요소
        - HTTP Method
          - GET
            - 데이터를 단순히 요청만 하는 과정
            - 데이터를 가져오는 역할만 함
            - https://youtu.be/rIr5Y_5Xk98?si=ZNB4WFZf_Imc4Ill&t=257
              - 위 웹사이트 주소에 들어가면 유튜브 영상이 나오는데, 해당 데이터를 가져오는 GET 요청을 통해 해당 영상을 볼 수 있음
          - POST
            - 새로운 데이터를 만드는 요청
            - 유튜브 페이지에 댓글을 달 경우, POST 요청을 사용하여 새로운 댓글을 추가
          - PATCH
            - 특정 데이터의 부분만 수정하는 요청
          - PUT
            - 특정 데이터의 전체를 수정하는 요청
            - PATCH와 PUT는 개념적으로는 구별하지만, 대부분은 PUT 요청을 사용함
          - DELETE
            - 특정 데이터를 삭제하는 요청
      - 표현
        - Representations
        - 클라이언트와 서버 간에 교환되는 데이터의 형태
        - 주로 JSON 형식을 사용
        ```json
        {
          "id": 1,
          "name": "song",
          "email": "song@test.com"
        }
        ```
  - 프레임워크
    - 소프트웨어 개발을 위한 기본 구조
    - 요리를 할 때, 밀키트와 같은 느낌
    - 밀키트가 없다면 재료를 직접 구하고, 손질하는 등의 수고로움이 늘어나지만 밀키트를 사용하면 좀 더 간단히 할 수 있음
  - 라이브러리
    - 개발할 때 컴퓨터 프로그램이 사용하는 특정 기능을 수행하는 코드
    - 프레임워크가 밀키트라면, 라이브러리는 토핑 느낌
    - 우삼겹 떡볶이가 먹고 싶다면, 떡볶이 밀키트(프레임워크)에 우삼겹 토핑(라이브러리)를 더해서 만들 수 있음
  - Function
    - 코드를 정의하고 해당 코드를 실행하는데 사용되는 키워드


## Tool
  ### 1. Editors
   - 프로그래밍을 위한 코드를 작성하는 편집 도구
   - 추천 에디터
      - Visual Studio Code
        - MS에서 만든 무료 에디터
        - 다운로드 링크
        > https://code.visualstudio.com/

  ### 2. 웹 브라우저
   - 웹 개발시, 코드가 어떻게 실행되는지 확인하기 위해 필요
   - 추천 브라우저
     - Chrome

  ### 3. 형상 관리 프로그램
   - 형상관리?
     - 프로그램을 개발할 때 프로그램의 변경점을 추적하고, 관리해주는 도구
     1. git
         - 클라우드 서비스(N드라이브, Google Drive...) 방식으로 소스코드 관리
         - 추천 툴
           - git bash
             > https://git-scm.com/
             - 커맨드를 이용하여 git 관리 가능

           - source tree
             > https://www.sourcetreeapp.com/
             - git 관리를 GUI로 제공

         - github?
           > https://github.com/
           - 깃을 제공해주는 사이트 중 하나.
           - 깃을 제공해주는 사이트는 여러 군데가 있는데, 그 중 가장 사용자가 많음