## v-card
- v-flex 안에서 카드형태 부분을 띄우거나 이미지를 넣거나 그림자 넣을 수 있음. 


### 삼항 연산자
- 조건문
  - ? 조건문이 참이 아닌 경우 실행구문
  - : 조건문이 참인 경우 실행구문


### vuex에 로그인 값을 저장하는 이유
- 중앙저장소에 저장해둠으로써 어디에서든 불러올 수 있음.


### guard
- 특정 상태가 아닌 경우 router 접근 금지
- 예: 로그인이 안됐는데 마이페이지 접근 / 로그인 했는데 로그인창 접근

### 의존성 모듈 관리
- 버전에 따른 에러가 발생하지 않게 package.json 파일만 있으면 
- `npm install` 만 있으면 에러 없이 package 사용 가능.
- ```npm install axos --save```를 통해 명세 저장.

### Fake API
- reqres.in

### Postman
getPostman.com
- 주소창에 데이터 보내는 방법
    - 1. query: 보안 신경쓸 필요 없음
    - 2. parameter: body에 보내고자 하는 정보를 담음.


##
- functions x () 대신 x => ()를 사용할 것
- callback함수에서 function을 쓰게 되면 vue instance를 가리키는 게 아니라 function 내부를 가리키게 되므로 arrow function 사용할 것.
- 받아온 데이터를 vue 내부의 변수에 할당시켜줘야 하기 때문.

## 로그인 프로세스
- 서버와의 통신 때 토큰을 통해 로그인을 진행함
  - 토큰에 아디/비번 정보를 담아 유저 정보 요청
  - 서버에서는 토큰을 확인하고 유저정보를 보내면 store에 유저 정보를 저장.
- 토큰은 정해진 시간이 지나면 초기화 됨.
- post방식: 링크 뒤에 파라미터가 올 수 있음.
- get 방식: 링크 뒤에 config(보안관련)