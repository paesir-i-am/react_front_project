# 개요
----
1. 리액트의 SPA를 이용하여 프론트엔드 프로젝트 구성
2. 새로운 페이지의 타겟 설정
: 모바일 점유율이 높아짐에 따라, 모바일 형식의 페이지 기반으로 웹페이지를 생성

----
# 개발일지
* 시연영상      : https://youtu.be/sQD_WO7NG6c
* PPT         : https://github.com/paesir-i-am/react_front_project/issues/9#issue-2687643235
* 개발 디스코드  : https://discord.gg/xVK9Amtjbf
----

## 핵심기능
1. 네이버 검색엔진 API
2. 카카오 소셜로그인 API
3. 게시판 및 카트 CRUD
4. SPA 를 통한 카테고리 구현
----

## 플로우차트

<img width="1525" alt="SCR-20241124-rxal" src="https://github.com/user-attachments/assets/9f4c8d81-add5-4ab5-b8b2-3da19ed12274">

----

## 시연영상

![소셜로그인](https://github.com/user-attachments/assets/1f477d10-88b4-492b-98e5-dbbcd7314ad0)
----
![쇼핑리스트불러오기](https://github.com/user-attachments/assets/2fb84ee3-46c5-47f7-98ae-71e17bdb79c0)
----
![글 조회 수정 삭제 댓글 작성 ](https://github.com/user-attachments/assets/338a4088-f7d3-4754-867f-46b7b465f85d)
----
![견적공유](https://github.com/user-attachments/assets/ce722728-b7a9-4c46-8831-b03bbcd13d13)
----
![장바구니수정삭제](https://github.com/user-attachments/assets/858c6a6f-a853-4fd3-9ae7-ef8baae2e567)
----














수정사항
   *   10/8 수정사항
        장바구니 메인에서 개수표시 -> 장바구니에 length 함수로 표현 (수정완)
        사양검토에서 사진 표시 -> 장바구니에서 대표 아이템만 보여주고 장바구니 전체 아이템의 수량을 표시함 & 문의 리스트에 사진 추가
        -> 컨텍스트의 카트아이템에서 인덱스 0번값을 활용하여 호출  -> 수정완
        Cpu 등 카테고리 페이지 들어갔을 때 장바구니 클릭 시 Api 검색값 안사라지고 같이 표현되는거 수정
        -> 카테고리와 하단 푸터 버튼들 동적페이지로 구성하여 로케이션 값 변경하지 않고 페이지 표기 -> 수정 완
        장바구니에 전체 리스트가 안보이고 하나만 보임
        -> 각각의 아이디값이 존재하지 않아 리랜더링이 안이루어짐
        -> 현재시각을 아이디값으로 지정해 아이디값에 따라 리랜더링하게 설정 -> 수정완
        api 검색값 product page Link 에서 동적페이지 구성으로 변환 완
   *  10/9 완성분에 대한 css 작업 완료
   *  10/10 동적페이지 구성 함수 if else 문에서 switch 문으로 변경
   *  10/10 memoization useMemo 통해
   *    1.검색 결과값 변하지 않으면 리랜더링 안하게 최적화
   *    2.장바구니 아이템 수량 체크와 장바구니 금액 합계도 장바구니의 아이템이 변해야 랜더링 하도록 변경
   *  10/10 useCallback 으로 handleAddToCart, handleCategorySelect 재사용
   *  10/10 관심상품 버튼 마이페이지 버튼으로 변경 -> 마이페이지 메인에 동적페이지 구성
   *  10/10 공유하기 url 링크 선택시 alert 추가하여 이용자에게 알림 추가하여 사용성 개선


* 10/19 API KEY 비공개 / 수정 PPT 업로드 완
