1. 프로젝트모임 관리 어플리케이션 

why?
학교에서 과제나 자발적으로 진행하는 프로젝트들이 많은데 시간관리를 잘하지못해 약속시간이 엉키는 경우가 있습니다.
이런 문제를 방지하기위해 프로젝트 시간관리만을 위한 app 을 개발하였습니다.
프로젝트 간의 빠른 의사결정을 위해 채팅기능, 달력 공유기능만을 타깃으로 개발했습니다.

기술요구상항
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

