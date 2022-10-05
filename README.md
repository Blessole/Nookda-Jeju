# 🍊 Nookda, Jeju | 눅다, 제주 🍊
제주의 감성이 담긴 유니크한 숙소만 모은, **숙소 검색 및 예약 웹사이트** <br>
'눅다'는 눕다의 제주 방언입니다 :)
<br>
<br>
## 🍊Description 
### 동기 및 목적
* 거리두기 완화로 '제주' 여행 수요가 국내 최고치로 증가
* 개인 숙소 예약 사이트의 분산으로 번거롭고 어려워진 장소 선택
* 감성적인 공간을 선별한 '제주만의 매력적인 숙소' 추천

### 기대효과
* 소비자에게 '특별한 경험'이 될 수 있는 숙소 정보를 선별 제공하여 여행 만족도를 향상시킴
* 최근 제주 여행 수요와 맞물려 제주의 경제회복에도 도움이 될 수 있음

### 프로젝트 기간 / 인원
* 2022년 4월 29일 ~ 2022년 7월 3일
* 4명 (Full-Stack)
  * 김솔, 김하영, 배현정, 손지민
<br>
<br>

## 🍊 Techs Used
<img src="https://user-images.githubusercontent.com/101856058/193999920-a9ce05ba-df55-443f-8c62-576de182df23.png">
<br>
<br>

## 🍊 ERD
![ERD2](https://user-images.githubusercontent.com/101856058/193999639-876b7a00-b746-4de4-87b5-598b7c4f4296.png)
<br>
<br>

## 🍊 Menu Tree
![menuTree](https://user-images.githubusercontent.com/101856058/193999441-7c85f7e0-72f5-4691-ba4f-4f5e3d36a616.png)
* Main Page / Search Page
* Accomodation Page / Booking Page
* My Page
* Host Page
* Admin Page
<br>
<br>

## 🍊 Main Functions with Screenshots
### ◾ Main Page
* 메인페이지 상단
  ![image](https://user-images.githubusercontent.com/101856058/194003243-5e7b1422-9778-4032-b5cd-69c9c6984618.png)
  △ [눅다,제주]의 분위기를 대표할 메인 영상 자동 재생, 무한 루프
  <br>
  <br>
  ![image](https://user-images.githubusercontent.com/101856058/194006638-b60f0f65-4b44-4a1d-9e80-773c2ed00220.png)
  △ Header/Navigation Bar - 로그인 전, 후 이용자 타입에 따라 아이콘 변경됨
<br>
<br>
  
* 조회수 TOP 6 숙소
  ![image](https://user-images.githubusercontent.com/101856058/194002163-36fa1359-de42-4dee-99be-0f045c721788.png)
  △ Swiper Slide 방식 구현
<br>
<br>

* 지도를 이용하여 지역별 숙소 검색 기능
  ![image](https://user-images.githubusercontent.com/101856058/194002307-5b396cc8-7e9b-4cb5-8ad3-f1852d249710.png)
  △ 이미지 맵 에디터를 이용해 지역에 맞는 좌표 값에 링크 삽입
<br>
<br>

### ◾ Header - Search Section
* 검색 모달을 이용하여 기간별, 지역별, 인원별 숙소 검색 기능
  ![image](https://user-images.githubusercontent.com/101856058/194002971-c3299bbe-e561-4358-872c-b5db3c4920c6.png)
  ![image](https://user-images.githubusercontent.com/101856058/194003044-4c92d9b3-c04d-4200-87a1-4403f29c2fc0.png)
<br>
<br>

* 검색 조건에 따라 sort 후 결과 출력
  ![image](https://user-images.githubusercontent.com/101856058/194005347-e28e6191-14e6-4ebc-9578-13919bd3935a.png)
<br>
<br>

### ◾ Accomodation Page
* 숙소 상세 정보 제공
  ![image](https://user-images.githubusercontent.com/101856058/194009966-0a991fdf-fa23-4e46-82ac-f1a9d73a0df0.png)
  △ 숙소 이미지 : jQuery를 이용한 Carousel 방식으로 좌우 슬라이드 구현 
  <br>
  △ 연락하기 버튼 : 호스트에게 쪽지 문의 기능 (DB CRUD/ajax 이용)
  <br>
  <br>
  ![image](https://user-images.githubusercontent.com/101856058/194010533-ab0ec3c8-9aea-4ece-aa8f-5bc8e87bc747.png)
  △ 네이버 지도 API 이용 - 숙소 지도 출력 (위경도 DB로 마커 표시)
<br>
<br>

* 북마크 기능<br>
  <img src="https://user-images.githubusercontent.com/101856058/194008820-0dca930f-a68c-4e18-b904-0e3792efdb15.png" width="45%">
  <img src="https://user-images.githubusercontent.com/101856058/194008916-7c6e158d-d941-4074-a981-7f7677de9443.png" width="45%"><br>
  △ ajax를 이용한 비동기식 북마크 기능 구현 및 DB insert
<br>
<br>

* 이용자 리뷰 및 별점 제공
  ![image](https://user-images.githubusercontent.com/101856058/194010855-65b4e6b2-93c6-4230-87e6-e6fe5901c793.png)
  △ JavaScript function/CSS로 평점 별 개수 동적 변경

<br>
<br>


### ◾ Booking Page (예약 페이지)
  ![image](https://user-images.githubusercontent.com/101856058/194011645-cd13d78b-4704-4750-ab00-7559070f189b.png)
  
* T-DatePicker UI 활용 - 예약이 비어있는 날짜만 선택 및 예약 가능
  ![image](https://user-images.githubusercontent.com/101856058/194011727-b94dd735-0112-404d-a9b6-05127957d986.png)
  △ 검색 기능을 통해 접속한 경우에는 자동 날짜 선택
<br>
<br>

### ◾ My Page
* 내 정보 관리 페이지 - 정보 수정 및 호스트 신청 기능
  ![image](https://user-images.githubusercontent.com/101856058/194015374-3b836b2a-c32b-4774-b0f4-e4d257ed7163.png)
  
<br>
<br>

* 예약 리스트 - 이용 전, 이용 후로 탭 페이지 구현
  ![image](https://user-images.githubusercontent.com/101856058/194014813-e6ebf84b-e6e6-4584-9edf-032d62ddab96.png)
  △ DB의 체크아웃 날짜를 시스템 날짜와 비교하여 가변적 분류 <br>
  △ 완료된 여행의 리뷰가 없는 경우에만 리뷰 버튼 활성화
  
<br>
<br>

* 리뷰 리스트
  ![image](https://user-images.githubusercontent.com/101856058/194015148-12c78c76-d657-47a2-a6a8-7756c9745b1f.png)
  △ 작성한 리뷰, 별점, 사진을 모아보고, 수정 및 삭제가 가능한 페이지

<br>
<br>

* 리뷰 작성 페이지
  ![image](https://user-images.githubusercontent.com/101856058/194021606-1810b44c-a7e3-43fd-9565-fefdd0fa1f70.png)
  ![image](https://user-images.githubusercontent.com/101856058/194021726-0b2aac4c-223b-42b8-b18e-863f35a8e516.png) <br>
  △ 마우스 드래그로 별점 선택 구현
  
<br>
<br>

* 북마크 리스트
  ![image](https://user-images.githubusercontent.com/101856058/194014001-c267744e-b1c6-4dbf-ad65-2f9edd718d6b.png)
  △ 카카오 지도 API 이용 - 북마크한 숙소 위치(위경도 기반) 출력
  
<br>
<br>

* 호스트와 쪽지 기능
  ![image](https://user-images.githubusercontent.com/101856058/194015508-af9cd5f1-137d-4108-904a-82aab2a75eb1.png)
  △ 숙소 상세페이지에서 연락하기 버튼을 눌러 메시지를 보낸 경우, 이곳에 출력 됨
<br>
<br>

### ◾ Host Page
* 예약 관리
  ![image](https://user-images.githubusercontent.com/101856058/194016370-e89bb498-f92a-444b-b0df-4e61d6939db4.png)

<br>

* 리뷰 관리
  ![image](https://user-images.githubusercontent.com/101856058/194016599-6d5c076a-903c-42d2-b338-ab1dcb256b94.png)

<br>

* 숙소 관리
  ![image](https://user-images.githubusercontent.com/101856058/194016946-b52cbd34-3680-41dc-abac-4dbe9c7a6c45.png)

<br>

* 매출 관리
  ![image](https://user-images.githubusercontent.com/101856058/194017080-dac94360-d0c5-4438-befa-8d3b7554f39b.png)
  △ 숙소별 월간 수익 그래프 제공

<br>
<br>

### ◾ Admin Page
* 회원 관리
  ![image](https://user-images.githubusercontent.com/101856058/194017465-f9e8ab7d-7bba-4174-8993-31fce57ad1a0.png)

<br>

* 호스트 관리
  ![image](https://user-images.githubusercontent.com/101856058/194017669-66102cf3-eeff-4c3f-ad75-7f6f637fbc2d.png)

<br>

* 숙소 관리
  ![image](https://user-images.githubusercontent.com/101856058/194017910-1ad42cc2-b533-405a-b37a-9b6057923d7e.png)

<br>
  
### ◾ FAQ, 1:1 Q&A Page
* Float Button 구현
  ![image](https://user-images.githubusercontent.com/101856058/194018109-8b89c799-cc3c-4e5d-8605-fa05f5a51441.png)
  
<br>
<br>

* FAQ
  ![image](https://user-images.githubusercontent.com/101856058/194018274-515c306a-062e-4dc4-9a26-a165b28058ae.png)
  △ click Function을 활용하여, 클릭 시 범위가 밑으로 넓어지며 내용이 출력되도록 구현
  
<br>
<br>

* 1:1 Q&A Page 
  ![image](https://user-images.githubusercontent.com/101856058/194019048-8ea285da-8963-4d9d-8098-512f39098991.png)
  △ 답글형 문의게시판, 비밀글 기능 구현

<br>
<br>
