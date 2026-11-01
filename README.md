### Assignment 4-1. REST API-Based CRUD Service with JavaScript

- Deployment: 
    - GitHub URL:https://github.com/2026-2-OSS/assign09-c01-22500248  
    - Vercel URL: https://2026-oss-assign09-sandy.vercel.app
    - MockAPI Endpoint URL: https://6adea7084e88f1bba4a53bf7.mockapi.io/movie

- Service: 
    - 주제: 영화 관리 프로그램
    - Field: id, title, director, year, genre, rating 
    - CRUD 기능: load / add / update / delete / search

- Key Learning: fetch(), JSON, async/await, REST API 등 배운 내용 3가지
    1. fetch는 결과 바로 주지 않아서 await함수로 기다려야한다. response.ok로 성공여부를 확인하고 response.json함수로 데이터를 꺼낸다.
    2. 같은 URL이여도 방법에 따라 조회, 추가, 수정, 삭제가 달라진다. POST/PUT에는 해더로 데이터 형식과, 객체에서 글자로 바꿔주는 작업이 필요하다.
    3. 데이터 보낼 땐 JSON.stringify로 객체에서 문자열로 변경해서 보내고, 받을 때는 response.json함수로 문자열에서 객체로 변환하여 데이터를 받는다.
- AI / Search Usage: 우선 개념을 이해하기 위해서 AI를 사용하여 fetch, JSON 등 개념을 학습하고 피피티를 바탕으로 피피티에 없는 구현 내용 부분 코드 부분을 잘 작성하였는 지 확인하고 코드 구조를 계획하는 용도로 AI를 사용하였다.
AI가 기여한 기여율은 30%정도인 것. 같다.

- Problem & Solution / Reflection: PATCh가 에러로 막혀서 LowerCase에 ()를 빼먹어서 코드를 잘 확인해야겠다. / 이번 과제를 하면서 외부에서 데이터를 가져와서 그 데이터를 바탕으로 crud를 만들어보며 백엔드의 개념을 약간 이해하게 된 것 같고, 내가 실제로 앱을 사용할 때 경험하는 것보다 프로그램에서는 훨씬 복잡한 과정이 필요함을 깨달았다.