# Azure 주간 업데이트 요약 - 2026년 06월 08일

## 🤖 AI 및 머신러닝 (Microsoft Foundry 포함)

AI 및 머신러닝 분야에서는 Microsoft Foundry를 비롯한 엔터프라이즈 AI 혁신이 중심이었습니다. 대형 언어 모델(LLM) 기반 번역, 음성/이미지 합성, 콘텐츠 이해, RAG 파이프라인, 프라이버시 자동화, 엔터프라이즈 데이터 활용 등 실서비스 수준의 기능이 광범위하게 정식 지원(GA) 또는 미리 보기(preview)로 확대되었습니다. 특히, Microsoft Foundry 플랫폼의 글로벌 PTU 예약 리전 독립성, 아바타 커스터마이징, 실시간 음성 연동 등 현업 도입을 위한 거버넌스와 통합이 대폭 강화되었습니다. 또한 프라이빗 네트워크 연계, 원격 평가(A/B 테스트), 사용자 피드백 통합 등 실제 업무 환경에서 필요한 안전성과 확장성에 초점을 맞춘 사례가 많았고, Copilot 및 에이전트 기반 자동화의 거버넌스와 품질 관리가 핵심 트렌드로 부상했습니다. 전반적으로 AI 서비스와 솔루션의 내재화, 엔터프라이즈급 보안·가시성·컴플라이언스 대응이 강화되는 추세입니다.

### [Microsoft Foundry의 글로벌 PTU 예약의 리전 독립성 지원](https://azure.microsoft.com/updates?id=563212)
Foundry에서 프로비저닝 처리량(PTU) 예약이 여러 지역 간 독립적으로 지원되어, 비용 절감과 워크로드 이동성이 현격히 개선되었으며 관리 복잡성이 크게 줄었습니다.

### [Microsoft Foundry에서 셀프 서비스 커스텀 포토 아바타 생성](https://azure.microsoft.com/updates?id=563491)
기업 맞춤형 음성과 외형의 아바타 생성 기능이 Foundry 포털에서 자체적으로 제공되어, 실시간 고객 서비스 등 다양한 사업에 쉽게 접목할 수 있게 되었습니다.

### [Microsoft Foundry Agent Service의 Voice Live 실시간 음성 통합](https://azure.microsoft.com/updates?id=563601)
실시간 음성 입출력(Voice Live)이 Agent Service에 결합되어, 에이전트 기반 대화형 서비스 품질과 고객 경험, 그리고 통합운영이 한층 간소화되었습니다.

---

## 🛠️ 데이터베이스 및 분석

데이터베이스와 분석 영역에서의 핵심 변화는 Azure Cosmos DB, PostgreSQL, DocumentDB, HorizonDB 등 다양한 플랫폼의 확장성과 자동화, 그리고 AI/분석 통합 강화입니다. Cosmos DB는 글로벌 세컨더리 인덱스(GSI) 및 파티션 장애조치 등 대규모 분산·AI 활용에 최적화된 기능이 GA로 도입되었고, PostgreSQL은 오라클-Postgres 마이그레이션/보안 및 확장성 개선, DocumentDB와 HorizonDB는 본격적인 RAG/AI 파이프라인, 오프라인 개발을 위한 에뮬레이터 등 개발자 경험까지 지원합니다. 분석 워크로드에서는 온톨로지 연동, 데이터 API 자동화, Copilot 활용 스키마 설계 등 신기술이 대폭 확대되었습니다. 전체적으로 하이브리드·멀티클라우드, 자동화, 분석/AI 내재화가 주도적인 트렌드입니다.

### [Azure Cosmos DB 글로벌 세컨더리 인덱스 정식 지원](https://azure.microsoft.com/updates?id=562799)
글로벌 세컨더리 인덱스(GSI) 도입으로, 대규모 분산/AI 워크로드에 맞는 효율적인 쿼리 및 워크로드 격리를 제공하여 확장성과 성능이 크게 향상되었습니다.

### [Azure Database for MySQL Flexible Server 셀프서비스 쿼터 관리](https://azure.microsoft.com/updates?id=563147)
포털 기반 셀프서비스 쿼터 관리로, 리드타임 없는 실시간 조정과 용량 계획 및 배포 안정성이 확보되었습니다.

### [Oracle 스키마를 Azure PostgreSQL로 전환하는 VS Code 확장 플러그인 제공](https://azure.microsoft.com/updates?id=563791)
오라클→PostgreSQL 마이그레이션 전체 과정을 VS Code 플러그인으로 지원, 마이그레이션 효율성과 가시성이 크게 강화되었습니다.

---

## 🧩 애플리케이션 통합 및 API 관리

API 관리와 통합 분야에서는 Azure API Management, Logic Apps, API Center 등에서 마이크로서비스, 에이전트통신, 자동화, 거버넌스가 중심적으로 강화되었습니다. 멀티 도메인·Wildcard·A2A 메시지 표준 지원, Agent 자동 등록 및 평가, MCP/AI 모델 게이트웨이, 콘텐츠 안전 관리, 통합 토큰 분석 등으로 실무 API 및 에이전트 관리 복잡도가 대폭 감소했습니다. 엔터프라이즈 등급 보안, 관찰성, 자동화/협업, 운영 효율 향상 등이 두드러진 변화입니다.

### [API Management Premium/Standard v2의 Wildcard 커스텀 호스트네임 지원](https://azure.microsoft.com/updates?id=562894)
다수 서브도메인을 단일 Wildcard로 관리할 수 있어, 대규모 API 온보딩 속도와 운영 효율이 획기적으로 향상됩니다.

### [API Center 에이전트 등록/자동 평가 및 Git 기반 동기화 지원](https://azure.microsoft.com/updates?id=562909)
에이전트 등록·평가 자동화, Git 동기화 등으로 오케스트레이션·협업/운영의 생산성과 신뢰성이 크게 제고되었습니다.

### [Agent-to-Agent(A2A) API 통신의 API Management 정식 지원](https://azure.microsoft.com/updates?id=562843)
마이크로서비스 및 Agent 간 JSON-RPC 통신을 REST/GraphQL/AI와 통합·관리, 보안과 운영 거버넌스 강화가 실현됩니다.

---

## 🚀 인프라 및 컴퓨트/컨테이너

컴퓨트 및 컨테이너 영역에서는 AKS, Functions, Azure Linux, Container Apps 등 핵심 인프라의 무중단 운영, 보안성, 비용 및 운영 효율 강화가 중심입니다. AKS 시스템 노드풀 자동화, Azure Container Linux/Node.js 24/Go 지원, 롤링 업데이트, 커넥터 통합 등 인프라 관점에서의 혁신 기능과 함께, 관찰성 및 진단 기능의 내재화, OS 자동 패치, 서버리스 에이전트 런타임 등 운영 최적화에 집중되어 있습니다.

### [AKS 자동 관리 시스템 노드풀 정식 지원](https://azure.microsoft.com/updates?id=562919)
핵심 Kubernetes 시스템 파트의 자동 관리로 운영팀 부담이 현격히 감축, 가용성과 안정성이 대폭 제고되었습니다.

### [Azure Kubernetes Service에서 Azure Container Linux(ACL) 출시](https://azure.microsoft.com/updates?id=564537)
컨테이너 환경 전용 OS(ACL) 정식 지원으로, 일관된 노드 상태·최신 보안·성능 최적화가 실현됩니다.

### [Azure Functions의 Node.js 24 지원 정식 출시](https://azure.microsoft.com/updates?id=562647)
최신 Node.js 24 런타임 지원이 추가되어, Javascript/Typescript 기반 서버리스 개발/운영 환경이 강화되었습니다.

---

## 📈 관리/운영 및 DevOps

운영 및 DevOps 부문에서는 Azure Monitor, Migrate, Backup, Policy 등 관찰성, 최적화, 규정 준수 측면에서의 품질 관리와 생산성 증진이 돋보입니다. 서비스 수준 지표(SLI/SLO), 머신러닝 기반 동적 임계치, OpenTelemetry 통합, 단순 로그 알림, 파일쉐어 단위 관리, VMSS Flex 자동 업데이트 등 ITSM 관점에서 실무 활용도가 높은 기능들이 대거 도입되었습니다. CI/CD, 운영 자동화, 글로벌 파일 마이그레이션 및 비용 효율화를 목표로 하는 개선이 활발히 이뤄졌습니다.

### [Azure Monitor의 서비스 수준 지표(SLI)/목표(SLO) 도입](https://azure.microsoft.com/updates?id=565159)
고객 경험 기반의 SLI/SLO 중심 진단이 가능해져 기술 지표와 실제 서비스 품질 간 연계가 한층 강화되었습니다.

### [Azure Monitor Log 검색 알림의 동적 임계치 정식 지원](https://azure.microsoft.com/updates?id=561984)
머신러닝 기반 동적 임계치 적용으로, 로그 알림의 자동화·정확성·운영 효율이 크게 개선됩니다.

### [Azure Migrate의 Azure Files 평가 전세계 확대 정식 지원](https://azure.microsoft.com/updates?id=564563)
SMB/NFS 파일쉐어 환경을 자동 분석·마이그레이션하는 평가 기능이 글로벌 지원되어, 파일 기반 워크로드의 클라우드 전환이 용이해졌습니다.