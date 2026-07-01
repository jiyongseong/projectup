# Azure 월간 업데이트 요약 - 2026년 06월

## 전반적 트렌드 및 핵심 인사이트

2026년 6월 Azure 업데이트는 AI·머신러닝, 데이터 분석, 클라우드 인프라, 개발자 생산성, 보안 및 거버넌스 강화, 그리고 멀티지역·멀티클라우드 확장에 초점을 맞추고 있습니다. 최근 집중되고 있는 트렌드는 크게 세 가지로 요약할 수 있습니다.

첫째, Microsoft Foundry와 관련한 에코시스템이 눈에 띄게 확장되고 있습니다. 모델·에이전트 개발, 도구 통합, 뱃치·리얼타임 평가, 가상네트워크 관리, 보안성과 거버넌스 정책 강화 등 Foundry 기반의 AI 개발환경이 전사적 활용에 한층 적합하도록 진화하고 있습니다. “다량의 모델(1,900+) 카탈로그, 호스팅 에이전트 서비스, VS Code 연계, 공통 모듈화 및 추적 기능 제공” 등 Foundry를 중심으로 한 AI 개발 생산성이 높아졌고, 전문 지식이 요구되는 데이터셋 접근, 모델 성능 벤치마크, 도메인별 필터링 등도 자동화가 가능해졌습니다.

둘째, Databricks 및 Microsoft Fabric과 연결된 통합 데이터 관리·분석 기능이 강화됐습니다. OneLake와의 연동, Lakehouse 기반 데이터 브랜칭, 자연어 검색, 데이터 카탈로그 통합, Fabric Ontology 연계 등 기존 데이터 플랫폼을 AI·분석 파이프라인으로 곧장 연결할 수 있게 진화하고 있습니다.

셋째, 클라우드 인프라와 서비스 확장이 속도를 내면서 VM 시리즈·컨테이너·데이터베이스·스토리지 등 주요 리소스의 성능 및 관리 편의가 더욱 높아졌습니다. VM 시리즈 신규 출시, 저지연 고성능 네트워킹, 최신 오픈소스 OS 적용, 플렉스 플랜 및 자동화, 그리고 퍼블릭 프리뷰 기반의 고보안·고신뢰 운영모델 등이 두드러집니다.

또한 API 관리, 에이전트간 통신, 자동화된 통합·연동, 통합 트레이싱과 모니터링 등 분산형 서비스 아키텍처를 위한 플랫폼 서비스도 한층 세분화되고 있습니다.

운영과 거버넌스 영역에서는 신규 모니터링 지표(서비스레벨지표), 동적 임계값 기반 로그 알림, 각종 SLI/SLO 도입, 마이그레이션 단순화, 자동화 관리, 정책 강화를 통해 안정성과 신뢰성을 높이고 있습니다. 엔트라 ID, RBAC, 키 관리, 테넌트간 암호화, 민감정보 추적 등 보안이슈 대응 역시 강한 성장세를 보입니다.

이번 달은 미리보기(preview)를 포함하여 차세대 AI 플랫폼 기능, 오픈소스 신기술, 네트워킹/스토리지 정책 변화, VM 및 API 사용 종료 안내(retirement) 등이 공존했던 시기입니다.

## 카테고리별 업데이트 요약

---

## 🧠 AI + 머신러닝 및 분석

AI와 데이터 분석 영역에서는 Foundry 강화와 AI Search, Translator, Speech, Fabric과 연계된 다양한 고도화 기능이 정식 지원 또는 미리 보기로 출시되었습니다. 이 카테고리는 산업별 모델 접근성, 도구 통합, 자동화, 보안, 사용자 피드백 기반 최적화, 그리고 네이티브 데이터 카탈로그 활용이 핵심입니다.

### [Adaptive Custom Translation in Azure AI Foundry NextGen playground](https://azure.microsoft.com/updates?id=563307)
- 도메인 특화 번역을 소규모 데이터로 동적으로 적용 가능한 정식 지원 기능. 모델 재훈련 없이 고품질 번역 및 빠른 콘텐츠 갱신 가능.

### [Azure Databricks native read access to Microsoft OneLake](https://azure.microsoft.com/updates?id=565733)
- Databricks에서 OneLake의 데이터를 복사하지 않고 직접 쿼리/분석 가능. 데이터 이중화 없이 통합 분석·거버넌스 강화.

### [GenAI prompt skill and chat completion in Azure AI Search knowledge sources](https://azure.microsoft.com/updates?id=563247)
- Azure AI Search의 인덱서가 챗 완료 모델 호출, 자동 분류·정규화·정리 등의 지능형 콘텐츠 가공을 실현.

### [Document translation for image files (synchronous, single document)](https://azure.microsoft.com/updates?id=563341)
- 이미지 파일(JPEG, PNG 등) 번역 정식 지원, OCR+번역 결합으로 문서 형태를 유지한 상태로 실시간 번역 결과 제공.

### [LLM Speech API in Azure AI Speech](https://azure.microsoft.com/updates?id=564387)
- 다국어(25개국, 90+ 로케일) 음성의 실시간/배치 변환 및 번역—정확도, 지역 확장, 프롬프트 튜닝 지원.

**요약**: AI 서비스의 품질·유연성·통합성이 대폭 향상되었으며, 엔터프라이즈 사용성을 강화하는 보안·비용관리·실시간 처리 기능이 계속 확대되고 있습니다.

---

## ⚙️ 클라우드 인프라 및 컴퓨트

컴퓨트와 인프라 영역에서는 VM 신제품, 고성능 네트워킹, 자동화 플랜, 컨테이너 운영체제 및 시스템 자동화 등 최신 기술이 도입되어 대용량/고성능·탄력적·보안 중심의 운영환경을 지원합니다.

### [Azure NC RTX PRO 6000 Blackwell Server Edition v6 Series Virtual Machines](https://azure.microsoft.com/updates?id=565271)
- NVIDIA Blackwell GPU 기반 VM 정식 지원, AI·그래픽·ISV용 최상급 성능 제공.

### [Azure Container Linux ACL for AKS](https://azure.microsoft.com/updates?id=564537)
- Flatcar 계열의 컨테이너 최적화 리눅스 OS 정식 제공, 보안 강화 및 운영일관성 확보.

### [Rolling updates in Flex Consumption](https://azure.microsoft.com/updates?id=562365)
- Functions Flex Consumption 플랜에서 무중단 롤링 배포 지원, 높은 가용성과 무중단 CI/CD 실현.

### [Automatic OS Image Upgrades for VMSS Flex](https://azure.microsoft.com/updates?id=564976)
- VM Scale Set Flex의 자동 OS 이미지 업그레이드 미리 보기, 대규모 인프라 일관적 패치 관리 자동화.

### [Guest RDMA on Azure Boost](https://azure.microsoft.com/updates?id=564981)
- VM 내부 RDMA 지원 미리 보기, 초저지연/고대역폭 네트워킹으로 AI/HPC 등 데이터 집약 워크로드 고속화.

**요약**: 컴퓨트 자원은 성능 향상, 보안 강화, 배포 자동화, 관리 일원화를 통해 최신 클라우드 운영환경으로 업그레이드되고 있습니다.

---

## 🌐 데이터베이스 및 스토리지

데이터베이스·스토리지 부문의 주요 변화로는 NoSQL·PostgreSQL·DocumentDB·HorizonDB 등 다양한 엔진 기능 개선, 마이그레이션 자동화, 에이전트·AI 기반 통합, 스토리지 계정 정책 업데이트 등이 있습니다.

### [Azure Cosmos DB global secondary indexes](https://azure.microsoft.com/updates?id=562799)
- 글로벌 세컨더리 인덱스 정식 지원, 쿼리 성능/최적화 및 비용 절감.

### [Azure Database for PostgreSQL - Flexible Server: DuckDB extension](https://azure.microsoft.com/updates?id=563766)
- DuckDB 및 pg_ivm 확장 지원—임베디드 분석 및 인메모리 매터리얼 뷰로 대규모 분석 효율 개선.

### [Azure DocumentDB Migration Extension in Visual Studio Code](https://azure.microsoft.com/updates?id=563072)
- MongoDB 환경→DocumentDB로 데이터 마이그레이션을 VS Code에서 바로 진행 (실시간, 비가동).

### [Azure HorizonDB Agentic Advisor Solution Accelerator](https://azure.microsoft.com/updates?id=563092)
- HorizonDB 기반 에이전트 솔루션 가속기—LangGraph, Mem0 등과 연계한 복합 데이터 처리/AI 검색 자동화.

### [Azure Database for MySQL Flexible Server self-service quota management experience](https://azure.microsoft.com/updates?id=563147)
- 쿼터 관리 자동화, 포털에서 실시간 조정 및 처리 시간 대폭 단축.

**요약**: 데이터베이스는 고성능·확장성, 개발자 친화적 자동화, 마이그레이션 단순화, AI와의 통합을 중심으로 진화 중이며, 실무자 요구에 맞는 현장 관리 기능도 확대되고 있습니다.

---

## 🛠️ 개발, 통합 및 API 관리

API·통합 관리 및 개발 생산성 영역에서는 Azure API Center, API Management, Logic Apps, Functions 등 중앙 관리 및 자동화 기능, 에이전트 기반 평가/연동, GitHub Copilot·MCP 연계, 다양한 도구 통합이 두드러집니다.

### [Azure API Center now provides a data plane MCP server for enterprise-wide discovery of APIs and AI assets](https://azure.microsoft.com/updates?id=562914)
- API/AI 자산 엔터프라이즈 카탈로그 중앙화, AI 에이전트·개발툴 자동 연계.

### [Azure API Management adds support for Agent-to-Agent (A2A) APIs](https://azure.microsoft.com/updates?id=562843)
- 에이전트간 JSON-RPC API 관리—보안/운영 통합 관점에서 신뢰도 향상.

### [Azure API Center supports agent registration, agent assessment, and Git-based synchronization](https://azure.microsoft.com/updates?id=562909)
- 에이전트 등록, 평가, Git 기반 동기화—자동화와 품질 관리를 통한 신속 배포 지원.

### [Azure API Management Premium v2 and Standard v2 wildcard custom hostnames](https://azure.microsoft.com/updates?id=562894)
- 와일드카드 호스트네임으로 대규모 도메인 관리 자동화, 운영복잡도 감소.

### [Azure Logic Apps MCP Server](https://azure.microsoft.com/updates?id=562868)
- Logic Apps 워크플로우를 MCP 도구로 공개, AI 에이전트와 직접 연동 가능.

**요약**: 통합 플랫폼은 API/에이전트/워크플로우/도메인 관리 및 품질 평가, 자동화와 보안정책 통합 등으로 대규모 AI와 API 운영을 효과적으로 통제하는 체계를 완성하고 있습니다.

---

## 🧩 Microsoft Foundry

Foundry 플랫폼은 AI 모델, 에이전트, 검색·지능 서비스의 통합 플랫폼으로 자리 잡고 있습니다. 대규모 모델 카탈로그, 도구·지식 소스 통합, 개발·운영 관점의 평가·벤치마크·옵서버빌리티 기능까지 전방위로 확장되고 있습니다.

### [Microsoft Foundry for Visual Studio Code (June Build 2026 refresh)](https://azure.microsoft.com/updates?id=563721)
- VS Code 기반 Foundry 환경—모델 카탈로그, 에이전트 배포, 스타터 코드 생성 등 개발자 생산성 극대화.

### [Content Understanding NextGen in Microsoft Foundry (Preview)](https://azure.microsoft.com/updates?id=563361)
- 문서 분석, 구조 정보 추출 등 실시간 AI 모델/도구와 시각적 통합 분석 환경 제공.

### [Foundry Memory preview refresh](https://azure.microsoft.com/updates?id=563616)
- 사용자·세션별 기억 저장소, 중복제거·TTL·관찰 기능 등 인공지능 특화 메모리 운영 체계 강화.

### [Toolbox connectors and triggers in Microsoft Foundry (Preview)](https://azure.microsoft.com/updates?id=563456)
- 이벤트 기반 AI 에이전트 자동화: 다양한 기업 시스템과 일정 트리거 연동.

### [MCP Server Knowledge Source in Microsoft Foundry IQ (Preview)](https://azure.microsoft.com/updates?id=563411)
- 외부 MCP 서버 연계 지식소스로 확장, Salesforce·Atlassian·Confluence 등 타 시스템 정보연동 자동화.

**요약**: Microsoft Foundry는 기업 AI 개발과 운영의 중심 플랫폼으로, 모든 서비스·프로토콜·도구 통합, 메모리 관리, 지식소스 연계, 사용자 피드백 기반 평가 등 AI 실무 전반을 커버하는 생태계를 제공합니다.

---

## 🏢 Microsoft Fabric 및 데이터 플랫폼

Microsoft Fabric은 OneLake·데이터 카탈로그, Ontology, Mirroring 기반 분석·AI 운영을 지원하며, Azure 및 Databricks·Foundry와 본격적인 연동이 이루어지고 있습니다.

### [OneLake catalog integration for Azure AI Search knowledge sources](https://azure.microsoft.com/updates?id=564407)
- OneLake 카탈로그를 AI Search 지식소스로 연계, 권한·민감도·소유권 연동 자동화.

### [Fabric IQ Ontology Knowledge Source in Microsoft Foundry IQ (Preview)](https://azure.microsoft.com/updates?id=563416)
- Fabric Ontology 기반 의미론적 지식소스, 엔터프라이즈 데이터에 기준된 AI 자동화 지원.

### [Azure Synapse Link for Azure Cosmos DB NoSQL 지원 종료](https://azure.microsoft.com/updates?id=558560)
- Synapse Link에서 Fabric Mirroring로 이행—제로 ETL, 데이터 동기화/분석 플랫폼 전환.

### [Azure Databricks natively storing data in Microsoft OneLake (Preview)](https://azure.microsoft.com/updates?id=565706)
- Databricks에서 OneLake로 직접 데이터 쓰기, 분석·AI 플랫폼간 데이터 중복 없이 연계.

### [Azure Databricks workspace-wide Genie MCP for Microsoft Copilot Studio (Preview)](https://azure.microsoft.com/updates?id=564868)
- Databricks 전체 워크스페이스를 대상으로 Copilot Studio에서 자연어 질의 구현.

**요약**: Fabric 플랫폼은 데이터 관리·연동·분석을 AI/앱 개발로 직결시키는 전사적 데이터 인프라를 실현하고 있습니다.

---

## 📊 관리 및 거버넌스, DevOps

운영관리 및 거버넌스 관련 업데이트는 모니터링 자동화, 동적 알림 임계값, 롤링 업데이트, SLI/SLO 도입, 대규모 마이그레이션, 정책 강화에 집중되어 있습니다.

### [Azure Monitor Service Level Indicators (SLI)](https://azure.microsoft.com/updates?id=565159)
- 서비스 경험을 기반으로 실제 사용자 지표(SLI)·목표(SLO) 설정 가능, 인프라 신호 중복 감소.

### [Dynamic threshold for Log search alerts](https://azure.microsoft.com/updates?id=561984)
- 머신러닝 기반 동적 임계값 자동 산출, 실시간 로그 모니터링 효율화.

### [Azure Migrate – GitHub Copilot Modernization integration for at scale code assessments (Preview)](https://azure.microsoft.com/updates?id=566145)
- GitHub Copilot과 연계한 코드 평가·현대화 분석, 마이그레이션 자동화 및 품질 고도화.

### [Azure Infrastructure Resiliency Manager (Preview)](https://azure.microsoft.com/updates?id=564759)
- 인프라 레질리언스 설계·점검 통합, AI 및 Azure Advisor, 모니터링, Chaos Studio, Copilot 연계.

### [Log Analytics Summary Rules experience](https://azure.microsoft.com/updates?id=562027)
- 대량 로그 요약·집계 자동화, 쿼리 효율 개선 및 데이터 프라이버시 향상.

**요약**: 관리 운영 전반에 자동화·지능화·정책 중심의 관리체계를 도입, 멀티클라우드·대규모 환경에 맞는 탄력적 거버넌스 지원이 이루어지고 있습니다.

---

## 👋 지원 종료(retirement) 및 사용자 공지

이번 달은 VM 시리즈, 스토리지 계정, NAT 규칙, Blueprints 등 특정 리소스의 지원 종료 및 사용 중단 공지가 다수 있었습니다. 신기능과의 구조적 충돌 예방 및 최신 플랫폼으로의 마이그레이션 안내가 주를 이룹니다.

### [Av2/F/G/Lsv2 등 구 VM 시리즈 Batch 지원 종료](https://azure.microsoft.com/updates?id=564774)
- 2028년 11월까지 기존 풀 운영 권장, 신규 생성 또는 스케일아웃 중단 예정. 대체 VM 시리즈로 이전 안내.

### [Azure Synapse Link for Cosmos DB NoSQL 지원 종료](https://azure.microsoft.com/updates?id=558560)
- 2029년 3월 EOL, Fabric Mirroring로 이전 권고.

### [GPv1 및 Legacy Blob Storage 계정 생성 종료](https://azure.microsoft.com/updates?id=564441)
- 2026년 6월 신규 생성 제한, 10월 자동 이관 및 비용 상승 가능.

### [Azure Blueprints 지원 종료(2027년 1월 전체 폐지)](https://azure.microsoft.com/updates?id=564806)
- 단계별 API/포털 사용 중단, 배포 스택/템플릿으로 이전 권장.

### [Azure VPN Client for Linux(Preview) 지원 종료](https://azure.microsoft.com/updates?id=565393)
- 2026년 8월 공식 종료, 대체 VPN 클라이언트로 이전 필요.

**요약**: 주요 인프라 및 개발도구의 지원종료(retirement) 공지는 최신 기술로의 이전, 비용 효율적·보안 중심 운영을 위한 필수 이행사항으로 강조되고 있습니다.

---

## 이번 달 총평 및 다음 달 전망

2026년 6월 Azure 업데이트는 AI, 데이터 플랫폼, 인프라, 통합, 거버넌스, 보안에 걸쳐 매우 폭넓은 진화를 보여줍니다. Foundry와 Fabric 등 Microsoft 중심의 플랫폼이 기업용 AI 및 데이터 전략의 중심을 잡아가고 있음을 확인할 수 있습니다. 지원종료(retirement) 공지와 프리뷰 신기술이 함께 발표되는 등, 하반기에는 레거시 시스템에서 최신 AI·데이터 기반으로의 적극적인 전환이 이어질 전망입니다. 다음 달에는 주요 서비스의 실제 현장 적용 사례와 프리뷰 기능의 GA 전환, 구 VM/스토리지 계정 대규모 마이그레이션 가이드, 신규 보안·콜라보레이션 기능 등이 더욱 강화될 것으로 기대됩니다. Azure 생태계는 점점 더 자동화, 일원화, 인텔리전트 통합 환경으로 진화해 나가고 있습니다.