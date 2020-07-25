3. No-show 고객 관리 site/server

why?
사회현상으로 no-show 고객으로 인해 피해를 입지않도록 업자들을 보호하기 위한 취지로 개발하였습니다.
target 은 no-show 가 자주 발생하는 미용실 사장님을 대상으로 개발하였습니다.

기술적인 요구사항.
1. 고객의 예약을 처리하는 spring 기반 rest api (CRUD)를 이용하여 고객의 예약 및 no-show 고객을 관리합니다.
2. 미용실 홓보용 페이지를 instagram open api 를 이용하여 instagram 의 사진들을 페이지에 노출합니다.
3. 고객의 예약을 받기위해 핸드폰 번호 입력과 시간 버튼으로 이루어진 inter active 가능한 web page 를 구현합니다.
	3.1. 핸드폰 번호 입력후 시간이 입력되어있는 버튼을 누르면 ajax 를 통해 서버에 예약 요청합니다.
4. 고객의 no-show count 를 기록 및 차단을 위한 db 및 spring 서버 로직 구현 합니다.


