# Azure 주간 업데이트 요약 - 2026년 09월 21일

## 🤖 AI 및 머신러닝

AI 및 머신러닝 분야에서는 Microsoft Foundry의 에이전트 관리 기능이 정식 지원으로 강화되었고, 네트워크 이그레스 제어 등 보안 중심 기능이 미리 보기로 선보였습니다. Foundry 에이전트를 Microsoft 365 Copilot 및 Teams에 직접 배포할 수 있게 되어 조직이 빠르게 혁신적인 AI 워크플로우를 운영할 수 있습니다. 중앙 집중식 관리와 거버넌스를 바탕으로 에이전트의 활성/비활성 상태를 세밀하게 제어할 수 있으며, 기업 내 컴플라이언스와 보안 요건 충족이 용이해졌습니다. 네트워크 이그레스 제어는 미리 보기로 공개되어 에이전트별 외부 연결 허용/차단 정책을 설계하고 감사할 수 있게 했으며, Foundry Routines 기능은 Logic Apps나 Azure Functions 등 외부 인프라 없이 자체 트리거를 활용한 자동 실행이 가능해 AI 자동화/관찰성이 크게 향상되었습니다. 이러한 업데이트들은 조직이 효율적으로 AI 에이전트의 배포, 실행, 관리 및 거버넌스를 강화할 수 있도록 설계되어, 기술 도입 및 운영의 민첩성을 크게 높입니다.

### [Microsoft Foundry 에이전트 활성/비활성 관리 기능 정식 지원](https://azure.microsoft.com/updates?id=571826)
이제 IT 관리자는 개발자 개입 없이 Admin Center에서 Foundry 에이전트의 활성/비활성 상태를 직접 컨트롤할 수 있습니다. 조직 내 에이전트 환경을 일관되게 관리하며 보안, 컴플라이언스 요구에 부합합니다.

### [Microsoft Foundry 에이전트 Microsoft 365 Copilot 및 Teams 배포 정식 지원](https://azure.microsoft.com/updates?id=571816)
Foundry 에이전트를 Microsoft 365 Copilot과 Teams에 직접 배포해 사용자에게 신속하게 도달하고 중앙 관리 및 거버넌스를 유지할 수 있습니다.

### [Foundry hosted agent 네트워크 이그레스 제어 미리 보기 출시](https://azure.microsoft.com/updates?id=571821)
에이전트별 외부 연결에 대한 허용/차단 규칙을 세분화해 설정할 수 있으며, Responsible AI 정책 기반 동적 감사와 실제 트래픽 분석 모드로 운영 환경 전환이 가능합니다.

---

## 🛠️ 데이터베이스 및 하이브리드/멀티클라우드

데이터베이스 및 하이브리드/멀티클라우드 영역에선 PostgreSQL과 Azure SQL 서비스가 지능적 자동화 및 신뢰성 향상에 중점적으로 확장되고 있습니다. PostgreSQL Flexible Server는 논리 복제 슬롯 동기화 상태 메트릭을 제공해 CDC 연동 시에도 복제 상태를 실시간으로 감시하며, elastic cluster에서 PG18 지원이 정식 제공되어 최신 분산형 데이터베이스 개발이 간편해졌습니다. 신규 가이드 문서는 CPU, 메모리, IOPS 등 상세 성능 이슈 진단 및 해결 프로세스를 지원해 운영 효율성이 증대됐습니다. Azure SQL은 논리 서버 삭제 시 소프트 딜리트 기능이 미리 보기로 도입되어 데이터 관리자의 실수로 인한 데이터 손실 위험을 최소화할 수 있습니다. PostgreSQL 스킬 및 MCP 플러그인은 AI 어시스턴트와 연동해 쿼리 튜닝, 보안, 백업/복구 등 지능적 지원을 제공하며, 실시간 데이터베이스 운영 관찰성에 새로운 시대를 열었습니다.

### [Azure PostgreSQL Flexible Server 논리 복제 슬롯 동기화 상태 메트릭 정식 지원](https://azure.microsoft.com/updates?id=568414)
논리적 복제 슬롯의 동기화 상태를 Azure Monitor에서 실시간 모니터링할 수 있어 CDC 도구 연동 시 일관성과 신뢰성을 확보할 수 있습니다.

### [Azure Database for PostgreSQL elastic cluster PG18 지원 정식 제공](https://azure.microsoft.com/updates?id=571047)
PostgreSQL 18 최신 기능 및 성능 개선을 분산 클러스터 환경에서 사용할 수 있어, 대규모 테이블과 노드에서 효율적 데이터 관리를 지원합니다.

### [PostgreSQL 성능 문제 진단 신규 가이드 출시](https://azure.microsoft.com/updates?id=571042)
CPU, 메모리, IOPS, 임시 파일 등 다양한 성능 이슈에 대해 원인 분석과 해결 방안이 상세하게 안내되는 최신 진단 문서가 제공됩니다.

---

## 🌐 네트워크 및 클라우드 인프라

네트워크 및 클라우드 인프라 영역에서는 대규모 가상 네트워크 메쉬 연결 기능이 Azure Virtual Network Manager에서 정식 지원되어, 최대 3,000개 네트워크를 단일 구성에서 효율적으로 관리할 수 있게 되었습니다. HTTP/3 (QUIC 기반) 지원이 Azure Application Gateway에 미리 보기로 출시되어 웹 및 모바일 환경의 연결 지연을 줄이고, 패킷 손실 복구력을 보강하며 네트워크 성능을 크게 개선합니다. 아울러 Azure Payments HSM v2가 미리 보기로 선보여 PCI DSS와 3DS 등 국제 금융 규정에 부합하는 결제/인증 데이터 보안 및 독립된 단일 테넌트 환경 구성이 가능해졌습니다. 이러한 기능들은 클라우드 네트워크 운영 및 보안, 대규모 서비스 확장, 민첩한 웹 환경 지원 측면에서 획기적 진전을 제공합니다.

### [Azure Virtual Network Manager 대규모 메쉬 연결 정식 지원](https://azure.microsoft.com/updates?id=571572)
최대 3,000 가상 네트워크를 단일 메쉬 구조에서 운영해 대규모 그룹 기반 네트워크 환경을 간소화하고 네트워크 관리를 효율적으로 개선합니다.

### [Azure Application Gateway HTTP/3 over QUIC 지원 미리 보기 출시](https://azure.microsoft.com/updates?id=571123)
HTTP/3 프로토콜 기반의 멀티 스트림 및 패킷 손실 복구 기능으로 최신 웹 서비스와 메시징, 모바일 등에서 네트워크 반응성을 높입니다.

### [Azure Payments HSM v2 미리 보기 출시](https://azure.microsoft.com/updates?id=570509)
PCI DSS, PCI 3DS 등 금융 규제 준수 환경에서 결제/인증 데이터 보호, 단일 테넌트 관리, 감사 및 컴플라이언스 효율성을 크게 강화합니다.

---

## ☁️ 컴퓨트 · 컨테이너 · 가상 데스크톱

컴퓨트 및 컨테이너 분야에서는 SAP용 고성능 메모리 VM(Mdsv4/Msv4 시리즈)이 미리 보기로 공개되어 대규모 엔터프라이즈 워크로드의 효율성을 증대시켰습니다. Azure Red Hat OpenShift에서 Hosted Control Plane 기반 배포 옵션이 미리 보기로 출시되어 완전 관리형 컨트롤플레인의 분리 운영과 워커노드의 유연한 관리가 가능하게 되어 멀티 클러스터 환경에서 클라우드 네이티브 개발과 확장성이 혁신됐습니다. Azure Virtual Desktop에서는 Windows App 클라이언트 측 신규 FQDN 엔드포인트 활용이 발표되어 네트워크 정책과 보안 제어가 보다 효과적이고 안정적으로 적용될 수 있어 기업 환경의 연결 및 장애 대응력이 강화되었습니다.

### [SAP 지원 Mdsv4 / Msv4 시리즈 메모리 최적화 VM 미리 보기 공개](https://azure.microsoft.com/updates?id=571530)
최신 Intel Xeon 기반의 메모리 최적화 VM이 미리 보기로 제공되어 SAP 워크로드에 특화된 성능, 확장성, 신뢰성을 제공합니다.

### [Azure Red Hat OpenShift Hosted Control Plane 미리 보기 출범](https://azure.microsoft.com/updates?id=571621)
클러스터 컨트롤플레인을 완전 관리형으로 운영하고 워커노드 생명주기를 분리 관리하여 운영 유연성과 멀티 클러스터 환경 확장이 가능해집니다.

### [Azure Virtual Desktop 신규 Windows App FQDN 엔드포인트 발표](https://azure.microsoft.com/updates?id=571360)
2026년 10월부터 Windows App 서비스 연결에 신규 FQDN이 도입되며, 네트워크 정책 및 연결 안정성에 대한 사전 대비가 요구됩니다.

---

## 📦 지원 종료 및 중요 알림

운영 환경의 중대한 변경 사항으로 SAP 컨테이너 이미지가 2026년 10월 14일부로 완전히 제거되어 신규 설치, 재배포, 장애 복구가 불가능해지고 반드시 SAP agentless connector로 마이그레이션이 필요합니다. Azure SQL은 논리 서버 소프트 삭제 기능이 미리 보기로 도입되어 삭제된 서버를 지정 기간 내 자체 복구할 수 있게 되어 데이터 보호가 강화되었습니다. PostgreSQL 스킬 및 MCP 플러그인은 AI 어시스턴트 연동을 통해 쿼리 튜닝, 백업/복구, 보안 등 데이터베이스 운영을 더욱 지능적으로 지원하며, 실시간 지식 기반 관리의 새로운 가능성을 열었습니다. 이러한 알림은 업무 연속성과 데이터 보호, 운영 전환 시 반드시 참고해야 하는 필수 가이드입니다.

### [SAP 컨테이너 이미지 2026년 10월 14일부로 제거 및 지원 종료](https://azure.microsoft.com/updates?id=571342)
기존 컨테이너 방식 SAP 연동은 지원 종료되어 신규 설치/재배포가 불가능합니다. 반드시 agentless connector로 마이그레이션해야 합니다.

### [Azure SQL 논리 서버 소프트 삭제 미리 보기 도입](https://azure.microsoft.com/updates?id=571056)
삭제된 Azure SQL 논리 서버를 보존 기간 내에 자체 복구할 수 있어, 관리자의 실수로 인한 데이터 손실을 예방할 수 있습니다.

### [PostgreSQL 스킬 및 MCP 플러그인 미리 보기 출시](https://azure.microsoft.com/updates?id=569664)
AI 어시스턴트와 연동해 PostgreSQL 운영 및 튜닝, 보안, 백업 복구 등 다양한 관리 기능을 데이터베이스 실시간 상황에 맞춰 지능적으로 지원합니다.