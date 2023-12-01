# 템플릿 문법
## 보간법
- 문자열: 데이터 바인딩의 기본 형태는 이중 중괄호 구문의 문자열 보간법
    ```html
    <span>{{ msg }}</span>
    ```
    - msg 속성이 변경될 때마다 갱신됨
    - 갱신을 원치않고 즉, 반응성이 필요없는 일회성 보간을 수행하고 싶을 경우 v-once 디렉티브 사용
    ```html
    <span v-once>변하지 않아용! {{ msg }}</span>
    ```
- 원시 html
    - 실제 html 출력하려면, v-html 디렉티브 사용해야함
    ```html
    <p>{{rawHtml}}</p>
    <p v-html="rawHtml"></p>
    ```