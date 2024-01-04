# Web Basic

## 1. HTML
### HTML 기초 문제!
- 적절한 태그를 사용해서 아래의 이미지와 같은 html 코드를 작성해보세요
    - ![html_test](./img/html_test.jpg)

## 2. CSS
### CSS 기초 문제!
- 1번에서 작성한 html 코드를 아래와 같이 꾸며보세요
    - ![css_test](./img/css_test.jpg)
    - 위와 같은 기본 틀만 지켜진다면 그 외의 요소는 마음대로 꾸며도 괜찮!

## 3. JavaScript
### JavaScript로 이벤트 넣기
- 2번에서 만든 HTML 요소 중 a태그를 클릭하면 아래와 같은 경고창이 나오도록 해주세요
    - ![js_test](./img/js_test.jpg)
    - 참고
        - document.body.addEventListener(type, listener)
            - 이벤트를 등록하는 함수
            - 해당 HTML 파일의 document 내부의 body 태그 안의 모든 요소에 이벤트를 주는 함수
            - 특정 요소에 이벤트를 주고 싶을 경우, document.body가 아닌 다른 요소를 선택
                - 선택하는 방법
                    - getElementById('id')
                    - getElementByClassName('id')
                    - 기타 등등.. 그 외의 함수는 검색
            - 인자
                - type
                    - 이벤트의 타입
                    - 주요 이벤트
                        - click
                            - 클릭 이벤트
                        - hover
                            - 마우스를 올리는 이벤트
                        - 기타 등등.. 자세한 내용은 아래 링크 참조
                        - https://developer.mozilla.org/en-US/docs/Web/Events
                - listener
                    - 지정된 유형의 이벤트가 발생할 때 실행되는 함수
                    - 발생한 이벤트 객체를 파라미터로 받음
                    - event.target
                        - listener에서 인자로 받는 event의 요소 중 하나
                        - 해당 이벤트가 발생한 대상(태그)를 리턴
                    - event.target.nodeName
                        - 해당 이벤트가 발생한 태그의 이름(예를 들면 li 태그, a 태그 등...)을 리턴