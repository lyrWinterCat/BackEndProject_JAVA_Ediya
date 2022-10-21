# BackEndProject_JAVA_Ediya
## EDIYA KIOSK & POS-Machine 프로그램 제작

### 주제 선정

코리아 IT 아카데미 웹앱개발 2 (JAVA) 수강 후 배운 기술을 활용하여 주제를 선정하고자 했다.

카카오톡 PC버전 구현, 영화 예매 프로그램 , 미니게임 모음, 카페 메뉴(키오스크), 포스기 프로그램(카페, 마트, 편의점 등) 이라는 의견이 제시되었다.

투표를 통해 포스기 프로그램이 선정되었고, 조원들과 의견을 나누어 본 결과 키오스크 및 포스기 통합 프로그램을 제작하게 되었다.

### 역할 분배

메인 화면(프로모션 이미지, 고객/관리자 로그인 기능), 키오스크 프로그램 (구매 페이지 구현)
- 이예림

포스기 프로그램 (재고 관리 페이지 구현)
- 임성은

포스기 프로그램 (판매,지출액 관리 페이지 구현)
- 오연호

### 프로젝트 목표

- JAVA만을 사용하여 포스기 프로그램 구현
- 최대한 강의 내용을 활용하여 제작
- 부족한 부분은 스스로 공부하기

### 프로젝트 기획

![기획.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/656ad284-3643-404f-96bf-ac3163e979ca/%EA%B8%B0%ED%9A%8D.png)

### 개발 환경

언어 : JAVA 

툴 : Eclipse

### 코드 참고 및 프로젝트 최종 파일

[https://github.com/lyrWinterCat/BackEndProject_JAVA_Ediya](https://github.com/lyrWinterCat/BackEndProject_JAVA_Ediya)

## 1. 메인 페이지 - 이예림

### 프로모션 이미지 구현 , 메인 화면 프레임 구현

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/42cbe284-0154-4ab9-937d-809b6a4c0d60/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/2e5b324c-205c-4a9e-9ee1-2f9fe86477fc/Untitled.png)

- 프로그램 실행 시 1초마다 화면이 바뀌며 3장의 프로모션 이미지가 나타난다.
- 이미지를 클릭하면 제품 구매 / 관리자 선택 화면으로 이동한다.
- 제품 구매 버튼 클릭 시 물건을 주문할 수 있는 키오스크 창으로, 관리자 버튼 클릭 시 로그인 화면이 나오며 맞는 암호를 입력하면 포스기 프로그램의 재고 관리 및 매출 관리 페이지로 이동한다.

## 2. 제품 구매 페이지 - 이예림

### 상품 선택, 옵션 선택, 장바구니 담기, 비우기, 주문하기 페이지

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/1cdf3ac1-6057-41d3-924f-b8ca0fb4d4a3/Untitled.png)

![orderImage.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/8cba30fc-3ffc-4479-9384-0f971b5959ec/orderImage.png)

- 메뉴 사진을 클릭하면 해당 메뉴에 맞는 옵션 선택 버튼이 활성화된다.
- 모든 옵션은 중복체크가 불가능한 라디오 버튼으로 구현하였다.
- 옵션을 체크하지 않고 장바구니에 담으려고 시도할 경우 알림창이 나오며 장바구니에 담을 수 없다.
- 상품과 옵션을 알맞게 선택하고 장바구니에 담으면 오른쪽 하단 장바구니 구역에 메뉴가 나타난다.
- 장바구니에 메뉴가 있고, 주문하기를 클릭했을 때 해당 메뉴의 재고가 부족하다면 경고창이 나오며 주문이 취소된다.
- 장바구니에 이미 있는 상품과 같은 상품,옵션으로 장바구니에 추가 할 경우, 메뉴가 늘어나지 않고 수량만 증가한다.
- 주문이 성공한다면 주문 내역 알림창이 나오며, 해당 페이지에는 주문한 메뉴명, 수량, 옵션 및 가격이 표기된다. 페이지 하단에는 대기번호와 총 결제 금액을 확인할 수 있다.

## 3. 관리자 페이지

## 포스기 프로그램 메인 페이지 - 이예림

### 관리자 모드 로그인 페이지

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/125dd45c-c821-492a-ad57-cf170937247a/Untitled.png)

- 관리자 버튼 클릭시 들어오는 화면
- 프로그램 구현시 설정한 비밀번호를 입력하면 매출관리, 재고관리 버튼이 활성화된다.
- 틀린 비밀번호를 입력하면 비밀번호가 맞지 않는다는 알림창이 나온다.
- 기획 단계에서는 비밀번호 설정과 비밀번호 찾기 기능을 구현하고자 하였으나 시간상의 문제로 완성하지 못했다. 이번 프로젝트의 아쉬운 부분 중 하나이며 차후 프로젝트에서 로그인 기능 구현을 담당한 계기가 되었다.

## 재고 관리 페이지 - 임성은

### 구매 페이지와 연동하여 재고 관리 페이지 구현

![storage.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/723b457b-a68c-482d-aa10-d0b66cdf3027/storage.png)

- 구매 화면에서 제품 주문하기에 성공하면 해당 상품의 재고가 줄어든다.
- 화면 상단의 버튼을 클릭하면 버튼에 맞는 상품의 재고가 출력된다.
- 버튼과 옵션을 통해 부족한 재고를 구매할 수 있다.

## 매출 관리 페이지 - 오연호

### 구매 페이지, 재고 페이지와 연동하여 매출 관리 페이지 구현

![accountAdmin.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/246665fe-ffd7-47c6-acc9-6f6ae45be4e9/accountAdmin.png)

![sellProduct.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/4ef76a74-2874-41f0-88dc-d70d29b46188/sellProduct.png)

![sellGraph.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/46fdde71-4cf3-4dfc-87d3-5676e0412141/sellGraph.png)

![sellCalendar.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c9b26f97-89a3-4d45-b851-7e5ad027cc93/sellCalendar.png)

![spendMoney.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a8f12cb3-d56a-4d4a-85e4-7f83a9e06267/spendMoney.png)

- 매출 관리 페이지로 들어가면 버튼에 따라 당일 매출, 월별 판매액, 총 지출액을 확인 및 입력할 수 있다.
- 당일 매출은 구매 페이지와 연동되어 주문 성공한 제품들의 수량과 가격이 표기되며, 즉시 확인이 가능하다. 그래프로 어떤 상품이 얼마나 팔렸는지도 확인할 수 있다.
- 총 판매액은 월 별로 판매액을 작성할 수 있으며, 당일 판매액은 자동으로 연동된다.

## 프로젝트 후기

코리아 IT 아카데미 웹앱개발 2 JAVA 강의를 마치고, 해당 강의에서 자세히 다루지 못한 부분을 직접 써보고 구현하며 배울 수 있었던 프로젝트였다. 프로그래밍 공부를 시작하고 처음으로 참여한 팀 프로젝트였으며, 팀 리더를 맡게 되어 부담감도 상당했다. 그러나 조원들과 함께 의견을 모아서 기획을 하고, 개발을 하는 모든 순간들이 즐거웠으며 많은 것을 배울 수 있었던 시간이었다.

JAVA만을 사용한 단순 프로젝트였던 만큼 처음 기획과 틀어진 부분도, 원하는 기능을 충분히 구현하지 못해 아쉬운 부분도 있었지만 이번 기회를 통해 JAVA라는 언어를 더욱 깊게 이해하고 활용할 수 있었다.

이번 프로젝트를 통해 팀 프로젝트의 가장 기본적인 부분을 깨달을 수 있었다. 프로젝트 기획 단계에서 공통 변수 및 클래스를 어떻게 설정할 것이며, 표기법 통일과 같은 세부적인 틀을 잡지 않아 프로젝트 후반으로 가면서 객체 공유가 어려웠고, 팀원 간의 코드 병합시 일어나는 충돌 문제로 많은 에러를 해결해야만 했다. 이러한 경험을 토대로 팀 프로젝트에서 가장 중요한 부분이 기획 및 개발환경설정이라는 것을 알 수 있었다. 

100시간의 강의보다 한 시간의 코딩이 낫다는 말이 있다. 한 달 동안 JAVA에 대해 많은 것을 배웠고, 배운 기술들을 토대로 직접 프로젝트를 진행해 보면서 한 단계 위로 성장할 수 있었던 프로젝트였다.
