# Azure 월간 업데이트 요약 - 2026년 06월

## 전반적 트렌드 및 핵심 인사이트

2026년 6월 Azure 업데이트는 AI와 에이전트 중심의 클라우드 혁신, 데이터 플랫폼의 확장, 그리고 관리/운영의 자동화와 보안 강화가 두드러진 달이었습니다. 가장 눈에 띄는 변화는 Microsoft Foundry와 Microsoft Fabric 등 새로운 서비스 카테고리의 정식 지원과 미리 보기 기능이 폭넓게 공개되어, 기업이 대규모 AI 및 에이전트 기반 솔루션을 빠르게 도입할 수 있는 환경이 마련된 것입니다.

AI 분야에서는 모델 배포와 운영의 표준화, 엔터프라이즈급 프라이버시 처리 및 평가 기능, 그리고 다양한 분석·검색·음성·비디오 API 통합이 가속화되었습니다. Microsoft Foundry는 모델 카탈로그, 에이전트 서비스, 평가, 자동화 워크플로우 등 혁신적 기능을 선보였고, AI Search와 Azure OpenAI 연동을 위한 관리·보안 강화도 이루어졌습니다. 특히 Purview 기반 민감도 라벨링과 감사, 서버리스 인덱서 등 데이터의 안전과 효율을 높이는 기능이 강조되었고, 에이전트 간 통신(A2A), 사용자 피드백 로깅 등 실무적 자동화도 발전하고 있습니다.

데이터 플랫폼에서 Cosmos DB, HorizonDB, PostgreSQL, DocumentDB 등 주요 서비스가 글로벌 인덱스, 분산 트랜잭션, 벡터 검색과 BM25 등 AI와 검색 특화 기능을 본격 지원하며, 관리 도구와 SDK도 Visual Studio Code와 GitHub Copilot과 연동되어 개발 생산성을 크게 높였습니다. MySQL, PostgreSQL, DocumentDB 등에서 지역 확장과 셀프서비스 할당량·유지 관리, 이관 지원 등 현장에서 요구하는 편의성도 강화되었습니다.

인프라와 운영 영역은 Kubernetes, VMSS, Container Apps, Azure Functions 등 클라우드 네이티브 환경의 자동화, 손쉬운 관리, 그리고 강력한 보안(Defender, RBAC)과 연계된 서비스 간 신뢰성이 크게 향상되었습니다. Azure Monitor는 OpenTelemetry 통합과 SLI/SLO 관점의 모니터링으로 운영 실무에서의 효율성과 가시성을 높였고, DevOps·마이그레이션 도구와의 연계, 네트워크 관리 기능 등도 확대되었습니다.

최신 서비스로의 전환·지원 종료(Deprecated) 정책 또한 지속적으로 고도화되어, 기존 VM, NAT, Synapse Link, Blueprints 등 레거시 서비스는 차세대 솔루션으로의 자연스러운 이동을 유도합니다. 이러한 변화는 Azure가 “AI+데이터+자동화+보안”의 엔터프라이즈 표준 클라우드 플랫폼으로 진화하고 있음을 보여줍니다.

## 주요 카테고리별 요약

---

## 🤖 AI 및 머신러닝

이번 달 Azure AI는 에이전트 개발·배포를 위한 Microsoft Foundry, Foundry IQ, 다양한 언어 및 음성 API, 그리고 Azure AI Translator, Azure AI Search 등에서 텍스트·이미지·음성 통합 및 민감도/보안 강화를 대폭 선보였습니다. 서버리스 인덱서, OpenTelemetry 지원 등 AI 운영 자동화도 진전되며, 엔터프라이즈 규모 모델 관리 및 평가가 실무에 적용되고 있습니다. Microsoft Purview와 연계한 데이터 보안과 감사도 핵심 트렌드입니다.

### [Document translation for image files (synchronous, single document)](https://azure.microsoft.com/updates?id=563341)
이미지 파일 실시간 번역 API가 정식 지원되어 모바일·현장 앱, 폼, 메뉴 등에서 즉시 번역이 가능해졌습니다.

### [Unified Text Translation API in Azure AI Translator](https://azure.microsoft.com/updates?id=563631)
텍스트 번역 API 통합으로 LLM, NMT, 도메인별 모델을 하나의 엔드포인트에서 사용할 수 있어, 엔터프라이즈-다국어 번역의 효율성이 극대화되었습니다.

### [GenAI prompt skill and chat completion in Azure AI Search knowledge sources](https://azure.microsoft.com/updates?id=563247)
Azure AI Search에서 GenAI 프롬프트 스킬 및 챗 완료 기능이 정식 지원되어, AI 기반 콘텐츠 분류 및 요약을 구축하기 쉬워졌습니다.

### [LLM Speech API in Azure AI Speech](https://azure.microsoft.com/updates?id=564387)
다국어 오디오 파일에 대해 LLM 기반의 고품질 음성 인식·번역 API가 정식 지원되어, 음성 AI의 활용도가 크게 향상되었습니다.

### [Voice Live integration with Microsoft Foundry Agent Service](https://azure.microsoft.com/updates?id=563601)
실시간 음성-텍스트 상호작용을 기반으로 Foundry 에이전트와 직접 연동, 고객 상담, 자동차 음성 서비스 등에서 완전한 AI 에이전트 통합이 가능해졌습니다.

---

## 🗄️ 데이터베이스

Cosmos DB, HorizonDB, DocumentDB 등 주요 데이터베이스에서 글로벌 인덱스, 분산 트랜잭션, AI/벡터 검색, 고가용성, 셀프서비스 관리 도구 및 통합 SDK가 출시되었습니다. 데이터베이스와 AI, 에이전트 연계의 표준화 및 개발 생산성 향상이 월간 트렌드입니다.

### [Azure Cosmos DB global secondary indexes](https://azure.microsoft.com/updates?id=562799)
글로벌 세컨더리 인덱스 정식 지원으로 읽기 성능이 대폭 개선, 복잡한 파티셔닝과 쿼리 부담을 줄였습니다.

### [Azure Database for PostgreSQL - Flexible Server: DuckDB extension](https://azure.microsoft.com/updates?id=563766)
DuckDB 확장 정식 지원으로 PostgreSQL에서 로컬 분석 및 클라우드 기반 분석 워크플로우를 유연하게 운영할 수 있습니다.

### [Azure DocumentDB Migration Extension in Visual Studio Code](https://azure.microsoft.com/updates?id=563072)
VS Code에서 드래그 앤드 드롭 방식의 DocumentDB 이관이 가능하여 DX(개발 경험)가 크게 개선되었습니다.

### [Azure Database for PostgreSQL flexible server pg_ivm extension](https://azure.microsoft.com/updates?id=563771)
pg_ivm 확장 정식 지원으로 PostgreSQL의 즉시 뷰(Materialized View) 기능 사용이 가능해졌습니다.

### [Azure Cosmos DB all versions and deletes change feed mode](https://azure.microsoft.com/updates?id=562971)
모든 버전 및 삭제 변경 피드 모드가 정식 지원되어, 데이터 복제·감사·트리거 개발이 가능합니다.

---

## ☁️ 인프라 및 컴퓨팅

Kubernetes, VMSS, Container Apps, Azure Functions, Azure Linux 등 클라우드 기반 인프라의 자동화·운영 개선이 두드러졌습니다. Azure Linux 4.0, Azure Container Linux, AKS 자동 관리, 멀티 클라우드 지원 등 효율성과 보안이 강화된 신규 기능이 출시되었습니다. VM, NAT, Batch 등 일부 인프라 서비스는 지원 종료 공지가 잇따랐습니다.

### [Azure Container Linux (ACL) now generally available on Azure Kubernetes Service (AKS)](https://azure.microsoft.com/updates?id=564537)
Immutable OS로 클러스터 운영 안전성·속도가 향상, 보안 기반 Kubernetes 환경 구축이 더 쉬워졌습니다.

### [Azure Kubernetes Fleet Manager for Arc-enabled clusters](https://azure.microsoft.com/updates?id=562904)
Azure Arc 지원으로 하이브리드·멀티클라우드 Kubernetes 클러스터 통합 관리가 실현되었습니다.

### [Azure NC RTX PRO 6000 Blackwell Server Edition v6 Series Virtual Machines](https://azure.microsoft.com/updates?id=565271)
최신 GPU·AI용 VM이 정식 지원되어, 고성능 AI·그래픽 워크로드 운영이 확대되었습니다.

### [Azure Functions Support for Node.js 24](https://azure.microsoft.com/updates?id=562647)
최신 Node.js 24 지원으로 Functions의 DX와 호환성이 개선되었습니다.

### [Azure VM 및 Batch용 Av2/F/G/Ls, D/Ds/Dv2/Dsv2/LS 지원 종료 안내](https://azure.microsoft.com/updates?id=564774)
레거시 VM 시리즈 지원 종료 및 대체 안내로 최신 VM으로의 전환을 촉진하고 있습니다.

---

## 🔗 통합 및 개발자 경험

Azure API Center, API Management, Logic Apps 등에서 MCP, Agent-to-Agent, 다중 커스텀 도메인, 컨텐츠 안전 정책, 통합 커넥터 등 엔터프라이즈 규모 API/에이전트 카탈로그 및 통합 관리 기능이 출시되었습니다. 신규 기능은 Git 기반 동기화, LLM 품질 평가, Agent API 관리 표준화, Connector Namespace 등의 형태로 DX와 신뢰성을 동시에 개선하였습니다.

### [Azure API Center now supports agent registration, agent assessment, and Git-based synchronization](https://azure.microsoft.com/updates?id=562909)
에이전트 등록·품질 평가·Git 동기화 정식 지원으로 AI 및 자동화 조직의 전체자산 관리가 간소화되었습니다.

### [Azure API Management adds support for Agent-to-Agent (A2A) APIs](https://azure.microsoft.com/updates?id=562843)
A2A 통신 API 관리 표준화로 에이전트 기반 워크플로우의 보안·운영 일관성이 향상되었습니다.

### [Azure API Management Premium v2 and Standard v2 now support wildcard custom hostnames](https://azure.microsoft.com/updates?id=562894)
와일드카드 도메인 지원으로 대규모 API 환경의 인증서·도메인 관리가 자동화되었습니다.

### [Azure Logic Apps MCP Server](https://azure.microsoft.com/updates?id=562868)
Logic Apps 워크플로우를 AI 에이전트 호출 대상(MCP Tool)로 노출 가능, 엔터프라이즈 자동화가 강화되었습니다.

### [Connector Namespace Public Preview](https://azure.microsoft.com/updates?id=562874)
SharePoint, Salesforce 등 타사와 표준 커넥터로 신속한 통합/인증 운영이 실현되었습니다.

---

## 👩‍💻 Microsoft Foundry

Microsoft Foundry는 AI 모델 카탈로그·플레이그라운드·에이전트 개발·평가·자동화 등 에이전트 중심 AI 제품의 표준 플랫폼으로 자리잡고 있습니다. 이번 달에는 Foundry IQ, Agent Service, 평가·관찰·피드백, 도메인 필터, Voice Live 통합, 정식 SDK 및 VS Code 확장, Purview 연동 등 데이터와 모델, 보안, 운영 계층 모두에서 혁신이 이뤄졌습니다. 또한 OneLake/Fabric와의 연동, 도메인별 모델, 원격 MCP 서버 지원 등이 가속화되고 있습니다.

### [Custom Avatar and Custom Video portal in Microsoft Foundry](https://azure.microsoft.com/updates?id=563436)
커스텀 아바타·비디오 저작·생성 기능 정식 지원, 음성·이미지 합성 기반 AI 에이전트 구현이 쉬워졌습니다.

### [Microsoft Foundry for Visual Studio Code (June Build 2026 refresh)](https://azure.microsoft.com/updates?id=563721)
VS Code 확장 정식 지원, 모델 검색/배포/코드생성까지 개발 환경에서 원스톱으로 진행 가능합니다.

### [Managed virtual network for evaluations in Microsoft Foundry](https://azure.microsoft.com/updates?id=564402)
에이전트/모델 평가용 Virtual Network 지원으로 보안·컴플라이언스 환경에서 자동화 평가가 가능해졌습니다.

### [Region-agnostic reservations for Global PTU in Microsoft Foundry](https://azure.microsoft.com/updates?id=563212)
폰드리 모델의 지역 비상관성 예약(할인) 지원, 대형 AI 사용 비용 관리·조달이 대폭 간소화되었습니다.

### [Benchmark evaluations for fine-tuned models in Microsoft Foundry](https://azure.microsoft.com/updates?id=563167)
모델 및 에이전트의 벤치마크 평가 자동화 기능 미리 보기, 엔터프라이즈 기준으로 AI 품질 측정 가능.

---

## 🏢 Microsoft Fabric

Microsoft Fabric은 데이터 레이크·AI·분석의 통합 플랫폼으로, OneLake 연동성·카탈로그·Mirroring 서비스가 다수 출시되었습니다. Azure Databricks와의 직접 연동, Genie MCP, Fabric Ontology, OneLake 기반 배치/분석 및 권한 관리 등이 엔터프라이즈의 데이터 거버넌스와 AI 활용을 혁신하고 있습니다.

### [Azure Databricks native read access to Microsoft OneLake](https://azure.microsoft.com/updates?id=565733)
OneLake 내 데이터 조회 기능 정식 지원, 데이터 이동 없이 Azure Databricks와 통합 분석 가능.

### [Azure Databricks natively storing data in Microsoft OneLake](https://azure.microsoft.com/updates?id=565706)
Azure Databricks 데이터 직접 OneLake 저장 지원, Fabric·Databricks 간 데이터 중복 및 관리 부담 해소.

### [Fabric IQ Ontology Knowledge Source in Microsoft Foundry IQ](https://azure.microsoft.com/updates?id=563416)
Fabric Ontology를 Foundry IQ 지식 소스로 연동, 엔터프라이즈 비즈니스 정의 및 AI 활용이 심화됨.

### [OneLake catalog integration for Azure AI Search knowledge sources](https://azure.microsoft.com/updates?id=564407)
OneLake 카탈로그 직접 연동, Fabric 통합 데이터 거버넌스 및 권한 정책의 AI/RAG 파이프라인 적용 가능.

### [Azure Synapse Link for Azure Cosmos DB NoSQL 지원 종료 및 Mirroring 권장](https://azure.microsoft.com/updates?id=558560)
2029년 Synapse Link 지원 종료, 대체 분석 플랫폼으로 Fabric Mirroring 권장 안내.

---

## 🔒 관리 및 거버넌스

Azure Monitor, Migrate, Policy, Blueprints 등 관리·운영 플랫폼에서 SLI/SLO 기반 모니터링, OpenTelemetry 통합, 자동 정책·감사, 마이그레이션 도구의 AI 연동이 본격 추진되고 있습니다. Blueprints, VM, NAT 등 일부 서비스는 지원 종료와 함께 신규 솔루션으로 이전 유도되고 있습니다.

### [Azure Monitor Service Level Indicators (SLI)](https://azure.microsoft.com/updates?id=565159)
서비스 수준 지표·목표(SLI/SLO) 기반 사용자 중심 모니터링 정식 지원, 실제 고객 경험 측정이 가능해졌습니다.

### [Azure Migrate – GitHub Copilot Modernization integration for at scale code assessments](https://azure.microsoft.com/updates?id=566145)
마이그레이션 자동화 도구와 Copilot 연동으로 코드 분석·현대화 추천이 자동화되었습니다.

### [Azure Infrastructure Resiliency Manager](https://azure.microsoft.com/updates?id=564759)
애플리케이션 레질리언스 설계, 평가, 개선을 위한 통합 관리 포털 미리 보기 기능 출시.

### [Azure Blueprints 지원 종료 및 Azure Deployment Stack으로 이전 권장](https://azure.microsoft.com/updates?id=564806)
Blueprints 2027년 지원 종료, 스택·템플릿 기반 운영으로 전환 필요.

### [Log Analytics Summary Rules experience](https://azure.microsoft.com/updates?id=562027)
로그 집계 및 추가 분석 경험 강화, 초고속 데이터 요약·비용 최적화 가능.

---

## 전체 업데이트 총평 및 다음 달 전망

이번 달 Azure는 데이터와 에이전트 중심 클라우드 시스템의 대규모 자동화와 표준화, 그리고 엔터프라이즈 실무 수요에 맞춘 AI·보안·운영 플랫폼의 진화를 다시 한번 입증했습니다. Microsoft Foundry, Fabric, API Center 등 신규 카테고리의 정식 지원은 데이터와 모델, 에이전트, 보안이 유기적으로 연동되는 클라우드 내재형 AI 표준의 본격화를 의미합니다. 관리 및 거버넌스 영역에서는 DX 개선, 자동화, 정책·감사 표준화가 강화됐고, 기존 인프라 자원(Blueprints, VM, NAT, Synapse Link 등)의 지원 종료 안내는 최신 서비스로의 전환을 적극 유도하고 있습니다.

다음 달에는 Microsoft Fabric과 Foundry의 기능 및 연결성이 추가 확대되고, 보안·감사·AI 평가와 운영 자동화 분야에서 새로운 규제 대응 및 실무 지원 도구들이 등장할 전망입니다. 또한 글로벌 및 한국 지역의 신규 서비스 배포와, 최신 VM, 컨테이너, 데이터 서비스 지원 확대를 통해 엔터프라이즈 클라우드 환경의 안정성·효율성이 더욱 향상될 것으로 기대됩니다.