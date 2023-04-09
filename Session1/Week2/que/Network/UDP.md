# UDP
- - -

    사용자 데이터그램 프로토콜(UDP)은 통신 프로토콜로, 특히 비디오 재생 또는 DNS 조회와 같이 시간에 민감한 전송을 위해 인터넷을 통해 사용됩니다. 
    이 프로토콜의 경우 데이터가 전송되기 전에는 공식적으로 연결이 설정되지 않으므로 통신 속도가 빨라집니다. 
    따라서 데이터를 아주 빠르게 전송할 수 있지만, 전송 중에 패킷이 손실되어 DDoS 공격의 형태로 악용될 수 있습니다.

## UDP 동작 원리

<img width="800" src="https://www.cloudflare.com/img/learning/ddos/glossary/user-datagram-protocol-udp/tcp-vs-udp.svg">


    모든 네트워킹 프로토콜과 마찬가지로 UDP는 네트워크의 두 컴퓨터 간에 데이터를 전송하기 위한 표준화된 방법입니다. 
    다른 프로토콜과 비교하여 UDP는 먼저 연결을 설정하거나, 해당 패킷의 순서를 표시하거나, 의도한 대로 도착했는지 여부를 확인하지 않고 
    패킷(데이터 전송 단위)을 대상 컴퓨터로 직접 보내는 간단한 방식으로 이 프로세스를 수행합니다. (UDP 패킷을 '데이터그램'이라고 합니다.)

    UDP는 또 하나의 일반적인 전송 프로토콜인 TCP보다 빠르지만, 안정성이 떨어집니다. 
    TCP 통신에서 두 컴퓨터는 '핸드셰이크'라는 자동화된 프로세스를 통해 연결을 설정하는 것으로 시작합니다. 
    이 핸드셰이크가 완료된 후에만 실제로 데이터 패킷이 한 컴퓨터에서 다른 컴퓨터로 전송됩니다.

    UDP 통신은 이 프로세스를 거치지 않습니다. 대신 한 컴퓨터에서 단순히 다른 컴퓨터로 데이터를 보내기 시작할 수 있습니다.
    또한 TCP 통신은 데이터 패킷이 수신되어야 하는 순서를 나타내고 패킷이 의도한 대로 도착하는지 확인합니다. 패킷이 도착하지 않는 경우(예: 중간 네트워크의 혼잡으로 인해) TCP를 다시 보내야 합니다. UDP 통신에는 이 기능이 포함되어 있지 않습니다.

    이러한 차이 때문에 몇 가지 이점이 생깁니다. UDP는 '핸드셰이크'가 필요하지 않거나 데이터가 제대로 도착하는지 확인하지 않기 때문에 TCP보다 훨씬 빠르게 데이터를 전송할 수 있습니다.

## Reference

https://www.cloudflare.com/ko-kr/learning/ddos/glossary/user-datagram-protocol-udp/