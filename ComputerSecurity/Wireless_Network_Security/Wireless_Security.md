wired인 유선 네트워크보다 보안상의 허점이 많음

일단 선이 없음.
broadcast fast로 데이터를 전송함. 그러니까 훨씬 더 도청이나 jamming 정보의 변조 등에 susceptible 민감하다.

active attack
communication protocol에 있어서 유선네트워크에 비해 open되어 있기 때문에 취약하다

mobility
이동성이 하나의 장점이 될 수 있지만 (portable, mobile) 이 때문에 보안상의 문제점이 생길수 있음

자원
스마트폰 같은 wireless장비들이 작기 때문에 메모리나 프로세스리소스 등이 상당히 제약적임. 자원이 작기 때문에 외부공격에 의한 자원 고갈이 더 쉬움.
sensor나 robot과 같은 hostile한 위치에 있음.

접근성의 문제점


이와 같은 Wireless Transmission을 어떻게 보호할 수 있는가?
================
가장 위협적인 공격은 eavesdropping도청
altering or inserting messages 아니면 파괴disruption

도청을 어떻게 방지할 수 있는가 2가지 방법 제시

Signal-hiding techniques
----------------
signal을 숨기는. 호텔이나 워크샵할 때 어떤 기관을 가면 SSID를 줌(와이파이 이름같은)
해당 AP(Access Point)내에서 제공해주는 서비스를 제공받을 수 있는 id임.
SSID = service set identifier
wireless access point에 의해서 broadcast가 발송되어지면 그걸 갖다가 패스워드를 등록해서 쓸 수 있음
=> 그걸 아예 꺼버려라. SSID자체를 알려주지 않는 방법

SSID에 cryptic name을 주는 것
수수께끼같은, 아리송한 애매모호한 이름을 assign

power를 아주 낮게 해서 밖으로는 신호가 못나가게끔. 특정 공간에서만 쓸수 있도록 (coverage를 제한)

대부분은 access point를 가능한한 interior center (벽이나 창문처럼 가장자리가 아닌 내부의 중앙에) 설치해서 최대한 밖으로 나가는걸 제지.

Encryption
-----------------
effective한 방법

Securing Wireless Access Points
============================
네트워크에 대한 승인받지 않은, 허가받지 않은 접근이 main threat임.
결국은 인증을 받아야함
그런 인증받는 access control 부분을 표준에서는 아래와 같이 정의
IEEE 802.1X 표준에서 port-based network access Network(포트기반 액세스 제어)

IEEE는 학회이름! 표준이 현재 23번인가 24번까지(?) 이뤄지고 있음.
그중에서 802.1은 internetworking과 관계되어진 표준들 정의하고 있음.
802.1d 가 MAC bridge(두개의 lan을 연결하는데 쓰이는 장비)
802.1q 는 VLAN(Virtual LAN 물리적으로 같이 있지는 않지만 소프트웨어적으로 마치 같은 네트워크인양
  broadcast가능함)
802.1x 는 Wireless lan에서의 외부로부터 들어오는 사용자들에 대해 port기반으로 인증을 제공해주는
802.11이 조금은 죽었지만 상당히 활발히 이루어지는 표준임.
rogue악한 목적을 가진 access point를 방지하고 다른 unauthorized device가 하나의 안전하지 않은 backdoor가 되는 것을 막는다.  

router의 identifier default값을 변경해준다
router에 preset되어 있는 admin password를 qkRnjwnsek
