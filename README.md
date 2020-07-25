## 1. 프로젝트모임 관리 어플리케이션 

### why?
학교에서 과제나 자발적으로 진행하는 프로젝트들이 많은데 시간관리를 잘하지못해 약속시간이 엉키는 경우가 있습니다.
이런 문제를 방지하기위해 프로젝트 시간관리만을 위한 app 을 개발하였습니다.
프로젝트 간의 빠른 의사결정을 위해 채팅기능, 달력 공유기능만을 타깃으로 개발했습니다.

### 기술요구상항
server 개발자가 없었기 때문에 google 의 firebase 를 기반으로 login authentication 대채
nosql DB 를 이용하여 DB 설계

1. 로그인 가능한 페이지 구현필요합니다.
2. 회원가입 가능한 페이지 구현필요합니다.
3. 채팅방 이름을 입력을 통한 채팅방 검색기능이 필요합니다.
	3.1. 입력한 이름이 존재하지않으면 새로운 채팅방을 만들게 됩니다.
4. 채팅방에서 채팅기능이 있어야 합니다.

5. 현재 자신이 참여하고 있는 팀을 리스트에서 확인가능합니다.
	5.1. 팀 리스트에서 팀이름을 누르면 해당 채팅방으로 이동합니다.
	5.2. 날자에 대해 desecending order 입니다.
	
6. 메인페이지에서는 현재에서부터 일주일 까지의 스케쥴을 확인할 수 있습니다.
	개인 스케쥴에 대해 일주일 까지의 스케쥴을 확인할 수 있습니다.
	팀 스케쥴에 대해 일주일 까지의 스케줄을 확인할 수 있습니다.
7. navigation bar 를 이용하여 User Id 를 확인할 수있습니다. 
또한 메인페이지, 나의 달력, 팀달력, 셋팅으로 이동가능 하며 로그아웃이 가능합니다.
8. 팀 캘린더 메뉴에서 현재 소속된 팀을 확인할 수 있습니다.
9. 팀 캘린더에서 팀의 스케쥴과 개개인의 스케쥴을 확인할 수 있습니다.
	9.1. 팀 캘린더에서 채팅, 일정 투표생성, 진행중인 투표 확인 기능을 선택할 수 있습니다.
	9.2. 팀 캘린더에서 일정조율을 위한 vote 를 생성할 수 있습니다.
		9.2.1 vote 에 모두가 동의하면 스케쥴에 등록됩니다.

## 2. 택시기사님 어플리케이션에 목적지를 무선으로 알려주는 어플리케이션

### why?
여행을 갔을때 자신이 방문하고자하는 위치를 기사님에게 전달하기 어려운 경우가 왕왕있습니다.
이러한 불편함을 해소하기위해서 자신의 핸드폰에서 위치만 선택하면 기사님의 네이게이션을 동작시켜 자동으로 안내를 시작하는 어플을 개발하였습니다.

### 기술요구사항
1. 사용자가 이동하고자하는 위치를 구글 지도에서 선택합니다.
2. 이후 전송버튼 통해 구글 지도상의 위치좌표를 넘겨받아 blue tooth 를 통해 위치 좌료를 기사님 앱으로 전달합니다.
3. 전달된 좌표를 받은 기사님 app 은 해당 좌표를 이미 설치되어있는 네비앱에 전달합니다. 이후, 네비앱을 통해 목적지의 경로를 안내받습니다.
4. 사용자의 app 에서 현재위치에서 목표 위치까지의 거리를 확인할 수 있습니다. ( open api 의 message parsing )
5. 사용자의 app 에서 대략적인 택시요금을 확인할 수 있습니다. ( open api 의 message parsing )



## 3. No-show 고객 관리 site/server

### why?
사회현상으로 no-show 고객으로 인해 피해를 입지않도록 업자들을 보호하기 위한 취지로 개발하였습니다.
target 은 no-show 가 자주 발생하는 미용실 사장님을 대상으로 개발하였습니다.

### 기술적인 요구사항.
1. 고객의 예약을 처리하는 spring 기반 rest api (CRUD)를 이용하여 고객의 예약 및 no-show 고객을 관리합니다.
2. 미용실 홓보용 페이지를 instagram open api 를 이용하여 instagram 의 사진들을 페이지에 노출합니다.
3. 고객의 예약을 받기위해 핸드폰 번호 입력과 시간 버튼으로 이루어진 inter active 가능한 web page 를 구현합니다.
	3.1. 핸드폰 번호 입력후 시간이 입력되어있는 버튼을 누르면 ajax 를 통해 서버에 예약 요청합니다.
4. 고객의 no-show count 를 기록 및 차단을 위한 db 및 spring 서버 로직 구현 합니다.


## 4. Homecarekit을 활용한 독거노인 

### why?
독거노인 분들이 열악한 환경에서 생활하는 현실의 문제에 대해 원격으로 케어링을 받을 수 있는 방법을 고안하기 위한 취지로 개발하였습니다.
원격 케어링 방법으로 독거노인분의 맥박에 대한 실시간 상황을 사회복지사분을 어플을 통해 확인받을 수 있도록 하였습니다.

### 기술요구사항.
1. 맥박측정 시계를 통해 독거노인분의 맥박데이터가 지속적으로 노인분의 스마트폰으로 전송이됩니다.
2. 노인분의 스마트폰앱을 통해 서버상으로 맥박데이터를 전송하여 노인부의 상태를 기록합니다.
3. 사회복자사앱은 사회복지사만 접속을 하기위해 로그인기능이 필요합니다.
4. 사회복지사앱은 사회복지사가 관리하는 노인분들을 리스트를 확인할 수 있습니다.
4. 리스트중 하나를 선택하게 되면, 맥박데이터를 이용해 그려진 그래프로 노인분의 상태를 확인할 수 있습니다.

*****

## 4. 현재 사용하고있는 기술.
임베디드 미디어 서버의 이슈 트래킹 및 web 에서 미디어 스트리밍을 통해 재생되고 있는 컨텐츠를 제어하기 위한 api 를 구현을 담당하고 있습니다.

1. gstreamer 를 이용하기 위한 media pipeline 을 설정하는 서버의 이슈 트래킹
2. subtitle engine 의 이슈 트래킹
3. web app 에서 보드의 media 를 control 하는데 필요한 api 를 c/c++ 로 구현. 
	3.1. play/seek/pause/get subtitle info/ get video info 등등..








