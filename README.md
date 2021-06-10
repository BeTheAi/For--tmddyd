# Nodejs0426
Nodejs practice

기본 crud부터 시작하여 결제기능 등 ***추후 프로젝트를 위한 기반 기술들을 구현해볼 프로젝트  


--05.22  
◆ 다중 사용자 기능 완성 및 posting 기능 기반 완성 및 mongodb 오류 해결  

--05.23  
◆ showpost 및 listpost 기능 추가  
◆ Foundation commit  

//추후 navbar action 추가해야함. --done  

--05.25  
◆ navbar action 추가  
◆ showpost rendering 부분 수정 및 오류 해결  

--05.26  
※ 미들웨어가 자꾸 2번 or 3번 호출된다 정신나갈거같애정신나갈거같애정신나갈거같애정신나갈거같애 favicon.ico문제 아님 @$%@#%!#%!@^&$  

//미들웨어 중복 호출 문제 해결해야 함. #조회수가 n배로 찍혀 상당히 곤란함; -- 06.03. 아무것도 건들지 않았는데 갑자기 중복호출되지 않음;;  
//포스트에 조회수 표시해야 함. -done  
//포스트 상세조회 뷰에 댓글기능 추가해야함. -done  
//포스트 검색기능 추가해야함. -done  

--05.26 (연등)  
◆ listpost 게시물페이지로 이동 기능 추가  
◆ 마우스 이벤트 추가  
◆ 댓글 기능 추가  
◆ writer -> name으로 변환 진행중  

--05.27  
◆ writer -> name으로 변환  
◆ 작성자에 적용 #동기처리를 해야만 값이 넘어감. --> 완료(async 괜히 설치함.)  

--05.27 (연등)  
◆ list->show 작업 시 body안에 head 내용 중복되는 문제 발견 -- 해결, 해당 과정 ajax 방식에서 location 이동 방식으로 변경.  

//글 수정 및 댓글 수정 기능 추가해야함. --글 수정은 done  
//이미지 업로드 기능 추가해야함. --done  

--05.28  
◆ 포스트 검색 기능 추가함.

//검색기능에 작성자로도 검색할 수 있도록 기능 추가해야함. -> 제목, 내용 변경하는 버튼 드롭다운으로 대체할까 고려 중. -- profile page에서만 내가 쓴글 조회 가능하도록 ui추가함. 

--05.29  
◆ multer 설치 -> local에서 이미지 처리  

--05.31(연등)  
◆ 검색 input태그에 enter이벤트 추가  
◆ 리스트페이지에서 keypress이벤트 발생 시 검색란 focus 추가  --06.10 기능 삭제
◆ 검색결과 창에서 내용 or 제목 옵션 유지되도록 추가  
◆ /process/addpost의 image 첨부 안했을 경우의 예외처리  
◆ post 상세페이지를 작성자 본인이 들어갔을 경우 삭제 기능 추가  
			

//유저 간 채팅 서비스 추가할 예정  
//post 상세페이지를 작성자 본인이 들어갔을 경우 수정 기능 추가 중.. --done  

--06.01(연등)  
◆ 게시글 수정기능 추가  
◆ 라우터에 multer err 핸들링 추가  
◆ 라우터에 multer fileFilter 예외처리  

--06.03(연등)  
◆ Back 버튼의 onclick event를 history로 수정  
◆ profile 페이지에서 내가 쓴 글 볼 수 있는 버튼 && 기능 추가  
◆ listpost 댓글 수 ui 추가  
◆ back 버튼 댓글 작성 시 referrer가 보안상 하나전까지만 담을 수 있어 list로 못 빠져나감. --> 댓글 다는 방식을 ajax로 변경함. -----> 실패 추후 다시 할 예정

--06.04  
◆ 댓글 다는 방식을 ajax로 변경 성공 form 태그 안에 버튼 타입을 submit으로 유지해서 헤맸음. --> 댓글 문자열이 특수코드로 변환되는 문제 남음. --> form data를 객체형식으로 serialize해서 해결.


--06.06  
◆ chat 기능 개발 시작 -- "socket.io": "^4.1.2" 설치 [cdnjs](https://cdnjs.com/libraries/socket.io)  
◆ 실시간 채팅 기능 초기단계 완료  

//비밀채팅방 + 비밀번호 거는 기능 추가해야함.

--06.08  
◆ chat page를 우측 하단 floating btn을 통한 켜고 끌 수 있는 기능 구현  

// 채팅방 ui 제작 해야함.  
// 채팅 page 화면 resizing하면 ui 겹치는 문제 해결해야함. -- position fixed로 전부 수정하여 일단 해결(chat page가 화면 사이즈마다 resizing되게 할지는 고민)  

--06.10  
◆ chat page css 수정  
◆ 모든 창에서 chating 기능 이용할 수 있도록 함.(chat.js, chat.css, chatpage.ejs, footer.ejs에 관련 내용있음.) ++ listpage에서 자동 focus기능 삭제함.  
