![bluetooth low energy stack](/bt_source/bluetooth_LE_stack.png "ble stack")

| layer | Key Responsibilites |
| --- | --- |
| Physical layer | 변조 방식, 주파수 대역, 채널 사용, 송신기 및 수신기 특성을 포함하여 라디오(RF)의 사용과 관련된 블루투스 기술의 모든 측면을 정의합니다. 물리 계층 파라미터들의 몇 가지 구별되고 지원되는 조합들이 정의되고 PHY로 지칭됩니다.|
| Link layer | 공중 인터페이스 패킷 형식, 오류 검사와 같은 비트 스트림 처리 절차, 상태 기계 및 공중 통신 및 링크 제어를 위한 프로토콜을 정의합니다. 논리 전송으로 알려진 무연결, 연결 지향 및 등시성 통신을 위해 기본 라디오를 사용하는 몇 가지 고유한 방법을 정의합니다. |
| Isochronous Adaptation Layer (ISOAL) | 등시성(일정한 시간간격) 통신을 사용하는 장치에서 서로 다른 프레임 기간을 사용할 수 있도록 합니다. 프레임된 PDU의 분할 및 재조립 또는 프레임되지 않은 PDU의 분할 및 재조합을 수행합니다.|
| Host Controller Interface (HCI) | 호스트 구성 요소(컴포넌트)와 컨트롤러 간의 명령 및 데이터의 양방향 통신을 위한 잘 정의된 기능 인터페이스를 제공합니다. 여러 물리적 전송 구현 중 하나에 의해 지원됩니다. |
| Logical Link Control and Adaptation Protocol (L2CAP) | 호스트 내에서 프로토콜 멀티플렉서 역할을 수행하여 프로토콜이 적절한 호스트 컴포넌트에 의해 서비스되도록 보장합니다. 아래 계층과 L2CAP 위 계층 사이에서 PDU/SDU의 세그먼트화 및 재조립을 수행합니다. |
| Security Manager Protocol (SMP) | 페어링과 같은 보안 절차를 실행하는 동안 사용되는 프로토콜입니다. |
| Attribute Protocol (ATT) |  서버의 속성 테이블에서 데이터를 검색하고 사용할 수 있는 ATT 클라이언트 및 ATT 서버에서 사용하는 프로토콜입니다. |
| Generic Attribute Profile (GATT) | 속성 테이블의 기본 속성에 대해 서비스, 특성 및 기술자로 알려진 상위 수준의 데이터 유형을 정의합니다. 속성 테이블을 작업하기 위해 ATT를 사용하는 상위 수준의 절차를 정의합니다. |
| Generic Access Profile (GAP) | 무연결 통신을 위한 광고 사용 방법, 기기 탐색 수행 방법 등 비연결 상태일 때 사용할 수 있는 운영 모드 및 절차를 정의합니다. 보안 수준 및 모드를 정의합니다. 일부 사용자 인터페이스 표준을 정의합니다. |
