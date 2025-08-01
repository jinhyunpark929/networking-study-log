# 🌐 네트워크 & 인터넷 기초 개념

## 📡 네트워크란?

- **정의:** 두 대 이상의 장치(예: PC, 스마트폰, 라우터 등)가 물리적 또는 무선 방식으로 연결된 통신망
- **목적:** 데이터를 효율적으로 **공유**하고, 장치 간 **통신**이 가능하도록 함

## 🌍 인터넷이란?

- **정의:** 전 세계에 존재하는 수많은 네트워크들이 연결되어 만들어진 **가장 거대한 네트워크**
- 지역망(LAN), 도시망(MAN), 광역망(WAN) 등이 연결되어 구성됨

---

## 🧩 네트워크 구성 요소

### NIC (Network Interface Card)

- **역할:** 컴퓨터와 네트워크 간 물리적인 연결을 담당하는 장치
- **기능:**
  - 데이터를 송수신하고 신호를 변환함 (유선/무선)
  - 고유한 MAC 주소를 가짐
  - 이더넷, Wi-Fi 등 다양한 네트워크 프로토콜 지원

### 노드, 호스트, 서버

- **노드(Node):** 네트워크에 연결된 모든 장치 (예: 컴퓨터, 라우터, 스위치 등)
- **호스트(Host):** IP 주소를 가지고 데이터를 송수신할 수 있는 장치
- **서버(Server):** 클라이언트에게 웹, 파일, DB 등 서비스를 제공하는 호스트
- **클라이언트(Client):** 서버로부터 데이터를 요청하고 사용하는 장치

---

## 🕸️ 네트워크 유형

| 유형 | 설명 |
|------|------|
| **LAN** (근거리 통신망) | 학교, 사무실 등 제한된 공간 내의 네트워크 |
| **MAN** (도시 통신망) | 도시 수준의 중간 규모 네트워크 |
| **WAN** (광역 통신망) | 국가 또는 대륙 단위의 대규모 네트워크. 대표적으로 **인터넷** |

> 📌 실무에서는 LAN과 WAN이 가장 널리 사용됨

---

## 🔌 케이블 & 프로토콜

### 네트워크 프로토콜이란?

> 네트워크에서 데이터를 주고받기 위한 **약속된 규칙(통신 규약)**

- **이더넷(Ethernet):** 근거리 통신 시 데이터 전송
- **IP:** 컴퓨터 간 주소 지정 및 데이터 경로 설정
- **TCP/UDP:** 특정 응용 프로그램에 신뢰성 있게 데이터를 전달

### 표준 기반 모델 (Standards-Based Model)

- **특징:**
  - **멀티 벤더 호환**: 다양한 제조사의 장비/소프트웨어 간 상호운용 가능
  - **계층적 구조**: 기능을 분리하여 관리하고 독립적으로 동작함
- **장점:** 유연성, 확장성, 호환성 우수
- **단점:** 설정 복잡, 통합 관리 어려움
- **의미:** 폐쇄형 시스템에서 개방형 표준 구조로 진화하면서 기술 통합이 가능해짐

---

## 🕸️ 웹 서비스와 네트워크

- **웹 서비스:** 웹 브라우저(클라이언트)가 **웹 서버**로부터 데이터를 요청하고 응답을 받는 서비스  
- 웹 서버는 HTTP 요청을 처리하며, 동적 콘텐츠의 경우 내부적으로 **WAS(Web Application Server)** 와 연동  
- 즉, 웹 서버는 정적/동적 자원을 클라이언트에 전달하는 **서버 호스트**의 일종

---

## 🛰️ 데이터 전송 경로 예시 (Traceroute)

`tracert` 명령어를 사용하면 데이터가 목적지(예: www.google.com)에 도달하는 동안 거치는 라우터 경로(Hop)를 확인할 수 있습니다.

<img width="1059" height="486" alt="스크린샷 2025-07-15 112754" src="https://github.com/user-attachments/assets/ffcd7daa-eabe-4028-84db-a17683eca70a" />

- `172.30.1.254`: 가장 가까운 라우터 (게이트웨이)
- 중간의 여러 통신사 라우터를 거쳐 Google 서버(142.250.206.228)에 도달
- `*`: 응답이 없거나 방화벽 등으로 차단된 구간

> 이처럼 각 구간의 지연 시간(ms)을 확인해 네트워크 상태나 병목을 진단할 수 있습니다.

---

## 🎮 게임으로 이해하는 네트워크

- **LAN 기반 게임:** **혼자 플레이하는 솔로 게임** – 외부 네트워크 연결 없이 실행  
- **WAN 기반 게임:** **온라인 멀티플레이 게임** – 인터넷을 통해 여러 사람과 연결

---
