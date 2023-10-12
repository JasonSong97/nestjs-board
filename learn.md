## (1) NestJS 소개

## (2) 게시물 CRUD APP

### NestCLI로 생성한 프로젝트 기본구조

- eslintrc.js
  - 개발자들이 특정한 규칙을 가지고 코드를 깔끔하게 짤 수 있게 도와주는 라이브러리
  - 타입스크립트를 쓰는 가이드 라인 제시, 문법에 오류가 나면 알려주는 역할 등등
- prettierrc
  - 주로 코드의 형식을 맞추는데 사용
  - 작은따옴표 사용? 큰따옴표 사용 이런 것들
  - eslintrc.js도 물론 코드의 포맷터 역할을 하지만 prettierrc가 훨씬 코드의 포맷터 역할을 함
- nest-cli.json
  - nest 프로젝트를 위해 특정한 설정을 할 수 있는 json 파일
- tsconfig.json
  - 어떻게 타입스크립트를 컴파일 할지 설정
- tsconfig.build.json
  - tsconfig.json의 연장선상 파일, build를 할 때 필요한 설정들 "excludes"에서는 빌드할 때 필요 없는 파일 명시
- package.json
  - build : 운영환경을 위한 build
  - format : 린트에러가 났을지 수정
  - start : 앱 시작
- src 폴더(비즈니스 로직)
  - main.ts(앱 생성하고 실행)
  - app.module.ts(앱 모듈 정의)

### 기본 구조에서 살펴보는 Nest.JS 로직 흐름

