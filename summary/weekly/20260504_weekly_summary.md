# Azure 주간 업데이트 요약 - 2026년 05월 04일

## 🧠 인공지능 및 Microsoft Foundry

이번 주 인공지능 및 Microsoft Foundry 분야에서는 기업 환경에서의 AI 통합 및 에이전트 개발 효율성이 크게 향상된 것이 특징입니다. Foundry Agent Service의 자체 AI Gateway 연동을 통해 기업 보안 정책 하에서도 외부·사내·오픈소스 모델을 손쉽게 통합할 수 있게 되었습니다. Microsoft Agent Framework 1.0의 공식 정식 지원은 .NET 및 Python 개발자 모두에게 장기적 안정성과 다양한 환경과의 상호운용성을 보장, 에이전트 기반 아키텍처의 확장 가능성을 높였습니다. 아울러, 내장 메모리 기능 미리 보기가 공개됨으로써 별도의 데이터베이스 구축이나 운영 없이 장기 기억 기반 에이전트가 보다 쉽게 구현될 전망입니다. 이러한 업데이트들은 데이터 보호, 프로바이더 분산, 멀티-에이전트 관리 등 최신 기업 AI 요구에 신속히 대응할 수 있도록 해줍니다.

### [정식 지원] Foundry Agent Service의 BYO AI Gateway 기능 도입  
이제 Foundry Agent Service가 자체 또는 외부 AI Gateway 모델 연동을 지원, 오픈소스·서드파티 모델 활용 시에도 엔터프라이즈 규정과 거버넌스를 완벽히 적용할 수 있습니다.  
https://azure.microsoft.com/updates?id=561002

### [정식 지원] Microsoft Agent Framework 1.0 공식 출시  
Agent Framework 1.0 버전이 안정적 API와 함께 정식 지원됩니다. .NET 및 Python 환경에서 멀티 에이전트 오케스트레이션, 다양한 AI 프로바이더 연계 등 유연한 통합이 강점입니다.  
https://azure.microsoft.com/updates?id=560982

### [미리 보기] Foundry Agent Service 내장 메모리 기능  
Foundry Agent Service에 장기 메모리 관리 기능이 미리 보기로 추가되어, 외부 DB 구축 없이도 에이전트의 기억력 기능을 간결하게 제공합니다.  
https://azure.microsoft.com/updates?id=560992

---

## 💾 스토리지 및 데이터 관리

스토리지 및 데이터 관리 영역에서는 데이터 접근 제어 및 운영 자동화 관련 정식 지원이 두드러집니다. Elastic SAN의 Windows VM 연동 자동화로 초기 인프라 배포 후 수작업 없는 운영이 가능해졌고, User Delegation SAS에 Prefix 범위 접근 지원이 추가되어 컨테이너 내부의 하위 경로 또는 디렉터리별 데이터 권한 분리가 효율적으로 이뤄집니다. 영국 지역에서는 Azure 외부 데이터 전송 정책이 변경되어, 데이터 이관 시 크레딧 신청 등 관련 프로세스 준수가 중요해졌습니다. 이러한 변화는 기업의 데이터 보안 체계, 분산 자원 및 복잡한 거버넌스 환경에서 실질적 관리 편의를 크게 높여줍니다.

### [정식 지원] Windows VM에서 Elastic SAN 볼륨 연동 자동화  
Elastic SAN 볼륨을 VM 확장 프로그램을 통해 Azure Portal에서 자동 연동할 수 있어, 수동 구성 부담을 해소합니다.  
https://azure.microsoft.com/updates?id=560914

### [정식 지원] User Delegation SAS의 Prefix 범위 접근 지원  
Blob Storage의 SAS 발급 정책에 디렉터리·경로(Prefix) 단위 접근제어가 추가되어 더 세분화된 데이터 보안정책을 적용할 수 있습니다.  
https://azure.microsoft.com/updates?id=561257

### [정식 지원] 영국 내 Azure에서 Egress 및 데이터 전송 정책 변경  
영국 지역에서 Azure 외부로의 데이터 전송 정책이 변경되며, 크레딧 신청 절차 등 세부 준수 사항이 생겼으니 유의해야 합니다.  
https://azure.microsoft.com/updates?id=561392

---

## 🌐 네트워킹 및 보안

이번 주에는 글로벌 네트워크 관리와 보안성을 높이는 주요 신기능이 출시되었습니다. Azure Virtual Network Manager에서는 크로스리전 IPAM Pool 연동을 통해 여러 리전에 걸친 네트워크 자원을 단일 정책으로 관리할 수 있게 되어 전략적 주소 체계 통제가 한층 용이해졌습니다. 또한 Azure WAF용 HTTP DDoS 규칙셋 미리 보기가 제공되어 프론트 도어 기반의 레이어7 공격 차단이 자동화되었으며, AKS용 Container Network Insights Agent 출시로 네트워크 인사이트 통합진단을 실시간으로 할 수 있게 되었습니다. 이러한 도입은 분산 클라우드 환경에서의 운영 효율성, 보안 위협 대응력, 장애 진단 시간을 한층 단축시켜줍니다.

### [정식 지원] Azure Virtual Network Manager에서 크로스리전 IPAM Pool 연동  
여러 리전에 걸쳐 단일 IPAM 풀을 연동해, 글로벌 네트워크 주소 및 거버넌스 정책을 일원화할 수 있습니다.  
https://azure.microsoft.com/updates?id=561067

### [미리 보기] Azure WAF용 HTTP DDoS 규칙셋(Azure Front Door Premium)  
신규 HTTP DDoS 자동방어 규칙셋으로 AI기반 트래픽 감지와 실시간 차단, 클라이언트별 베이스라인 적용이 가능해졌습니다.  
https://azure.microsoft.com/updates?id=561148

### [정식 지원] AKS Container Network Insights Agent 출시  
웹 기반 인텔리전스 도구로 AKS 클러스터의 네트워크 문제를 자연어로 신속 진단하며, 장애 원인분석이 훨씬 쉬워집니다.  
https://azure.microsoft.com/updates?id=561020

---

## 🧩 컨테이너·오픈소스·컴퓨트

컨테이너 및 오픈소스, 컴퓨트 분야는 유럽 데이터 국지성 강화와 개발 옵션 확장에 초점이 맞춰졌습니다. 오스트리아 동부 리전에서 Azure Red Hat OpenShift가 정식 지원되어, EU 규제 및 각국 법령을 중시하는 기업들이 리전 내에 데이터를 안전하게 보관할 수 있습니다. Azure Functions에서 Java 25 지원도 정식 출시되어, 최신 Java 기반 서버리스 앱을 리눅스·윈도우·플렉스 소비 요금제 등 다양한 환경에 배포할 수 있게 되었습니다. AKS용 네트워크 인사이트 에이전트 도입으로 컨테이너 인프라의 네트워크 문제를 보다 신속히 해결할 수 있습니다.

### [정식 지원] 오스트리아 동부 리전에서 Azure Red Hat OpenShift 지원  
EU·오스트리아 데이터 국지성 및 공공/규제산업 고객 요구에 부응, 유럽 내 클라우드 채택이 한층 확대됩니다.  
https://azure.microsoft.com/updates?id=561135

### [정식 지원] Azure Functions Java 25 지원 시작  
최신 Java 25로 Function 앱 개발 및 폭넓은 배포가 가능, 오픈소스 개발 생태계에 강력한 지원을 제공합니다.  
https://azure.microsoft.com/updates?id=560879

### [정식 지원] AKS용 Container Network Insights Agent 출시  
AKS 내 컨테이너 네트워크 문제 탐지·원인 분석을 위한 실시간 인사이트를 제공, 운영 효율화에 기여합니다.  
https://azure.microsoft.com/updates?id=561020

---

## 🛑 기능 지원 종료 및 변경

서비스 수명주기 변화에 따라 Prompt Flow 등 일부 기능의 단계적 지원 종료가 예고되었습니다. Prompt Flow는 2027년 4월 전면 지원 종료가 확정, Microsoft Agent Framework로의 전환이 권고됩니다. 이에 따라 기존 워크로드, 코드 및 운영환경의 조기 마이그레이션 계획 수립과 테스트가 필수적입니다. 조기 이전 시 최신 Foundry 및 에이전트 기반 아키텍처 기능, 신뢰성, 장기지원을 신속히 활용할 수 있으니, 조직 내 적용 가이드 및 기술 매핑 준비가 필요합니다.

### [지원 종료] Prompt Flow 서비스, 2027년 4월 전면 중단 안내  
Prompt Flow가 2027년 4월 20일부로 Microsoft Foundry, Azure ML, VS Code에서 모두 지원 종료되며, Microsoft Agent Framework로의 이관이 필수입니다.  
https://azure.microsoft.com/updates?id=502936