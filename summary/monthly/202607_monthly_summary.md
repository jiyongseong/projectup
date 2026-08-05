# Azure 월간 업데이트 요약 - 2026년 07월

## 트렌드 및 핵심 인사이트

2026년 7월의 Azure 업데이트는 클라우드 네이티브 현대화, AI 및 분석 인프라의 확장, 보안·컴플라이언스 강화, DevOps 및 관리 자동화, 하이브리드 및 멀티 클라우드 지원, 지역 확장, 전문 서비스형 툴 제공 등의 주요 트렌드를 명확히 보여주고 있습니다.

먼저, Kubernetes 관련 기능의 정식 지원과 관리 효율화로 클러스터 운영의 일관성과 확장성을 극대화하는 방향이 뚜렷합니다. AKS의 Gateway API 기반 애플리케이션 라우팅과 Kubernetes Fleet Manager의 리소스 배치 관리 등은 대규모 멀티 클러스터 환경을 위한 표준화된 정책과 운영 도구를 제공하여 기업의 클라우드 네이티브 도입을 본격적으로 가속화합니다.

AI 및 데이터 분석 영역에서는 Databricks 기반의 Anthropic Claude/Opus 신모델, GPT-5.6, SQL Serverless 등이 강화되며, 모델 서빙 통합과 자동화된 워크플로우 도입이 두드러집니다. Microsoft Foundry와 연결된 GPT 모델, Toolboxes, PII 검출 등 고도화된 AI 활용과 서비스 연계도 눈에 띕니다. AI Gateway 등 API Management 연동도 확대되며, Fabric 데이터 플랫폼으로 Azure Monitor Log Analytics가 실시간으로 연동되어 크로스도메인 데이터 분석이 용이해졌습니다.

보안과 컴플라이언스에서는 Confidential Computing, 네트워크 경계(Perimeter) 정책, Entra ID 기반 인증, DDoS Protection, Key Vault 대칭키 지원 등이 강화되었습니다. 데이터 전송 암호화, Blob Storage 데이터 무결성, Firewall 헤더 제어, VPN IPv6, NAT64 등 인프라 보안과 네트워크 유연성이 전반적으로 향상되었습니다.

DevOps, 관리 자동화 측면에서는 PowerShell 7.6, Python 3.14 및 언어 런타임 정식 지원, Site Recovery 고성능화, Chaos Studio CLI·Workspace, Storage Mover 기능 등 변화가 두드러지며, 관련된 지원 종료 계획(일부 Python, PowerShell 런타임) 등 수명 주기 관리가 투명하게 이루어지고 있습니다.

하이브리드 및 멀티 클라우드 지원은 Az.PostgreSQLFlexibleServer 파워셸 모듈, Storage Mover의 GCS→Blob 지원 등으로 확대되며, 지역별 신규 서비스 출시(인도 South Central, 칠레 Central, 영국 West Databricks Serverless 등)는 글로벌 확장과 현지화 노력의 산물입니다.

Microsoft Foundry와 Fabric, 그리고 API Gateway 등 서비스형 구성이 강조되면서, 개발 및 운영 로드 감소, 표준 도입, 거버넌스 및 재사용성 확보가 주요 IT 트렌드로 자리잡았습니다. 이처럼 Azure는 전략적으로 “실질적 현대화·운영 효율·보안 최적화·AI 기반 혁신·글로벌 확장”이라는 핵심 방향에 초점을 맞춘 업데이트를 이어가고 있습니다.

---

## 🖥️ 컴퓨트 & 컨테이너

클라우드 네이티브 현대화를 선도하며, AKS와 Azure Functions, Kubernetes Fleet Manager 등에서 신규 기능과 운영 정책의 표준화가 이뤄지고 있습니다. 개발 언어 지원 강화와 직접적 보안 기능 제공도 주요 변화입니다.

---

### [Application Routing with Gateway API](https://azure.microsoft.com/updates?id=567944)
AKS에서 Gateway API 기반의 애플리케이션 라우팅 정식 지원으로 Kubernetes 표준 ingress 관리가 강화되었습니다. 기존 nginx 기반 라우팅은 11월까지 지원되며, 점진적 마이그레이션이 가능합니다.

### [Azure Functions support for Python 3.14](https://azure.microsoft.com/updates?id=567646)
Azure Functions에서 Python 3.14를 사용할 수 있게 되어, 개발자가 최신 언어 버전을 활용하며 보안·성능 혜택을 누릴 수 있습니다. 업그레이드와 롱텀 지원이 강화됩니다.

### [Public Preview: Azure Functions Support for PowerShell 7.6](https://azure.microsoft.com/updates?id=567651)
PowerShell 7.6 런타임의 미리 보기 지원을 통해 Functions의 스크립트 개발 환경이 최신화됩니다. 향후 정식 지원 예정으로, 언어 관련 퇴출 정책과 연계됩니다.

### [Resource placement in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567931)
Fleet Manager의 리소스 배치 기능이 정식 지원되며, 멀티 클러스터 환경에서 일관된 리소스 설정·배포가 가능해지고, 플랫폼팀의 관리 효율성이 크게 향상됩니다.

### [Maximum allowed failures for update runs in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567939)
업데이트 실패 허용 범위 설정(프리뷰)으로, 대규모 클러스터 업데이트 시 일부 실패 상황에서 롤아웃을 지속할 수 있게 되어, 운영 탄력성과 자동화 전략이 더 견고해집니다.

---

## 💾 스토리지 & 네트워킹

데이터 무결성, 전송 암호화, 네트워크 기능 확장 등 스토리지 및 네트워크 서비스가 현대적 인프라 요구에 맞게 진화하고 있습니다. 보안 및 인증, 특수 네트워킹 지원이 전반적으로 강화됩니다.

---

### [Client-side data integrity protections in Azure Blob Storage](https://azure.microsoft.com/updates?id=566895)
Blob Storage SDK에서 CRC64-NVME 체크섬으로 애플리케이션 레벨 데이터 무결성 검증이 가능해졌습니다. 엔드 투 엔드 데이터 보호로 컴플라이언스 및 보안이 강화됩니다.

### [Encryption in Transit for Azure Files NFS Shares in AKS](https://azure.microsoft.com/updates?id=567787)
AKS의 Azure Files NFS v4.1 데이터 전송 암호화(TLS)가 정식 지원됨으로써, 민감한 데이터의 규제·보안 요건을 충족하고, 애플리케이션은 변경 없이 사용할 수 있습니다.

### [Microsoft Entra ID-based access for Azure Blob Storage SFTP](https://azure.microsoft.com/updates?id=567085)
Blob Storage SFTP에 Entra ID 인증이 적용되어, MFA·조건부 액세스 및 외부 협업이 더 안전하고 효율적으로 보장되는 통합 인증 체계가 완성되었습니다.

### [IPv6 support for Azure VPN Gateway](https://azure.microsoft.com/updates?id=567847)
VPN Gateway에서 IPv6 듀얼 스택과 Site-to-Site, Point-to-Site VPN 모두 지원되어, 차세대 네트워크 요구에 맞는 글로벌 연결성과 현대화된 인프라 구현이 가능해졌습니다.

### [NAT64 on StandardV2 NAT Gateway](https://azure.microsoft.com/updates?id=568409)
NAT64 도입으로 IPv6 워크로드가 IPv4 전용 인터넷과 매끄럽게 통신할 수 있게 되었으며, DNS64 통합으로 하이브리드 네트워크 확장을 간편하게 지원합니다.

---

## 🔒 보안 & 컴플라이언스

Persistent 및 실시간 데이터 보호, 네트워크 보안 강화, 권한 인증/관리, 워크로드 경계 설정 등 다양한 범위의 보안 및 컴플라이언스 혁신이 이루어졌습니다.

---

### [Confidential Computing support for Azure Event Hubs Dedicated](https://azure.microsoft.com/updates?id=567212)
Event Hubs Dedicated가 Confidential Computing을 정식 지원하여, 메모리 내 데이터도 하드웨어 기반 TEE로 보호합니다. 민감한 스트리밍 데이터의 보안을 크게 강화합니다.

### [HTTP header insertion in Azure Firewall](https://azure.microsoft.com/updates?id=568115)
Firewall에서 HTTP 헤더 삽입이 가능해져, 세분화된 보안 정책 적용 및 클라우드 기반 앱 액세스 관리가 유연해지고, 엔터프라이즈 시나리오 대응력이 개선됩니다.

### [Azure DDoS Protection custom policy](https://azure.microsoft.com/updates?id=568063)
DDoS Protection의 맞춤 정책(프리뷰)은 프로토콜별 임계값을 직접 구성해 예측 가능한 고유 트래픽과 대규모 이벤트 대응이 가능하게 합니다.

### [Azure Enclave](https://azure.microsoft.com/updates?id=568377)
Azure Enclave 프리뷰로, 네트워크 인프라의 기본 격리 및 다중 보안 제어, 민감 데이터·특수 워크로드를 위한 관리형 아키텍처가 제공되어 규제 산업 대응이 용이해집니다.

### [Symmetric keys on Azure Key Vault Premium](https://azure.microsoft.com/updates?id=566746)
Key Vault Premium에서 대칭키 및 AES 알고리즘(프리뷰)이 지원되어, 중앙집중식 키 관리와 포스트퀀텀 보안 준비, 신뢰성 있는 암호화 환경이 강화되었습니다.

---

## 📊 분석 & AI + 머신러닝

데이터 플랫폼 혁신, 고급 AI 모델 서빙·통합, 프라이버시 보호·검출, 실시간 분석과 관리 자동화가 크게 진화하며, AI 도입의 현실적 가치를 높이고 있습니다.

---

### [Claude Opus 5 on Azure Databricks](https://azure.microsoft.com/updates?id=568316)
Anthropic Claude Opus 5 모델 지원으로 고도화된 AI 앱·분석(복잡한 추론·코딩/에이전트) 환경이 Databricks에서 가능해졌습니다.

### [Open AI GPT-5.6 on Azure Databricks](https://azure.microsoft.com/updates?id=567431)
Databricks에서 GPT-5.6을 Microsoft Foundry와 연계해 사용할 수 있어, 엔터프라이즈 데이터 기반 AI 서비스 구현이 한층 용이해졌습니다.

### [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)
UK West 리전에서 Databricks SQL Serverless가 출시되어, 즉각적 컴퓨트·자동확장·관리 편의가 강화되어 분석 워크로드 현대화가 촉진됩니다.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)
AI Language에서 문서 기반 PII 검출 Playground가 정식 지원되어, 실시간 예측과 컴플라이언스 업무 효율이 대폭 향상되었습니다.

### [Azure Monitor Logs mirroring into Microsoft Fabric](https://azure.microsoft.com/updates?id=568322)
Monitor Log Analytics 데이터를 실시간으로 Microsoft Fabric에서 분석 가능해져, OneLake 기반의 크로스 도메인·멀티 소스 분석이 실무 혁신을 주도합니다.

---

## ⚙️ 관리 & 거버넌스 / DevOps

운영 자동화, 리질리언스 검증, 데이터 이동·통제, 언어 수명 주기 관리 등 관리와 DevOps 환경이 실질적 효율성·자동화·투명성을 갖추도록 발전합니다.

---

### [Azure Automation supports PowerShell 7.6 runbooks and Runtime environment](https://azure.microsoft.com/updates?id=568102)
PowerShell 7.6 런타임 GA로 보안·성능 개선, 최신 스크립트 자동화, 구버전 런북 손쉽게 업그레이드, Azure CLI 연동이 가능해졌습니다.

### [Support 5x churn in Azure Site Recovery](https://azure.microsoft.com/updates?id=566966)
Site Recovery에서 VM별 최대 500MB/s(5배) 처리량 지원으로, 고성능 데이터베이스·대용량 분석 등 미션 크리티컬 서비스의 복구력이 대폭 향상되었습니다.

### [Public Preview: Azure Storage Mover now supports migration from Google Cloud Storage (GCS)](https://azure.microsoft.com/updates?id=566948)
GCS에서 Azure Blob Storage로의 클라우드 간 데이터 이관 기능이 프리뷰로 제공되어, 멀티 클라우드 환경의 통합·보안·자동화 측면에서 획기적입니다.

### [Export historical data from Log Analytics workspace with Export jobs](https://azure.microsoft.com/updates?id=566591)
Log Analytics 워크스페이스에서 지정된 쿼리/기간 데이터의 스토리지 내보내기 프리뷰가 제공되며, 준법감시·보안분석·장기 보존이 간편해집니다.

### [Support for Python-2.7; 3.8 and PowerShell- 7.1; 7.2 will be retired on September 30, 2026](https://azure.microsoft.com/updates?id=567556)
Automation에서 Python 2.7/3.8, PowerShell 7.1/7.2 지원 종료(9월 30일) 예정. 업그레이드를 반드시 권장하며, 최신 런타임의 지원 정책과 일치합니다.

---

## 🌍 지역 및 데이터센터 (글로벌/특화 리전)

글로벌 클라우드 확장, 신규 리전 개설, 지역 맞춤 서비스 강화 등 Azure의 전 세계 사업 역량 확대와 현지화 전략이 지속됩니다.

---

### [Microsoft Azure now available from new cloud region in India (India South Central)](https://azure.microsoft.com/updates?id=568013)
인도 South Central 리전(하이데라바드) 공식 개설로, AI 기반 클라우드 인프라 및 데이터 레지던시, 빠른 서비스 렌턴시와 회복력 있는 리전 확장이 이뤄졌습니다.

### [Azure Database for PostgreSQL flexible server in India South Central](https://azure.microsoft.com/updates?id=568334)
PostgreSQL Flexible Server가 인도 South Central 리전에서 정식 제공되어, 지역 특화 데이터 기반 서비스와 컴플라이언스 지원이 강화됩니다.

### [Azure Red Hat OpenShift in Chile Central](https://azure.microsoft.com/updates?id=566732)
칠레 Central 리전에서 Red Hat OpenShift 정식 지원. 현지 인프라 기반의 하이브리드/멀티클라우드, 규제산업 대응, 낮은 레이턴시가 장점입니다.

### [Az.PostgreSQLFlexibleServer PowerShell module](https://azure.microsoft.com/updates?id=566209)
PostgreSQL Flexible Server 파워셸 모듈 업데이트 및 REST API와 연계. PostgreSQL 18, 탄력적 클러스터 등 신규 기능 편리하게 관리 가능합니다.

### [Reservation exchanges for Azure services supported by savings plans will no longer be available starting February 1, 2027](https://azure.microsoft.com/updates?id=568514)
2027년 2월 1일부터 Savings Plan 범위 서비스의 예약 교환 정책이 종료되어, 예약 교환 유연성 감소 및 기존 예약의 적합성 검토 필요성이 증대됩니다.

---

## 🧠 Microsoft Foundry & Microsoft Fabric

Foundry와 Fabric은 서비스형 AI, 데이터, 워크플로우 거버넌스를 핵심으로 하며, Toolboxes, 샘플 Playground, 텔레메트리 보호 등 혁신적 기능을 제공합니다.

---

### [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)
Foundry에서 Toolboxes 정식 지원. 표준화된 도구세트 관리, 조직별 재사용·거버넌스 강화, AI/모델 워크플로우 통합이 혁신적으로 구현됩니다.

### [Document PII playground sample in Microsoft Foundry NextGen](https://azure.microsoft.com/updates?id=563331)
PII playground 기능으로 문서 샘플 기반 개인정보 검출·자동화가 더욱 손쉽고 빠르게 실현됩니다.

### [Protect sensitive generative AI telemetry in Application Insights and Microsoft Foundry](https://azure.microsoft.com/updates?id=567594)
Generative AI 텔레메트리를 Foundry/Monitor에서 별도 보호 테이블로 저장·액세스 제어. 규제 산업에서 AI 서비스 사용의 보안성·유연성 확보.

### [AI Gateway in Azure API Management](https://azure.microsoft.com/updates?id=568184)
AI Gateway 프리뷰 지원으로 Foundry, Bedrock, Vertex AI 등 다양한 AI 모델을 API로 안전하게 노출하고, 일관된 보안과 관찰성, 인증·정책 적용이 가능해집니다.

### [Azure Monitor Logs mirroring into Microsoft Fabric](https://azure.microsoft.com/updates?id=568322)
Azure Monitor Log Analytics를 Fabric OneLake로 실시간 연동·분석. 운영 및 비즈니스 데이터 통합 분석이 강화되어, Fabric 기반의 데이터 전략이 현실화됩니다.

---

## 총평 및 다음 달 전망

2026년 7월의 Azure 업데이트는 ‘현대화·보안·AI·자동화·글로벌 확장’의 5대 트렌드가 뚜렷하게 드러난 한 달이었습니다. AKS, Databricks, Foundry, Fabric 등 핵심 클라우드 플랫폼의 기능 확장과 서비스형 제공 방식이 주목받았고, 네트워크/스토리지/보안 등 인프라 현대화와 글로벌 리전 개설이 실무에 큰 영향을 미쳤습니다.

관리 자동화와 수명주기 관리가 강조되며, 최신 언어 런타임 지원과 퇴출 계획이 투명하게 제시되어 조직별 전략 수립이 용이해졌고, 보안·컴플라이언스 강화는 엔터프라이즈/규제산업 대응에 실질적 이점이 제공되었습니다.

AI 기반 워크플로우·분석 환경은 Foundry와 Fabric에서 실무적 혁신을 이끌고, 멀티 클라우드·하이브리드 지원 강화로 다양한 레거시·현대 시스템이 Azure로 쉽게 통합되고 있습니다.

다음 달에는 이 프리뷰 기능들의 정식 지원, 신규 AI·네트워크·컴플라이언스 정책의 발표, 추가 리전 확대, Microsoft Fabric 및 Foundry 기반 데이터/AI 사용성 강화 등이 기대됩니다. 업계 트렌드에 따라 Azure는 지속적으로 최신 기술을 빠르게 도입하면서도 고도화된 자동화·보안·운영 효율성에 초점을 맞출 전망입니다.