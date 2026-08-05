# Azure 월간 업데이트 요약 - 2026년 07월

## 전반적인 트렌드 및 핵심 인사이트

2026년 7월 Azure 업데이트는 클라우드 인프라의 대대적 현대화, AI 및 데이터 분석 서비스의 차별화, 네트워크·보안 기능의 고도화, 자동화 플랫폼의 다양성과 표준화, 그리고 글로벌 리전 확장 및 규제 산업 대응 등 다양한 이슈를 담고 있습니다.  
특히 ▲Kubernetes, AKS, Fleet Manager 등 컨테이너 관리와 오케스트레이션의 신규 기능, ▲Azure Databricks와 Microsoft Foundry를 중심으로 AI 모델 및 에이전트 도입 확산, ▲Storage, Networking, Security 분야의 고객 중심 파일럿 기능과 보안 강화가 두드러집니다.

실무 관점에서 가장 눈에 띄는 흐름은 데이터 보호와 데이터 무결성, 그리고 미리 보기 기능에서 운영 환경까지의 안전한 전환 지원입니다. Standardized Gateway API, 에이전트 ToolBox, AI Gateway 등은 클라우드 내 워크로드 통합과 관리 효율성을 높이고, 신규 Python·PowerShell 지원 및 지원 종료 정책 발표는 자동화 워크플로의 기술 갱신에 대한 실무적 요구를 반영합니다.

또한, 지역 확장(인도 South Central, 칠레 Central 등)은 글로벌 고객의 로컬 요구에 부응하며, 전통적인 서비스와 신흥 AI·데이터 서비스 간 경계가 점차 줄어드는 인프라 융합 트렌드가 감지됩니다.  
마지막으로, Microsoft Fabric 및 Foundry와 Azure 핵심 서비스의 통합적 업데이트는 고객이 보안·컴플라이언스와 혁신을 동시에 달성할 수 있도록 설계된 것이 특징입니다.

## 카테고리별 업데이트

---

## 🚀 출시 및 정식 지원

전통적인 Azure 서비스와 신규 오퍼링 모두에서 많은 정식 지원(General Availability)이 이루어졌습니다.  
Kubernetes, Fleet Manager, Databricks, Storage, Networking 등 클라우드 엔터프라이즈 구성이 표준화되고 기능이 강화되는 흐름이 확인됩니다.

### [Application Routing with Gateway API](https://azure.microsoft.com/updates?id=567944)  
AKS의 애플리케이션 라우팅에서 Gateway API가 정식 지원되어 서비스 메시 없이 표준화된 인그레스 관리가 가능합니다.

### [Azure Automation supports PowerShell 7.6 runbooks and Runtime environment](https://azure.microsoft.com/updates?id=568102)  
PowerShell 7.6 런북 및 런타임 환경 지원으로 자동화 스크립트의 보안과 이식성이 획기적으로 개선되었습니다.

### [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)  
UK West 리전에서 Serverless SQL 웨어하우스가 기본 옵션으로 제공되어 데이터 분석 및 인프라 관리가 더욱 편리해졌습니다.

### [Azure Functions support for Python 3.14](https://azure.microsoft.com/updates?id=567646)  
Python 3.14 지원으로 앱 개발의 최신 보안과 장기 지원이 가능해졌습니다.

### [Azure Red Hat OpenShift in Chile Central](https://azure.microsoft.com/updates?id=566732)  
칠레 중앙 리전에서 OpenShift 사용이 가능해져 규제 산업에 대응한 현지 실행 환경이 확대되었습니다.

---

## 🤖 AI 및 머신러닝 / 분석

AI 모델과 분석 서비스의 급진적 확산이 이루어지고 있습니다. Databricks, Microsoft Foundry, Azure AI Language 등에서 대규모 AI 모델, agentic 에이전트, PII 플레이그라운드가 정식 지원되어 엔터프라이즈 AI 활용 폭이 넓어졌습니다.

### [Claude Opus 5 on Azure Databricks](https://azure.microsoft.com/updates?id=568316)  
최신 Claude Opus 5 모델을 Databricks AI Model Serving에서 사용할 수 있어 고도의 인공지능 개발에 적합합니다.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)  
PII 검출 기능이 개선되어 컴플라이언스 평가 속도와 정확성이 크게 향상되었습니다.

### [Open AI GPT-5.6 on Azure Databricks](https://azure.microsoft.com/updates?id=567431)  
GPT-5.6을 Databricks Model Serving Endpoint에서 활용 가능하며, 데이터 거버넌스가 통합 지원됩니다.

### [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)  
Foundry Toolboxes가 에이전트 개발에 표준화된 도구 집합을 제공, 조직별 재사용과 거버넌스가 간소화되었습니다.

### [Anthropic Claude Sonnet 5 on Azure Databricks](https://azure.microsoft.com/updates?id=567194)  
클라우드 Sonnet 5 모델로 고성능·경제성이 강조된 AI 코딩, 에이전트 워크플로를 지원합니다.

---

## 🛠️ 관리 · 자동화 · 거버넌스

자동화, 이관, 장애 대응, 예약 정책 등 실무적 관리 기능이 강화되고 표준화되었습니다. PowerShell 및 Python 런북 지원, Site Recovery 고효율화, 예약 정책 변경 등은 대규모 운영 환경을 겨냥한 최적화의 흐름입니다.

### [Azure Site Recovery – Support 5x churn](https://azure.microsoft.com/updates?id=566966)  
Azure Site Recovery가 5배 향상된 변경율을 지원해 고IOPS 워크로드의 재해복구 신뢰성이 대폭 강화되었습니다.

### [Microsoft Defender security assessments for PostgreSQL Flexible Server](https://azure.microsoft.com/updates?id=567527)  
Defender CSPM 평가 기능이 PostgreSQL에 최적화되어 보안 취약점 점검과 컴플라이언스 지원이 용이해졌습니다.

### [New Powershell module: Az.PostgreSQLFlexibleServer](https://azure.microsoft.com/updates?id=566209)  
신규 PowerShell 모듈로 PostgreSQL 18, 탄력적 클러스터 등 최신 기능을 효율적으로 관리할 수 있습니다.

### [Resource placement in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567931)  
Fleet Manager의 리소스 배치 기능으로 클러스터 간 일관된 운영·배포가 자동화되었습니다.

### [Reservation exchanges for Azure services supported by savings plans will no longer be available](https://azure.microsoft.com/updates?id=568514)  
2027년 2월부터 Savings Plan이 적용된 서비스의 예약 교환 정책이 종료되어, 비용 전략 관리에 주의가 필요합니다.

---

## 🛡️ 네트워킹 · 보안 · 컴플라이언스

네트워크·보안 기능의 강화와 컴플라이언스 대응이 주요 흐름입니다. NAT64, IPv6, Event Hubs Confidential Computing, Azure Firewall, VPN Gateway의 신기능은 클라우드 네트워크 전환을 뒷받침합니다.

### [HTTP header insertion in Azure Firewall](https://azure.microsoft.com/updates?id=568115)  
Azure Firewall에서 HTTP 헤더 삽입 기능을 지원, 보안·접근 정책의 유연성이 확대되었습니다.

### [IPv6 support for Azure VPN Gateway](https://azure.microsoft.com/updates?id=567847)  
VPN Gateway의 IPv6 지원으로 듀얼 스택 환경과 장기 확장을 대비할 수 있습니다.

### [NAT64 on StandardV2 NAT Gateway](https://azure.microsoft.com/updates?id=568409)  
NAT64를 통한 IPv6-IPv4 통신이 지원되어 하이브리드 인프라의 연결성이 크게 향상되었습니다.

### [Confidential Computing support for Azure Event Hubs Dedicated](https://azure.microsoft.com/updates?id=567212)  
Event Hubs Dedicated에서 Confidential Computing 지원으로 데이터의 인메모리 보호가 가능해졌습니다.

### [Network Security Perimeter support for Azure Event Hubs](https://azure.microsoft.com/updates?id=567203)  
Event Hubs NSP 기능으로 네트워크 경계 기반 접근제어 및 데이터 유출 방지가 강화되었습니다.

---

## 📦 스토리지 · 데이터 · SDK

스토리지 서비스에서 데이터 무결성, 암호화, 이관, SDK 등 다양한 기능이 출시됐습니다. Blob Storage, Azure Files, Storage Mover, NetApp Files 등은 대용량 데이터와 네트워크 마이그레이션 활용도를 높였습니다.

### [Client-side data integrity protections in Azure Blob Storage](https://azure.microsoft.com/updates?id=566895)  
Blob SDK를 통한 클라이언트 단 데이터 무결성 체크로 엔드 투 엔드 데이터 검증이 가능해졌습니다.

### [Encryption in Transit for Azure Files NFS Shares in AKS](https://azure.microsoft.com/updates?id=567787)  
AKS에서 Azure Files NFS 볼륨의 전송 중 암호화(EiT)를 지원, 보안 및 컴플라이언스 요구에 대응합니다.

### [Microsoft Entra ID-based access for Azure Blob Storage SFTP](https://azure.microsoft.com/updates?id=567085)  
SFTP 접속 시 Entra ID 인증 및 조건부 액세스 적용으로 운영 관리 효율성과 보안이 극대화되었습니다.

### [Azure Storage Mover now supports migration from Google Cloud Storage](https://azure.microsoft.com/updates?id=566948)  
Google Cloud Storage에서 Azure Blob Storage로 클라우드-클라우드 이관이 지원되어 멀티클라우드 통합과 보안적 데이터 마이그레이션이 간소화되었습니다.

### [Azure Sphere OS version 26.09 is now available for evaluation](https://azure.microsoft.com/updates?id=568466)  
Sphere OS 26.09 평가 버전으로 Linux 커널 대형 업데이트가 장기 지원·보안 중심으로 이루어졌습니다.

---

## 🧑‍💼 Microsoft Foundry / Microsoft Fabric

AI Governance, ToolBox, PII 샘플 등 Foundry 특화 기능과 Azure Monitor 로그의 Fabric OneLake 실시간 미러링 등 혁신적 통합 솔루션이 출시됐습니다.

### [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)  
Toolbox 기능으로 표준 Tool 집합을 MCP 서버/커넥터 등에 쉽게 적용 가능, 조직 전체 거버넌스가 구현됩니다.

### [Document PII Playground in Azure AI Language (Foundry NextGen)](https://azure.microsoft.com/updates?id=563331)  
PII 검출 샘플이 Foundry NextGen에 도입되어 빠르고 직관적인 컴플라이언스 테스트가 가능해졌습니다.

### [Protect sensitive generative AI telemetry in Application Insights and Microsoft Foundry](https://azure.microsoft.com/updates?id=567594)  
GenAIContent 테이블과 Role 기반 접근제어로 AI 텔레메트리 보호 및 규제 산업 대응이 더욱 강화되었습니다.

### [Azure Monitor Logs mirroring into Microsoft Fabric](https://azure.microsoft.com/updates?id=568322)  
Azure Monitor Log 데이터를 Fabric OneLake에 실시간 미러링, 이벤트 분석·머신러닝·BI 통합 적용 가능성이 크게 늘었습니다.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)  
컴플라이언스팀이 신속하게 PII 프로젝트 범위 설정이 가능, AI 기반 문서 보호 및 평가가 간소화되었습니다.

---

## 🧪 미리 보기 기능 (Preview)

데이터 관리, AI 연동, 네트워크·보안 강화 등 다양한 미리 보기 기능이 선보이고 있습니다. 적용을 위한 실험과 커뮤니티 피드백이 적극 반영되는 점이 특징입니다.

### [AI Gateway in Azure API Management](https://azure.microsoft.com/updates?id=568184)  
AI Gateway 전용 Tier가 공개되어 AI 워크로드의 보안, 정책, 인증, 관측제어가 통합적으로 제공됩니다.

### [Azure Chaos Studio Workspaces and Scenarios](https://azure.microsoft.com/updates?id=567184)  
Chaos Studio의 워크스페이스·시나리오 기능으로 실제 장애 패턴을 손쉽게 테스트할 수 있습니다.

### [Azure DDoS Protection custom policy](https://azure.microsoft.com/updates?id=568063)  
DDoS 보호 정책 사용자 지정 기능으로 트래픽 유형별 임계값을 세분화해 맞춤 보안이 가능합니다.

### [Azure Enclave](https://azure.microsoft.com/updates?id=568377)  
민감한 워크로드를 위한 격리 환경 지원으로 정부 및 규제 산업의 보안·접근제어가 강화됩니다.

### [Azure Front Door edge actions](https://azure.microsoft.com/updates?id=567402)  
서버리스 Edge Actions로 실시간 요청 처리/필터링이 가능, 고성능·보안·유연성이 실현됩니다.

---

## 총평 및 다음 달 전망

이번 7월 Azure 업데이트는 클라우드 전반의 혁신과 운영 효율화, 보안·데이터 거버넌스 강화, 그리고 AI와 자동화의 실무 도입 확산이 두드러진 한 달이었습니다.  
신규 기능들의 ‘정식 지원’ 본격화, 미리 보기(Preview)에서 실운영 환경으로의 전환 준비, 지역적 인프라 확대 등 구체적 변화가 나타납니다.  
관리 자동화, 네트워크 보안, 멀티클라우드 이관, 컴플라이언스 대응 등 실무에서 꼭 필요한 기능이 다수 편입된 점은, Azure 클라우드가 엔터프라이즈 혁신과 안정적인 서비스 운영에 더욱 최적화되고 있음을 보여줍니다.

다음 달 전망은 AI 및 데이터 중심 서비스와 보안·컴플라이언스 강화 기조가 더욱 구체화될 것으로 예상됩니다.  
특히 Foundry/Fabric 통합 솔루션, Kubernetes 환경 내 효율·신뢰성 극대화, 글로벌 리전 확대 정책 등은 Azure의 경쟁력을 지속 강화할 것으로 보입니다.  
Preview 기능에 대한 커뮤니티 피드백과 적용 사례 역시 실무 운영자와 개발자에게 중요한 선택 기준이 될 전망입니다.