# Azure 월간 업데이트 요약 - 2026년 07월

## 전반적인 트렌드 및 핵심 인사이트

2026년 7월 Azure 업데이트는 AI 및 머신러닝, 보안 강화, 클라우드 네이티브 인프라의 확장, 데이터 거버넌스, 운영 효율성 개선을 중심으로 이루어졌습니다. AI와 데이터 분석 기능이 Azure Databricks와 Microsoft Foundry를 통해 더욱 다각도로 확장되고 있으며, Anthropic Claude 및 OpenAI GPT-5.6 신규 모델 지원으로 엔터프라이즈 AI 도입의 진입 장벽이 낮아졌습니다. Azure Kubernetes Service, Red Hat OpenShift 등 컨테이너 기반 워크로드는 지역별 지원 확대(예: 인도, 칠레 등)와 관리 자동화, 표준 API 채택에서 혁신이 두드러집니다.

보안 영역에서는 네트워크 및 데이터 보호 기술이 대폭 강화되었습니다. Confidential Computing, Network Security Perimeter, HTTP header 삽입, IPv6 지원, NAT64 등 보안 아키텍처와 관리 자동화가 정식 지원되며, Key Vault에서는 대칭키 기능이 미리 보기로 제공되어 암호화 워크플로우의 유연성이 높아졌습니다. 자동화 운영에서는 PowerShell과 Python의 최신 버전 지원, 언어 지원 종료 정책 등 기술 생태계의 변화도 병행되었습니다.

관리 및 거버넌스 분야에서는 Azure Monitor와 Chaos Studio의 혁신적인 기능 미리보기가 등장하여, 복잡한 멀티클라우드 관측 및 장애 대응 시나리오에 더 높은 대응력이 확보되었습니다. 데이터베이스와 스토리지는 Azure Blob Storage의 클라이언트 데이터 무결성, Entra ID 통합, 네트워크 기반 접근제어 등이 도입돼 스토리지 솔루션의 신뢰성과 확장성이 강화되었습니다.

Microsoft Foundry, Fabric 등 신제품 카테고리에서는 데이터 분석·관찰 데이터 융합, 도구 관리 표준화, AI 기반 개인정보 탐지 등 조직의 데이터 및 AI 활용 역량이 극대화되고 있습니다. 인프라 및 지역서비스의 확장(인도·칠레 신규 리전)은 글로벌 비즈니스와 데이터 레지던시 요구에 부응하며, 기업들의 지역 기반 워크로드 전환을 더욱 촉진하고 있습니다.

이번 달 주요 인사이트는 다음과 같습니다:
- **AI/ML 본격 확산:** Azure Databricks·Foundry 신모델, AI Gateway 등 엔터프라이즈 AI 통합 지원 확대
- **네트워크 및 데이터 보안 강화:** Confidential Computing, NAT64, Network Security Perimeter 등 신규 기능 정식 지원
- **운영 자동화 및 개발 효율성:** 최신 PowerShell·Python 지원, 클러스터 관리 자동화, Kubernetes API 혁신
- **멀티클라우드·국가별 인프라 확대:** 인도·칠레 신규 리전 등 신흥시장 지원, 글로벌 서비스 분산
 
이런 트렌드는 조직의 클라우드 이전 전략, 데이터 분석·보안 역량 확장, AI와 DevOps 통합 가속화에 결정적으로 작용할 전망입니다.

---

## ☁️ 컴퓨트 및 컨테이너

이번 달 컴퓨트·컨테이너 카테고리는 AKS, Fleet Manager, Azure Functions 등 핵심 워크로드의 기능 현대화와 글로벌 확장에 집중됐습니다. 애플리케이션 라우팅 표준화, Python 3.14 지원, PowerShell 7.6 정식 지원, 노드 이미지 사전 준비 기능 등 개발·운영 효율성을 대폭 개선하였으며, 리소스 배치 자동화와 업데이트 실패 허용 설정 도입으로 대규모 클러스터 관리성이 크게 향상되었습니다.

### [Application Routing with Gateway API](https://azure.microsoft.com/updates?id=567944)
AKS에서 Gateway API 기반 애플리케이션 라우팅을 정식 지원하여, 서비스 메시 없이 표준 쿠버네티스 라우팅 모델 도입이 가능해졌습니다.

### [Azure Functions support for Python 3.14](https://azure.microsoft.com/updates?id=567646)
Azure Functions에서 Python 3.14 지원이 제공되어, 더욱 안전하고 장기 지원이 가능한 앱 개발이 가능해졌습니다.

### [Azure Automation supports PowerShell 7.6 runbooks and Runtime environment](https://azure.microsoft.com/updates?id=568102)
최신 PowerShell 7.6 런북 지원 및 런타임 환경 업그레이드 기능이 추가되어, 자동화 스크립트 관리의 안정성과 효율성이 제고되었습니다.

### [Resource placement in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567931)
Fleet Manager에서 리소스 배치 정책 기능이 정식 지원되어, 멀티 클러스터 환경에서 배포 및 업데이트의 일관성 관리가 용이해졌습니다.

### [Prepared Image Specification](https://azure.microsoft.com/updates?id=567949)
AKS 노드 이미지를 사전 준비하는 기능이 미리 보기로 제공되어, GPU·AI 등 대규모 워크로드의 노드 생성 지연 해소가 기대됩니다.

---

## 🔒 보안 및 네트워킹

7월에는 보안 및 네트워킹 기능이 강력하게 강화되었습니다. Confidential Computing, NAT64, HTTP 헤더 삽입, IPv6 대응, DDoS Protection 커스텀 정책, Azure Enclave 도입 등 데이터·네트워크 보호와 정책 기반 제어가 클라우드 서비스 전반에 적용되고 있습니다. 네트워크 경계, 최소 권한 접근, 가상 네트워크 분리 기능이 미리 보기와 정식 지원으로 배포되었습니다.

### [Confidential Computing support for Azure Event Hubs Dedicated](https://azure.microsoft.com/updates?id=567212)
Event Hubs Dedicated 환경에서 Confidential Computing 지원으로 데이터의 실시간 사용 보호가 가능해졌습니다.

### [HTTP header insertion in Azure Firewall](https://azure.microsoft.com/updates?id=568115)
Azure Firewall의 HTTP 헤더 삽입 기능이 제공되어, 인증·테넌트 제한·백엔드 연동 등 보안 및 운영 효율화를 지원합니다.

### [IPv6 support for Azure VPN Gateway](https://azure.microsoft.com/updates?id=567847)
VPN Gateway에서 IPv6 트래픽 지원이 추가되어, 듀얼 스택 네트워크 및 Site-to-Site, Point-to-Site 연결이 더욱 유연해졌습니다.

### [NAT64 on StandardV2 NAT Gateway](https://azure.microsoft.com/updates?id=568409)
NAT64 지원으로 IPv6 워크로드가 IPv4 전용 인터넷에 연결 가능하게 되어 네트워크 변화 및 현대화에 대응합니다.

### [Azure DDoS Protection custom policy (미리 보기)](https://azure.microsoft.com/updates?id=568063)
DDoS Protection에서 per-resource 커스텀 트래픽 임계값 정책이 적용되어, 대량 트래픽 이벤트·게임 업계·특수 워크로드 대응성이 향상되었습니다.

---

## 📊 데이터베이스 및 스토리지

데이터베이스와 스토리지 분야에서의 주요 업데이트는 PostgreSQL, Blob Storage, NetApp Files, Azure Files, Storage Mover 등에서 무결성, 보안 연동, 네트워크 암호화, 멀티클라우드 마이그레이션 지원, SDK 연동 강화가 이뤄졌습니다. 클라이언트 및 서버 측 데이터 일관성, Entra ID·RBAC·ABAC 기반 접근제어 등 기업 데이터 보안 요구에 부합하는 기술이 두드러집니다.

### [Client-side data integrity protections in Azure Blob Storage](https://azure.microsoft.com/updates?id=566895)
Blob Storage에서 CRC64-NVME 기반의 클라이언트 데이터 무결성 검증 기능이 SDK (.NET, C++, JS)에서 정식 지원됩니다.

### [Microsoft Entra ID-based access for Azure Blob Storage SFTP](https://azure.microsoft.com/updates?id=567085)
Blob Storage SFTP 접근에 Entra ID를 활용한 통합 인증·권한 관리가 도입되어 외부 협업 및 보안이 강화되었습니다.

### [Encryption in Transit for Azure Files NFS Shares in AKS](https://azure.microsoft.com/updates?id=567787)
AKS에서 Azure Files NFS v4.1 데이터의 TLS 암호화 지원이 정식화되어 데이터 이동·스토리지 사용 환경의 보안성이 높아졌습니다.

### [Azure Storage Mover now supports migration from Google Cloud Storage (미리 보기)](https://azure.microsoft.com/updates?id=566948)
Google Cloud Storage에서 Azure Blob Storage로의 마이그레이션이 지원되어, 멀티클라우드 데이터 통합이 쉬워졌습니다.

### [Support for SMB Opportunistic Locking (Oplocks) configuration (미리 보기)](https://azure.microsoft.com/updates?id=568396)
Azure NetApp Files에서 SMB Oplocks 설정 지원으로, 볼륨 관리·성능·복제 효율성이 개선되었습니다.

---

## ⚡️ AI + 머신러닝 및 분석

AI 및 분석에서는 Azure Databricks, AI Gateway, Microsoft Foundry를 중심으로 고성능 모델과 도구, 개인정보 검출, AI 기반 로그 분석 등 혁신이 이루어졌습니다. Anthropic Claude, OpenAI GPT, AI Gateway, Document PII Playground, Fabric 연동 등 차별화된 모델 지원 및 실무 데이터 활용 시나리오가 강화되었습니다.

### [Claude Opus 5 on Azure Databricks](https://azure.microsoft.com/updates?id=568316)
Azure Databricks에서 Anthropic Claude Opus 5 지원으로 복잡한 AI 작업과 앱 개발에 고차원 모델 활용이 가능해졌습니다.

### [Open AI GPT-5.6 on Azure Databricks](https://azure.microsoft.com/updates?id=567431)
GPT-5.6 모델이 Databricks에서 사용 가능해져, 첨단 AI 워크플로우 구축 및 Foundry 연계가 가능합니다.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)
Document PII 검출 Playground 정식화로 개인식별 정보 검출 및 컴플라이언스 프로젝트 평가 속도가 향상되었습니다.

### [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)
Databricks SQL Serverless가 UK West 지역에서 지원되어 분석 업무의 확장성과 인프라 자동화가 가속화됩니다.

### [Azure Monitor Logs mirroring into Microsoft Fabric (미리 보기)](https://azure.microsoft.com/updates?id=568322)
Azure Monitor 분석 로그를 Fabric으로 실시간 공유 가능해져 통합 관찰·운영·비즈니스 분석 파이프라인 구성이 쉬워졌습니다.

---

## 🛠️ 관리 및 거버넌스

이번 달 관리 및 거버넌스 업데이트는 자동화 플랫폼 개편, 운영 효율화, 예약 정책 변경, 데이터베이스 및 사이트 복구 성능 강화, Chaos Studio 미리 보기 등 조직의 클라우드 오케스트레이션·자동화 역량 향상에 중점을 두었습니다. 최신 언어 지원, 운영 모듈 개선, 장애 시나리오 테스트 확대, 정책·컴플라이언스 강화가 주요 특징입니다.

### [Reservation exchanges for Azure services supported by savings plans will no longer be available starting February 1, 2027](https://azure.microsoft.com/updates?id=568514)
Savings Plans 적용 서비스에 대한 예약 교환이 내년부터 중단되어 비용 관리 관행 변화가 예고됩니다.

### [Support 5x churn in Azure Site Recovery](https://azure.microsoft.com/updates?id=566966)
Azure Site Recovery에서 VM당 500MB/s까지의 고속 데이터 변경 지원이 추가되어 재해복구 성능이 크게 향상됩니다.

### [Azure Chaos Studio Workspaces and Scenarios (미리 보기)](https://azure.microsoft.com/updates?id=567184)
Chaos Studio에서 워크스페이스·시나리오 기능 미리 보기로 실제 장애 패턴 테스트 및 보고 자동화가 가능해졌습니다.

### [Retirement: Support for Python-2.7; 3.8 and PowerShell- 7.1; 7.2 will be retired on September 30, 2026](https://azure.microsoft.com/updates?id=567556)
자동화에서 Python 2.7, 3.8, PowerShell 7.1·7.2 지원이 9월 말 종료됨에 따라 최신 버전으로 전환이 필수화됩니다.

### [Manage Azure Chaos Studio from the Azure CLI (미리 보기)](https://azure.microsoft.com/updates?id=567225)
Azure CLI에서 Chaos Studio 시나리오 생성·실행이 가능해져 운영 자동화와 장애 대응의 효율성이 극대화됩니다.

---

## 🤖 Microsoft Foundry

Microsoft Foundry 카테고리는 AI 기반 개인정보 검출, 도구 표준화, API 평가·연동 등 에이전트 중심 개발 환경 혁신이 두드러졌습니다. Toolboxes 정식 지원, PII Playground, API 연동·정책·거버넌스를 통한 조직 내 AI 자산 재사용성과 관리 용이성이 대폭 개선되었습니다.

### [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)
Toolboxes를 정식 지원하며, 표준화된 도구 번들 관리 및 재사용, 에이전트 거버넌스가 편리해졌습니다.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)
Foundry에서 빠른 문서 개인정보 검출 샘플과 평가 환경이 도입되어 컴플라이언스 AI 프로젝트의 효율성이 높아졌습니다.

### [Public Preview: Document PII playground sample in Microsoft Foundry NextGen](https://azure.microsoft.com/updates?id=563331)
Foundry NextGen에서 개인정보 검출 샘플 Playground 미리 보기로 실용적인 문서 평가 및 API 통합이 가능해졌습니다.

### [Protect sensitive generative AI telemetry in Application Insights and Microsoft Foundry (미리 보기)](https://azure.microsoft.com/updates?id=567594)
Application Insights와 Foundry에서 AI 생성 콘텐츠(PII 등) 접근 제한 기능으로 규제 산업 활용성과 개인정보 보호가 강화되었습니다.

### [AI Gateway in Azure API Management (미리 보기)](https://azure.microsoft.com/updates?id=568184)
Foundry·AWS·Google AI 모델 연동, 체계적인 정책 적용, 모델 제어권 제공 등 AI Gateway 미리 보기로 조직별 AI 자산 관리 효율성이 극대화됩니다.

---

## 🧩 Microsoft Fabric

Fabric 관련 주요 업데이트는 데이터 분석, 관찰 데이터 융합, 로그 분석 통합 시나리오의 가속화를 이끌었습니다. Azure Monitor 로그를 Fabric으로 미러링하는 기능이 미리 보기로 제공되며, 기존 운영 데이터와 비즈니스 데이터를 통합 분석하는 조직 중심 데이터 전략 구축이 가능해집니다.

### [Azure Monitor Logs mirroring into Microsoft Fabric (미리 보기)](https://azure.microsoft.com/updates?id=568322)
Azure Monitor Log Analytics 로그 데이터를 OneLake의 개방형 포맷으로 바로 연동하여, Fabric 기반 실시간 분석 체계가 이루어집니다.

---

## 🌍 국가별 업데이트 (한국 관련 없음)

2026년 7월에는 인도 South Central, 칠레 Central 신규 리전에서 Azure 서비스 지원이 확대되었습니다. 한국에서 특화된 업데이트는 포함되지 않았으나, 글로벌 리전 확장은 데이터 레지던시, 규제, 현지화 전략에 더욱 유리한 환경을 제공합니다.

---

## 총평 및 다음 달 전망

7월 Azure 업데이트는 AI 및 데이터 분석의 확장, 강력한 보안·네트워킹 기능 도입, 멀티클라우드·자동화 플랫폼 혁신이 중심이었습니다. 엔터프라이즈 환경의 복잡한 요구에 맞춰, 최신 버전·운영 효율성·데이터 무결성·보안·컴플라이언스 기준이 한층 높아지고 있습니다. Foundry·Fabric 등 신제품군의 체계적인 도입은 데이터와 AI 활용의 조직 내 표준화, 제어, 재사용성을 크게 개선시키고 있습니다.

향후 업데이트에서는 AI Gateway 정식화, 국가별 신규 리전 지원 확대, 기존 언어의 지원 종료 정책 적용, 네트워크·보안 기능 매니지드화, Fabric을 통한 데이터 융합 분석 체계 확장 등이 기대됩니다. 조직별 클라우드 전략, AI 및 운영 자동화 도입, 지역별 데이터 인프라 투자 방향에 결정적인 영향을 미칠 것으로 전망됩니다.