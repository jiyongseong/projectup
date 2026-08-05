# Azure 월간 업데이트 요약 - 2026년 07월

## 전반적인 트렌드 및 핵심 인사이트

2026년 7월의 Azure 업데이트는 AI 및 데이터 분석, 컨테이너·Kubernetes 기반 관리, 보안 강화, 자동화 환경 업그레이드와 멀티클라우드 이행 지원이 전면적으로 확대되는 트렌드를 보여줍니다. 특히 Azure Databricks와 Microsoft Foundry, Microsoft Fabric 등 엔터프라이즈 AI와 데이터 서비스를 통한 높은 수준의 통합, 자동화, 거버넌스 도입이 돋보입니다.

AI 및 머신러닝 관련 서비스에서는 최신 AI 모델(Anthropic Claude Opus 5, Claude Sonnet 5, OpenAI GPT-5.6 등)의 빠른 정식 지원과 데이터 활용성 강화, 보안 및 컴플라이언스 대응이 중점적으로 이루어졌습니다. Kubernetes 관리 영역에서는 AKS 내 Gateway API 기반 라우팅, 리소스 자동 배치, 업데이트 실패 허용 범위 등 실무적 요구에 맞춘 기능들이 등장했습니다.

스토리지와 네트워킹 부문에서는 Blob Storage, Azure Files에서의 암호화 및 접근 제어, VPN 및 NAT Gateway의 IPv6 지원 등 인프라 현대화와 네트워크 탄력성이 더욱 강조되고 있습니다. 자동화 및 관리 측면에선 PowerShell 7.6 및 Python 3.14 정식 지원, Azure Automation의 런타임 환경 업그레이드 등 운영 효율성과 보안 강화가 두드러집니다.

공공·규제 산업과 글로벌 시장 대응을 위한 신규 데이터센터 출시, Confidential Computing·Enclave같은 고도의 보안 분리 환경 확대도 눈길을 끌었습니다. Microsoft Foundry/Build, Fabric 등 혁신 플랫폼은 도구집합 통합, 실시간 로그 미러링 등 조직 내 AI 및 데이터 활용의 새로운 표준을 제시하며, 멀티클라우드 및 하이브리드 시나리오에 최적화된 기능이 다수 추가되었습니다.

전반적으로 Azure는 민첩한 클라우드 인프라 구축과 엔터프라이즈 AI 활용, 자동화 및 SRE 관점의 운영 최적화, 고객 중심의 보안, 규제 컴플라이언스 대응 등 모든 영역에서 혁신을 이어가고 있습니다.

---

## ☁️ 컴퓨트, 컨테이너, 인프라

이번 달에는 Kubernetes와 Functions, Automation 등 핵심 인프라 서비스에서 정식 지원 및 중요한 기능 개선이 집중적으로 발표되었습니다.

### [Application Routing with Gateway API](https://azure.microsoft.com/updates?id=567944)
AKS에서 Kubernetes Gateway API를 통한 최신 애플리케이션 라우팅이 정식 지원되어 서비스 메시 없이 현대적 인그레스 관리가 가능해졌습니다.

### [Resource placement in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567931)
Fleet Manager에서 Kubernetes 리소스 배치를 자동화하여 다수 클러스터에 대한 일관된 배포·업데이트를 지원합니다.

### [Azure Functions support for Python 3.14](https://azure.microsoft.com/updates?id=567646)
Python 3.14를 사용하는 Azure Functions 개발·배포가 정식 지원되어 보안과 장기 라이프사이클 개선이 이루어집니다.

### [Azure Automation supports PowerShell 7.6 runbooks and Runtime environment](https://azure.microsoft.com/updates?id=568102)
PowerShell 7.6 기반 Runbook 및 런타임 환경, Azure CLI 명령어 지원 등 Azure Automation 운영 효율·보안이 대폭 향상되었습니다.

### [Public Preview: Azure Functions Support for PowerShell 7.6](https://azure.microsoft.com/updates?id=567651)
PowerShell 7.6 미리보기 런타임이 Functions에 지원되어 최신 스크립트·자동화 환경 적용이 가능해졌습니다.

요약:
올해 7월은 AKS·Fleet Manager·Functions 등에서 표준 API 기반 현대화, 리소스 자동배치, 최신 런타임생태계 적용을 통한 개발 효율성 및 보안 강화가 중심. 기존 인프라를 단계별로 현대화할 수 있도록 마이그레이션 지원 및 기존 환경과의 호환성을 강조합니다.

---

## 🔒 보안, 네트워킹, 컴플라이언스

네트워크 보안과 데이터 보호 전반을 아우르는 기능 업그레이드가 이루어졌습니다.

### [HTTP header insertion in Azure Firewall](https://azure.microsoft.com/updates?id=568115)
Azure Firewall에서 HTTP/HTTPS 헤더 삽입이 지원되어 엔트라 테넌트 제한 등 보안 및 접근제어 정책을 Native하게 적용할 수 있습니다.

### [IPv6 support for Azure VPN Gateway](https://azure.microsoft.com/updates?id=567847)
VPN Gateway에서 듀얼스택(IPv4/IPv6) 지원으로 네트워크 환경의 현대화 및 확장성을 강화합니다.

### [NAT64 on StandardV2 NAT Gateway](https://azure.microsoft.com/updates?id=568409)
NAT64 지원을 통해 IPv6 워크로드와 IPv4 목적지 간 통신이 NAT Gateway에서 직접 가능해졌습니다.

### [Azure DDoS Protection custom policy (미리 보기)](https://azure.microsoft.com/updates?id=568063)
DDoS 임계값을 직접 설정하는 맞춤 정책이 미리 보기로 제공되어, 트래픽 특성에 맞는 Anti-DDoS 대응 전략 수립이 가능해졌습니다.

### [Azure Enclave (미리 보기)](https://azure.microsoft.com/updates?id=568377)
정부 및 규제산업 맞춤 Azure Enclave가 미리 보기로 출시되어 네트워크 격리, 세분화된 접근제어, 관리 편의성 확대를 지원합니다.

요약:
방화벽·VPN·NAT·DDoS·Enclave 등 네트워크 및 인프라 보안이 대폭 강화되어 고객 별 니즈(테넌트 제한, IPv6, DDoS 대응, 규제 환경)에 맞춘 맞춤형 보안 전략 구축을 뒷받침합니다.

---

## 💾 스토리지, 데이터베이스, 이식/마이그레이션

스토리지와 데이터베이스 서비스에서 데이터 무결성, 암호화, 권한관리, 멀티클라우드 이식 등 혁신이 이어졌습니다.

### [Client-side data integrity protections in Azure Blob Storage](https://azure.microsoft.com/updates?id=566895)
Blob Storage SDK가 CRC64-NVME를 클라이언트까지 확장, 엔드-투-엔드 데이터 무결성 검증이 가능해졌습니다.

### [Azure Files NFS Shares Encryption in Transit for AKS](https://azure.microsoft.com/updates?id=567787)
AKS와 Azure Files NFS v4.1 볼륨 간 데이터 암호화 전송(Encryption in Transit) 정식 지원으로 보안 및 컴플라이언스 기준 강화.

### [Microsoft Entra ID-based access for Azure Blob Storage SFTP](https://azure.microsoft.com/updates?id=567085)
Entra ID 기반 SFTP 접근 권한 관리를 통해 운영 효율성과 외부 파트너 협업 보안이 개선되었습니다.

### [Azure Storage Mover supports migration from Google Cloud Storage](https://azure.microsoft.com/updates?id=566948)
Storage Mover가 GCS에서 Azure Blob Storage로의 클라우드 간 데이터 마이그레이션을 지원, 멀티클라우드 통합을 가속화합니다.

### [New Powershell module:  Az.PostgreSQLFlexibleServer](https://azure.microsoft.com/updates?id=566209)
PostgreSQL Flexible Server 관리용 PowerShell 모듈이 업데이트되어 PostgreSQL 18, 탄력적 클러스터 등 새로운 데이터 관리 방식을 제공합니다.

요약:
데이터 보호·권한 관리·암호화·클라우드 간 이식성을 중시하며, SDK·PowerShell·CLI 등의 도구 지원과 함께 자동화 체계를 확장합니다.

---

## 🤖 AI 및 머신러닝, 분석

초대형 언어모델 정식 지원, AI 에이전트 통합, 데이터 분석 플랫폼 확대 등 Azure AI 혁신이 집중적으로 나타났습니다.

### [Open AI GPT-5.6 on Azure Databricks](https://azure.microsoft.com/updates?id=567431)
Foundry 구매 모델로 Databricks AI 모델 서비스에 GPT-5.6이 정식 지원되어 엔터프라이즈 AI 활용 폭이 크게 넓어집니다.

### [Claude Opus 5 on Azure Databricks](https://azure.microsoft.com/updates?id=568316)
Anthropic Claude Opus 5 모델을 Databricks에서 AI 에이전트 빌드, 고급 추론·코딩 업무 등 다양한 시나리오에 사용할 수 있습니다.

### [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)
SQL Serverless 정식 지원으로 즉시 사용 가능한 분석 처리, 자동 확장, 간소화된 인프라 관리가 가능해집니다.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)
PII(개인정보 식별) 문서 샘플 Playground 정식 지원, 컴플라이언스·법무팀이 신속한 프로젝트 설계와 테스트가 가능해졌습니다.

### [Generally available: Anthropic Claude Sonnet 5 on Azure Databricks](https://azure.microsoft.com/updates?id=567194)
최신 Sonnet 5 모델이 Databricks에서 정식 지원되어, 저비용 고효율 코딩·에이전트 업무 등 AI 활용 확산을 지원합니다.

요약:
Azure는 AI 모델 접근성, 통합 플랫폼, 데이터·보안 연계, PII 평가 툴을 통해 조직 내 AI 활용 표준과 업무 생산성 혁신을 촉진하고 있습니다.

---

## 🛠️ Microsoft Foundry 및 Microsoft Build

Foundry와 Build 플랫폼에서 도구집합(툴박스), 문서 기반 PII 샘플, AI 안전성, 거버넌스 정책 등 내부 개발팀 표준화와 확장성을 위한 핵심 기능이 발표되었습니다.

### [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)
조직별 AI, MCP 서버, API, 커넥터 등을 통합·거버넌스 가능하도록 관리하는 툴박스 기능이 정식 지원됨.

### [Document PII playground sample in Microsoft Foundry NextGen](https://azure.microsoft.com/updates?id=563331)
Foundry 포털에서 샘플 문서 기반 PII 탐지 Playground를 제공, API 통합 전 신속한 기능 평가가 가능합니다.

### [Protect sensitive generative AI telemetry in Application Insights and Microsoft Foundry (미리 보기)](https://azure.microsoft.com/updates?id=567594)
Foundry·Application Insights에 AI 생성 데이터의 테이블별 제한 접근제어(GenAIContent table)가 추가되어 민감 AI 테이터 보호가 가능해졌습니다.

### [AI Gateway in Azure API Management (미리 보기)](https://azure.microsoft.com/updates?id=568184)
Foundry 기반 모델, MCP 서버, AWS/GCP/OpenAI 등 멀티 모델에 AI Gateway 통합 거버넌스·보안 관리 가능.

### [Azure Monitor Logs mirroring into Microsoft Fabric (미리 보기)](https://azure.microsoft.com/updates?id=568322)
Fabric으로 실시간 관측 로그 미러링이 가능해져, 비즈니스 데이터와 연관 분석·예측·머신러닝 활용성이 확장됨.

요약:
Foundry/Build 플랫폼은 조직 내 AI, 데이터, 보안, 거버넌스 체계의 혁신 기준으로 자리잡고 있으며, 다양한 표준화·확장 기능으로 업무 효율과 신뢰도를 높이고 있습니다.

---

## 📊 관리, 운영 자동화, DevOps

운영 관리 환경에서 자동화·Log Analytics·Chaos Studio 등의 기능이 혁신적으로 확장되고, 기존 런타임의 지원 종료 정책 안내와 클라우드 예약 정책 변경 등이 발표되었습니다.

### [Azure Site Recovery - Support 5x churn](https://azure.microsoft.com/updates?id=566966)
Site Recovery에서 500MB/s까지 IOPS를 지원, 고성능 워크로드의 재해 복구 신뢰성 대폭 개선됨.

### [Azure Chaos Studio Workspaces and Scenarios (미리 보기)](https://azure.microsoft.com/updates?id=567184)
Chaos Studio의 Workspace/Scenario 기반 실무적 장애 시나리오 시뮬레이션 자동화, 리포트 생성, RBAC 연계 지원.

### [Export historical data from Log Analytics workspace with Export jobs (미리 보기)](https://azure.microsoft.com/updates?id=566591)
Log Analytics Export Job을 통해 시기별 데이터 추출·외부 시스템 연계·규제 감사 대응 등이 지원됩니다.

### [Retirement: Support for Python-2.7/3.8, PowerShell-7.1/7.2](https://azure.microsoft.com/updates?id=567556)
2026년 9월 30일부터 자동화 런타임 환경에서 Python 2.7, 3.8, PowerShell 7.1/7.2 지원 종료. 보안 및 서비스 연속성을 위해 최신 런타임으로의 업그레이드가 필수.

### [Reservation exchanges for Azure services supported by savings plans will no longer be available](https://azure.microsoft.com/updates?id=568514)
2027년 2월부터 Savings Plan 적용 서비스(특히 VM, DB 등)의 예약 교환 기능이 중단됨. 교환권한은 마지막 1회만 적용.

요약:
운영/자동화 환경은 고성능·SRE 기반 장애 시뮬레이션, 데이터 추출·감사, 런타임 지원 정책 명확화 및 예약 정책의 변화에 맞춘 대응이 강조됩니다.

---

## 🌍 글로벌 및 지역(인도, 남미, 기타)

국가별·지역별 데이터센터, 인프라, 전문 서비스 확대에 초점이 맞춰졌습니다.

### [Azure Database for PostgreSQL flexible server in India South Central](https://azure.microsoft.com/updates?id=568334)
인도 South Central 신규 지역에서 PostgreSQL Flexible Server 지원, 멀티클라우드 DB 배포 폭 확대.

### [Microsoft Azure now available from new cloud region in India (India South Central)](https://azure.microsoft.com/updates?id=568013)
인도 Hyderabad 기반 Azure 데이터센터 신규 출시, AI Ready 인프라 및 로컬 레지던시·규제 대응.

### [Azure Red Hat OpenShift in Chile Central](https://azure.microsoft.com/updates?id=566732)
칠레 Central에서 OpenShift 완전 관리형 서비스 정식 지원, 남미 지역 현대화 클라우드 전환 강화.

### [Azure Sphere OS version 26.09 is now available for evaluation](https://azure.microsoft.com/updates?id=568466)
Azure Sphere OS 최신 버전(26.09) 평가판 배포, 장기 보안·커널 버전 업그레이드로 IoT 운영 신뢰성 강화.

### [Azure NetApp Files supports configuration of SMB opportunistic locking (Oplocks)](https://azure.microsoft.com/updates?id=568396)
SMB Oplock 설정 지원, 크로스리전 레플리케이션 시 볼륨 간 독립적 캐싱·성능 개선.

요약:
인도, 칠레 등 신규 클라우드 지역 출시 및 IoT 운영체제, 하이브리드 DB, 분산 파일 시스템의 지역 지원 확대로, 전 세계 고객의 사업 연속성과 현지 컴플라이언스 대응이 강화되었습니다.

---

## 총평 및 다음 달 전망

2026년 7월 Azure 업데이트는 AI 모델·분석, Kubernetes 표준화, 보안·컴플라이언스 강화, 자동화·운영 효율성, 글로벌 리전 확대 등 클라우드 인프라의 핵심 역량을 전방위적으로 확대하는 모습을 보여줍니다. 특히 Foundry, Databricks, Fabric 등 조직별 AI 및 데이터 서비스의 통합이 빠르게 표준화되고 있으며, 서비스 현대화와 보안 중심의 운영 관리가 업계 리더십을 더욱 공고히 합니다.

다음 달에는 AI/ML 모델 지원의 추가 확장, Kubernetes 관리 역량 심화, 환경별 자동화 도구 및 운영 인사이트 강화, 글로벌 지역 확대, 보안·네트워크 정책의 더욱 세분화된 적용이 예측됩니다. 기업마다 요구하는 맞춤형 클라우드 전략 및 AI 활용 기준이 고도화되며, Azure는 이를 선도하는 기능과 서비스를 지속적으로 발표할 것으로 전망됩니다.