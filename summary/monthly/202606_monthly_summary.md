# Azure 월간 업데이트 요약 - 2026년 06월

## 전반적인 트렌드와 핵심 인사이트

2026년 6월 Azure의 업데이트에서 가장 뚜렷하게 관찰된 트렌드는 "AI 중심의 플랫폼 혁신"과 "엔터프라이즈 자동화 및 개발 효율성 강화"입니다. Microsoft Foundry와 Microsoft Fabric 등 AI 및 데이터 기반 서비스가 핵심 사업부들의 전략적 방향을 주도하고 있습니다. 이번 달에는 AI/머신러닝 관련 기능의 정식 지원과 미리 보기, 그리고 보안과 거버넌스를 위한 기술적 강화가 많은 비중을 차지했습니다.

Azure AI 및 Foundry는 매우 다양한 AI 및 데이터 분석 시나리오를 지원하면서, 개발자와 엔터프라이즈 사용자의 피드백을 반영한 새로운 API, 모델, 도구를 지속적으로 출시하고 있습니다. 특히, 영지식 처리와 도메인별 모델 필터링, 자연어 기반 데이터 쿼리, API 레이어의 표준화, 대화형 PII 탐지 등 데이터 및 작업 기반 AI에서 중요한 역할을 합니다.

인프라 관점에서는 VM과 스토리지의 세분화, 네트워킹의 성능 및 보안 향상, OS 플랫폼(예: Azure Linux, Azure Container Linux) 미리 보기 및 정식 지원이 확대되었습니다. 컨테이너, 서버리스 컴퓨팅, 데이터베이스 등에서 확장성과 자동화, 표준화된 관리 경험을 위한 신기능이 연이어 등장하며 개발자 효율성과 운영 신뢰성을 높였습니다.

또한, 보안 및 거버넌스 강화가 꾸준히 이루어지고 있으며, 서비스별 도메인 통합, 역할 기반 액세스, 감시 및 감사 기능이 도입되어 클라우드 환경 전반에서 법적/사업적 요구를 충족시키고 있습니다. 데이터베이스와 AI, 미리 보기 기능, 기존 서비스의 지원 종료(deprecation, retirement) 등으로 Azure의 서비스 포트폴리오는 더욱 진화하고 있습니다.

전체적으로 이번 달 Azure 업데이트는 차세대 AI 기반 개발 환경의 대중화와 엔터프라이즈 현업 업무 자동화, 그리고 인프라 운영의 표준화와 거버넌스 강화를 중심으로 진행되었으며, 개발자와 엔터프라이즈 고객의 협업과 생산성이 크게 높아질 수 있는 기반을 마련했습니다.

---

## 🚀 AI 및 머신러닝

Azure의 AI 및 머신러닝 부문에서는 생산성과 거버넌스, 인프라 연동의 강화가 두드러집니다. Foundry와 Azure AI Translator를 중심으로 다양한 실시간 및 비동기 지원이 확대되었으며, 데이터 및 모델 기반의 자동화와 효율적 협업이 가능해졌습니다.

### [Speech SDK 1.50 for Azure AI Speech](https://azure.microsoft.com/updates?id=563192)
최신 Speech SDK 1.50이 여러 언어와 플랫폼에서 정식 지원되며 음성 인식 및 합성 기능을 강화함.

### [LLM Speech API in Azure AI Speech](https://azure.microsoft.com/updates?id=564387)
최신 LLM 기반 음성 API의 정식 지원으로 25개 언어, 90+ 로케일의 정확한 트랜스크립션 및 번역 제공.

### [Document translation for image files (synchronous, single document)](https://azure.microsoft.com/updates?id=563341)
이미지 파일 즉시 번역 기능이 정식 지원되어 OCR과 번역이 단일 API에서 실시간으로 처리 가능.

### [OneLake catalog integration for Azure AI Search knowledge sources](https://azure.microsoft.com/updates?id=564407)
OneLake 카탈로그와 Azure AI Search의 통합으로 데이터 거버넌스와 보안, 중복 제거가 실현됨.

### [Azure Databricks native read access to Microsoft OneLake](https://azure.microsoft.com/updates?id=565733)
Databricks에서 OneLake 데이터를 직접 분석할 수 있게 되어 데이터 플랫폼 전반의 활용성과 효율성이 크게 향상됨.

---

## 👩‍💻 Microsoft Foundry

Microsoft Foundry는 Azure 상에서 AI, 음성, 텍스트 이해, 평가, 모델 통합 등 다양한 기능을 선보이며 개발자 중심의 혁신적 플랫폼으로 자리잡고 있습니다. 이번 달에는 모델 카탈로그, 도메인 필터, 전문 API, 평가 및 관찰 기능, 보안 연동 등 새로운 기능들이 정식 지원 및 미리 보기로 대거 추가되었습니다.

### [Adaptive custom translation in the Azure AI Foundry NextGen playground](https://azure.microsoft.com/updates?id=563307)
AdaptCT 기능이 정식 지원으로 출시되어 도메인 기반 번역 개선 및 자동화된 워크플로우 구현이 가능해짐.

### [Content Understanding extractionMode for documents](https://azure.microsoft.com/updates?id=563257)
문서 분석에서 extractionMode 옵션이 도입되어 구조화/비구조화 문서 모두 정확한 분석 지원.

### [Custom Avatar and Custom Video portal in Microsoft Foundry](https://azure.microsoft.com/updates?id=563436)
맞춤 아바타 및 영상 제작 기능이 Foundry에 통합되어 AI 기반 대화형 컨텐츠 제작 자동화 구현.

### [Custom Voice portal experience in Microsoft Foundry](https://azure.microsoft.com/updates?id=563691)
맞춤 음성 생성 및 배포 기능이 Foundry portal로 통합되어 음성 모델 생산성과 협업 흐름이 강화됨.

### [Microsoft Foundry for Visual Studio Code (June Build 2026 refresh)](https://azure.microsoft.com/updates?id=563721)
VS Code에서 Foundry 전체 모델 카탈로그, 플레이그라운드, 에이전트 배포 기능을 쉽게 사용할 수 있어 개발 환경의 혁신적 변화 제공.

---

## 🛠️ 데이터베이스 및 스토리지

데이터베이스 및 스토리지 부문에서는 대규모 데이터 처리, 연속성, 자동화, 인텔리전스 기능이 강화되었습니다. PostgreSQL, Cosmos DB, DocumentDB 등에서 새로운 기능과 관리 경험이 정식 지원 및 미리 보기로 제공되고 있습니다.

### [Azure Cosmos DB all versions and deletes change feed mode](https://azure.microsoft.com/updates?id=562971)
Cosmos DB의 변경 피드에서 모든 버전 및 삭제 상태 추적이 정식 지원되어 데이터 변경과 보안/감사 워크플로우 강화.

### [Azure Database for MySQL Flexible Server self-service quota management experience](https://azure.microsoft.com/updates?id=563147)
MySQL 서버에서 실시간 쿼터 관리 기능 제공으로 개발자 및 운영팀의 효율적 리소스 관리 실현.

### [Azure Database for PostgreSQL - Flexible Server: DuckDB extension](https://azure.microsoft.com/updates?id=563766)
PostgreSQL에서 DuckDB 확장 설치로 빠른 로컬 분석과 OLAP 워크플로우 구현 가능.

### [Azure Database for PostgreSQL flexible server pg_ivm extension](https://azure.microsoft.com/updates?id=563771)
pg_ivm 확장 지원으로 실시간 인메모리 뷰 관리 가능, 대용량 데이터 분석에 최적화.

### [Azure DocumentDB Migration Extension in Visual Studio Code](https://azure.microsoft.com/updates?id=563072)
VS Code에서 MongoDB에서 DocumentDB로 마이그레이션을 손쉽게 수행할 수 있는 확장, 비용 및 시간 절약.

---

## 🏗️ 인프라, 컴퓨트, 네트워크

컴퓨트 및 네트워크 서비스에서는 VM, OS, 컨테이너, 네트워크 게이트웨이 등 인프라 성능과 관리성 강화가 주요 흐름입니다. 특히 VM 시리즈와 OS의 지원 확대, NAT Gateway 개선, 인프라의 자동화와 손쉬운 운영이 강조되었습니다.

### [Azure NC RTX PRO 6000 Blackwell Server Edition v6 Series Virtual Machines](https://azure.microsoft.com/updates?id=565271)
최신 NVIDIA GPU 기반 VM 시리즈의 정식 지원으로 고성능 AI 및 그래픽 워크로드를 더욱 빠르고 효율적으로 처리할 수 있음.

### [Premium SSD v2 disks now support non-zonal Azure Virtual Machines](https://azure.microsoft.com/updates?id=565359)
비존 VM에서도 프리미엄 SSD v2 사용 지원으로 비용 및 성능 최적화 가능.

### [ICMP Support for Azure Standard V2 NAT Gateway](https://azure.microsoft.com/updates?id=565487)
NAT Gateway에서 ICMP(Echo, Reply) 지원으로 네트워크 연결성 검증 및 장애 분석이 간편해짐.

### [Azure Container Linux (ACL) now generally available on Azure Kubernetes Service (AKS)](https://azure.microsoft.com/updates?id=564537)
컨테이너 최적화 리눅스 OS(ACL)의 AKS 정식 지원으로 보안성, 불변성, 관리 효율 향상.

### [Azure Kubernetes Fleet Manager for Arc-enabled clusters](https://azure.microsoft.com/updates?id=562904)
Fleet Manager를 통한 하이브리드/멀티클라우드 쿠버네티스 중앙 관리 지원으로 운용 효율 및 가시성 극대화.

---

## 🔗 통합, API, IoT, DevOps

API Management, Logic Apps, IoT, DevOps 관련 영역에서는 최신 통합, 자동화, 감시, 거버넌스 강화 기능이 대폭 추가되었습니다. API 에이전트 관리, MCP 서버, A2A 통신 등 엔터프라이즈 통합 및 운영 효율이 크게 향상되었습니다.

### [Azure API Center now provides a data plane MCP server for enterprise-wide discovery of APIs and AI assets.](https://azure.microsoft.com/updates?id=562914)
API Center에서 MCP 서버 데이터 평면이 정식 지원되어 기업 전체의 API 및 AI 자산 탐색 및 관리 중앙화.

### [Azure API Management adds support for Agent-to-Agent (A2A) APIs](https://azure.microsoft.com/updates?id=562843)
A2A API 지원으로 엔터프라이즈 AI 시스템의 에이전트간 통신과 거버넌스가 강화됨.

### [Azure API Management now supports content safety controls for MCP and A2A APIs.](https://azure.microsoft.com/updates?id=562880)
MCP/A2A API 대상 콘텐츠 안전 정책 중앙관리, 비정상/위험 데이터 차단 및 규제 준수 구현.

### [Azure Logic Apps MCP Server.](https://azure.microsoft.com/updates?id=562868)
Logic Apps 워크플로우를 MCP 서버로 노출 가능하게 하여 AI 에이전트 기반 자동화 및 통합 실현.

### [Azure Event Grid - MQTT v5 Subscription Identifier](https://azure.microsoft.com/updates?id=564532)
MQTT v5 구독 식별자 정식 지원으로 메시지 라우팅 및 IoT 이벤트 처리 품질 및 효율성 개선.

---

## 🦾 관리 및 거버넌스, 보안

Azure는 관리 및 거버넌스, 보안 부문에서 DevOps 및 서비스 관리 체계를 강화하고 있습니다. 모니터링, 감사, 업데이트, 자율 관리, 사고 복구 등에서 더욱 스마트한 운영 경험과 신뢰성 향상이 이루어졌습니다.

### [Azure Monitor Service Level Indicators (SLI)](https://azure.microsoft.com/updates?id=565159)
애플리케이션 고객 경험 중심의 서비스 품질 지표(SLI/SLO) 도입, 운영 노이즈 제거 및 서비스 수준 실현 가능.

### [Dynamic threshold for Log search alerts](https://azure.microsoft.com/updates?id=561984)
동적 임계치 기반 로그 알림 정식 지원으로 모니터링 자동화 및 대규모 환경 운영 효율성 향상.

### [Log Analytics Summary Rules experience](https://azure.microsoft.com/updates?id=562027)
Summary Rules 기능으로 대량 로그 데이터를 요약 관리 및 쿼리 성능 개선 가능.

### [Azure Migrate – GitHub Copilot Modernization integration for at scale code assessments](https://azure.microsoft.com/updates?id=566145)
Azure Migrate와 GitHub Copilot 현대화 통합으로 대규모 코드 평가 및 현대화, 자동화 추천 가용.

### [Azure Site Recovery support for Linux Azure VMs with NVMe disk controllers.](https://azure.microsoft.com/updates?id=565103)
NVMe 디스크 기반 Linux VM 복구 지원으로 고성능 워크로드의 DR 및 운영 신뢰성 강화.

---

## 📉 서비스 지원 종료 및 사용 중단(Retirement/Deprecation)

Azure는 지속적으로 서비스 포트폴리오를 재정비하고 있습니다. 노후 VM 시리즈, Storage Accounts, Blueprints, VPN Client 등 일부 서비스의 지원 종료가 발표되어 사용자들의 선제적 대응이 요구됩니다.

### [Av2-series, F-series, Fs-series, Fsv2-series, G-series, Gs-series, and Lsv2-series Virtual Machines for Azure Batch pools](https://azure.microsoft.com/updates?id=564774)
Batch Pool 대상 VM 시리즈의 2028년 11월 15일 지원 종료, 신규 Pool 생성을 막고 기존 Pool 마이그레이션 권장.

### [Azure Load Balancer Inbound NAT rule version 1 for Azure VMSS (Inbound NAT Pools)](https://azure.microsoft.com/updates?id=565482)
Inbound NAT Pools는 2027년 9월 30일에 지원 종료, 버전 2로의 마이그레이션 요구.

### [GPv1 and Legacy Blob storage account creation](https://azure.microsoft.com/updates?id=564441)
GPv1 및 레거시 Blob Storage Account 신규 생성은 2026년 6월 1일부터 불가, 10월 13일 최종 Retirement.

### [Azure Synapse Link for Azure Cosmos DB NoSQL](https://azure.microsoft.com/updates?id=558560)
Synapse Link의 신규 계정 생성 중단(2026년 3월 31일), Fabric Mirroring로의 마이그레이션 권장.

### [Azure VPN Client for Linux (Preview)](https://azure.microsoft.com/updates?id=565393)
Linux VPN 클라이언트 미리 보기 2026년 8월 31일 사용 중단, 대체 클라이언트로 전환 필수.

---

## 총평 및 다음 달 전망

2026년 6월 Azure 업데이트는 AI 기반 업무 자동화와 플랫폼 연동, 인프라 표준화, 엔터프라이즈 거버넌스와 보안, 그리고 개발 생산성의 획기적 향상을 중심으로 이루어졌습니다. Microsoft Foundry와 Fabric의 지속적인 발전으로 모든 개발자와 엔터프라이즈가 AI-기반 서비스와 자동화에 한층 쉽게 접근할 수 있게 되었으며, 기존 인프라 서비스의 효율성과 표준화가 강화되고 있습니다.

수많은 미리 보기(preview) 기능이 빠르게 정식 지원(GA) 단계로 발전하는 만큼, 향후 AI를 중심으로 한 모듈형 자동화, 데이터 거버넌스, 개발자 환경 혁신이 계속될 것으로 예상됩니다. 7월에는 Foundry 기반 신규 모델, Fabric 및 OneLake 관련 확장, 더 빠른 데이터베이스 기능, 엔터프라이즈 보안 및 거버넌스 도구의 정식 지원 소식이 이어질 전망입니다. Azure를 활용하는 모든 조직은 AI, 자동화, 데이터 중심의 기술 포트폴리오 변화를 주목하면서 적극적인 도입 전략을 준비해야 할 시점입니다.