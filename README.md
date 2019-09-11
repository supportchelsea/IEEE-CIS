# IEEE-CIS

## Data Definition

**- Transaction Table**

TransactionDT : 주어진 참조 날짜 시간의 타임 델타 (실제 타임 스탬프 아님)
TransactionAMT : 거래 결제 금액 (USD)
ProductCD : 제품 코드, 각 거래에 대한 제품
card1-card6 : 카드 유형, 카드 카테고리, 발행 은행, 국가 등과 같은 지불 카드 정보
addr : 주소
dist : 거리
P_ and (R__) emaildomain : 구매자 및 수신자 이메일 도메인
C1-C14 : 지불 카드와 관련된 주소 수 등의 계산. 실제 의미는 숨겨져 있습니다.
D1-D15 : 이전 거래 간의 날짜 등과 같은 타임 델타
M1-M9 : 카드 이름 및 주소 등 일치
Vxxx : Vesta는 순위, 계산 및 기타 엔티티 관계를 포함한 다양한 기능을 엔지니어링했습니다.

범주 Features :
ProductCD
card1 - card6
addr1, addr2
Pemaildomain Remaildomain
M1 - M9

**- Identity Table**

이 표의 변수는 거래와 관련된 신원 정보 – 네트워크 연결 정보 (IP, ISP, 프록시 등) 및 디지털 서명 (UA / browser / OS / version 등)입니다.
Vesta의 사기 방지 시스템과 디지털 보안 파트너가 수집합니다.
(필드 이름은 마스킹되며 개인 정보 보호 및 계약 계약을 위해 쌍별 사전은 제공되지 않습니다)

범주 Features :
DeviceType
DeviceInfo
id 12-id 38
