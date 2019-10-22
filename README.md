# API
#### manage(lv = 0만 사용가능)
**user**
Method | Url | Detail
---- | ---- | ----
 GET | /manage/user | 유저 정보 리스트를 반환한다.
 PUT | /manage/user/{ _id } | 유저 정보 수정 API.
 DELETE | /manage/user/{ _id } | 유저 정보 삭제 API.


GET | POST | UPDATE | DELETE
---- | ---- | ---- | ----
다리 | 다리1 | 다리2 | 뚝배기깹니다
금 | 의 | 환 | 향

- GET /user/account/check-duplicate/id/{id} : ID 중복체크 API

- POST /user/account/signup : 회원가입 API. ID/비밀번호/닉네임을 받는다.

- POST /user/account/auth : 로그인 API. JWT 포맷으로 인코딩된 access token과 refresh token을 발급한다.

- GET /user/account/refresh : access token refresh API. refresh token의 expire가 얼마 남지 않았다면 refresh token도 새로 만들어서 발급해 준다.

- POST /board/categories : 카테고리 생성 API

- GET /board/categories : 카테고리 목록 API

- POST /board/posts : 게시글 작성 API

- GET /board/posts : 게시글 목록 API. category ID를 요청으로 optional하게 받아서, 카테고리별 필터링도 가능하게 할 생각이다.

- GET /board/posts/{post_id} : 게시글 내용 API

- PATCH /board/posts/{post_id} : 게시글 수정 API

- DELETE /board/posts/{post_id} : 게시글 삭제 API

- GET /board/posts/{post_id}/comments : 게시글의 댓글 목록 API

- POST /board/posts/{post_id}/comments : 댓글 작성 API
