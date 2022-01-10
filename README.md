# Inflearn_node_react_basic
## Node.js Basic
- 몽고 DB 연결하기
  - 몽고 DB 사이트 회원가입 (https://www.mongodb.com/)
  - 클리스터 생성
  - 몽고 DB 유저 생성
  - Mongoose 다운로드 => npm install mongoose --save
  - App에 MongoDB 연결하기

- NODE MON = 소스를 변경할 때 그걸 감지해서 자동으로 서버를 재시작해주는 tool
  - node mon 설치 => npm install nodemon --save-dev
  - nodemon으로 시작한다 => package.json에 script 하나 더 만들기

- DB 비밀번호 암호화하기
  - Bcrypt 설치
  - index.js에 register코드에 가서 save하기전 비밀번호 암호화
  - User.js에 비밀번호 암호화 함수 추가

- 로그인 시 필요한 라이브러리
  - DB에 저장된 이메일과 비밀번호가 입력한 값과 같다면 토큰을 생성한다.
  - 토큰 생성을 위해 필요한 JSONWEBTOKEN 라이브러리 다운 => npm install jsonwebtoken --save 

## React.js Basic
- React란?
  - Library이다. 기능들을 컴포넌트화 시킬 수 있다.
  - Virtual DOM (여러개에 리스트 중 한가지만 Update할 때 전체 리스트를 reload하는 것이 아닌 바뀐 한가지만 DOM에서 바꿔준다.)
  - 어떻게 Virtual DOM이 한가지만 Update 할 수 있을까?
    - 1. JSX을 렌더링한다. 그럼 Virtual DOM이 Update가 된다.
    - 2. Virtual DOM이 이전 virtual DOM에서 찍어둔 Snapshot과 비교를 해서 바뀐 부분을 찾는다.(== diffing)
    - 3. 그 바뀐 부분만 Real DOM에서 바꿔준다.
