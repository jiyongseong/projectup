# Azure 월간 업데이트 요약 - 2026년 07월

## 전반적인 트렌드와 핵심 인사이트

2026년 7월 Azure 업데이트는 인프라와 서비스의 전방위적 최적화와 플랫폼 신뢰성 강화, 그리고 AI·데이터 분석 역량의 비약적인 확장이라는 세 가지 핵심 트렌드로 요약됩니다. Kubernetes 및 컨테이너 기반 서비스가 지속적으로 발전하면서 최신 표준을 적용한 게이트웨이 API, 이미지 프리페어드 사양, 리소스 플릿 관리 등 운영 효율성과 확장성을 높이는 기능들이 정식 지원 혹은 미리 보기로 도입되었습니다. Azure Databricks와 AI Model Serving(Claude Opus/Claude Sonnet/GPT-5.6 등), Microsoft Foundry 도구 통합, Application Insights의 AI 텔레메트리 보호 등 AI·머신러닝 플랫폼은 엔터프라이즈 워크로드에 맞춘 보안, 컴플라이언스, 운영 거버넌스를 대폭 강화하는 방향으로 진화 중입니다.

네트워크 및 보안 측면에서는 NAT64, IPv6, DDoS 맞춤 정책, 새로운 Perimeter 기능, Azure Enclave, Confidential Computing 등 클라우드 네트워크의 민첩성과 업무·데이터 보호 장치가 동시에 고도화되었습니다. Storage 부분에서도 Blob Storage의 클라이언트 무결성, Entra 기반 SFTP 인증, Azure Files EiT 등 데이터 신뢰성, 관리 효율성, 통합 정책이 강화됐습니다. 인프라 지역 측면에서는 인도·칠레 등 신규 리전을 통한 글로벌 확장, PostgreSQL·OpenShift·Databricks 등 서비스의 지역별 지원 확대가 두드러집니다.

마지막으로 Microsoft Foundry·Fabric·Automation 등 조직 내 DevOps 및 데이터·AI 거버넌스의 중요성이 강조되고 있으며, 런타임 지원 종료 정책, 예약 교환 제한 등 플랫폼의 장기적 안정성과 관리 정책 변화도 확인할 수 있습니다.

---
## 🛠️ AI + 머신러닝 및 데이터 분석

AI 플랫폼과 데이터 분석 서비스는 이번 달 혁신적인 모델 통합, AI 거버넌스 도구 강화, 엔터프라이즈 워크로드 최적화에 초점을 맞췄습니다.

### [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)
UK West 리전에서 Databricks SQL Serverless가 정식 지원되어 즉각적인 분석, 자동 스케일링, 인프라 관리 최소화가 가능합니다. 다양한 워크로드에 Serverless, Classic, Pro 옵션을 제공해 유연성을 확대합니다.

### [Claude Opus 5 on Azure Databricks](https://azure.microsoft.com/updates?id=568316)
Anthropic Claude Opus 5 모델이 Databricks AI Model Serving에 통합되어 복잡한 추론, 소프트웨어 개발, 장기 계획 등에 사용 가능하며, 엔터프라이즈 데이터와 연계된 AI 에이전트 구축이 한층 수월해졌습니다.

### [Open AI GPT-5.6 on Azure Databricks](https://azure.microsoft.com/updates?id=567431)
GPT-5.6 모델이 Foundry 및 Databricks 통합 환경에서 정식 지원되어 데이터 거버넌스와 유니티 AI Gateway 연동을 통한 AI 애플리케이션 구축이 가능합니다.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)
문서 기반 PII 탐지 샘플 Playground가 정식 지원되어 규제/컴플라이언스 담당자와 개발팀이 빠르게 개인 정보 탐지·적용 결과를 평가할 수 있습니다.

### [Anthropic Claude Sonnet 5 on Azure Databricks](https://azure.microsoft.com/updates?id=567194)
Claude Sonnet 5 모델이 Databricks에 정식 지원되며, 대규모 AI 에이전트, 코드 자동화 등 엔터프라이즈 워크로드에서 효율성과 품질을 실현할 수 있습니다.

이번 달 AI&Ml 항목은 최신 모델의 빠른 도입과 안전한 운영, 다양한 워크로드 지원과 플랫폼 통합의 강화를 통해 Azure의 기업 AI 역량 확대를 이끌었습니다.

---

## ☁️ 클라우드 인프라·운영·컴퓨트

컴퓨트와 Kubernetes 기반의 서비스, 운영 관리의 혁신이 두드러집니다. 리소스 배치, 이미지 준비, 최신 런타임 등으로 운영 신뢰성과 확장성을 높이고 있습니다.

### [Application Routing with Gateway API](https://azure.microsoft.com/updates?id=567944)
AKS에서 Gateway API 기반의 어플리케이션 라우팅이 정식 지원되어 서비스 메시 없이 최신 Ingress 관리를 구현할 수 있습니다.

### [Azure Functions support for Python 3.14](https://azure.microsoft.com/updates?id=567646)
Linux 환경의 Azure Functions에서 Python 3.14 개발 및 배포가 가능해 보안성과 장기 지원, 개발 도구 호환성이 향상됩니다.

### [Resource placement in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567931)
Fleet Manager에서 리소스 배치 기능이 정식 지원되어 클러스터 간 일관된 Kubernetes 리소스 분배와 정책 관리를 자동화합니다.

### [Azure Automation supports PowerShell 7.6](https://azure.microsoft.com/updates?id=568102)
Automation에서 PowerShell 7.6 런북, 최신 런타임 환경이 정식 지원되어 스크립트 관리 효율성과 보안, Azure CLI 통합성이 강화됩니다.

### [Prepared Image Specification in AKS (Preview)](https://azure.microsoft.com/updates?id=567949)
AKS 노드 이미지 사양 미리 보기가 제공되어 사전 이미지 구성으로 노드 시작 속도와 운영 효율성을 대폭 개선할 수 있습니다.

운영 효율성과 개발 환경의 최신화는 Azure 플랫폼의 신뢰성 및 확장성 강화를 위한 지속적인 혁신이라는 트렌드로 정리됩니다.

---

## 🗃️ 스토리지·네트워크·보안

저장소, 네트워크, 보안 기능은 데이터 무결성, 접근 통제, 서비스 연결 등 실질적인 안정성과 관리 효율성을 강화하는 방향으로 도입되었습니다.

### [Client-side data integrity protections in Azure Blob Storage](https://azure.microsoft.com/updates?id=566895)
.NET/C++/JavaScript SDK에서 클라이언트 측 CRC64-NVME 검증 지원으로 애플리케이션~물리적 저장소 간 완전성 검증이 가능합니다.

### [Microsoft Entra ID-based access for Azure Blob Storage SFTP](https://azure.microsoft.com/updates?id=567085)
Entra ID 기반 인증이 SFTP에 도입되어 운영 관리, MFA, 조건부 접근 정책 등 클라우드 수준의 보안 통합을 실현합니다.

### [Encryption in Transit for Azure Files NFS Shares in AKS](https://azure.microsoft.com/updates?id=567787)
AKS에서 Azure Files NFS v4.1 데이터 이동 트래픽에 TLS 기반 암호화를 적용해 보안과 컴플라이언스 요구를 충족합니다.

### [IPv6 support for Azure VPN Gateway](https://azure.microsoft.com/updates?id=567847)
VPN Gateway에서 IPv6 듀얼 스택 트래픽 전송이 지원되어 IPv4/IPv6 워크로드 통합 및 확장성이 한층 높아졌습니다.

### [NAT64 on StandardV2 NAT Gateway](https://azure.microsoft.com/updates?id=568409)
IPv6 워크로드가 IPv4-only 인터넷 대상으로 NAT64를 통해 통신할 수 있게 되어 네트워크 이기종 환경 확장성이 개선되었습니다.

네트워크와 저장소의 보안, 유연성, 데이터 신뢰성이 실질적 워크로드 운영 안정성을 크게 높이고 있습니다.

---

## 🔒 보안·컴플라이언스·관리

Azure 보안, 컴플라이언스, 관리 도구는 네트워크 경계, DDoS 맞춤 정책, 엔클레이브, 머신러닝 기반 보호 등 보안 신뢰성을 한층 강화했습니다.

### [Confidential Computing support for Azure Event Hubs Dedicated](https://azure.microsoft.com/updates?id=567212)
하드웨어 기반 신뢰 실행 환경(TEE)을 활용한 스트리밍 데이터 인-메모리 보호로 컴플라이언스 강화에 기여합니다.

### [HTTP header insertion in Azure Firewall](https://azure.microsoft.com/updates?id=568115)
Azure Firewall에서 요청 헤더 삽입 기능을 통해 Tenant Restriction, SaaS 접근 제어 등 보안 정책 구현이 가능해졌습니다.

### [Azure DDoS Protection custom policy (Preview)](https://azure.microsoft.com/updates?id=568063)
DDoS 방어 임계값을 리소스별로 세밀하게 맞춤 설정할 수 있는 기능이 도입되었습니다.

### [Azure Enclave (Preview)](https://azure.microsoft.com/updates?id=568377)
Azure Enclave가 민감 워크로드용 격리 환경 제공, 네트워크 분리 및 접근 제어 강화로 규제 산업별 특별 보안 수요를 만족시킵니다.

### [Symmetric keys on Azure Key Vault Premium (Preview)](https://azure.microsoft.com/updates?id=566746)
고급 대칭키 및 AES 기반 암호화/복호화 기능이 Key Vault Premium에서 미리 보기로 제공, CNSA 2.0 맞춤 및 포스트-퀀텀 대비 마련.

보안·컴플라이언스 기능은 실제 현장에서 필요한 맞춤화, 자동화, 통합의 방향으로 지속 발전 중입니다.

---

## 🚀 Microsoft Foundry

Microsoft Foundry 관련 기능은 도구 통합, 신속한 평가, AI 관측 데이터 보호가 눈에 띄게 강화되고 있습니다.

### [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)
Foundry에서 툴박스가 정식 지원되어 다양한 업무 도구를 일관되게 호출·거버넌스 적용이 가능해져 조직 전체 생산성이 높아졌습니다.

### [Document PII playground sample in Microsoft Foundry NextGen (Preview)](https://azure.microsoft.com/updates?id=563331)
PII 탐지 샘플 평가 기능이 NextGen 포털에 제공되어 API 연동 전 빠르고 직관적으로 기능 테스트가 가능합니다.

### [Protect sensitive generative AI telemetry in Application Insights and Microsoft Foundry (Preview)](https://azure.microsoft.com/updates?id=567594)
Application Insights에서 AI 텔레메트리 보호기능이 도입되어, 민감한 AI 생성 데이터 접근을 테이블별로 제어할 수 있게 되었습니다.

### [AI Gateway in Azure API Management (Preview)](https://azure.microsoft.com/updates?id=568184)
Foundry, AWS, GCP 등 주요 AI 자산의 게이트웨이 연동이 미리 보기로 제공되어 API 통합 거버넌스와 보안 정책을 적용할 수 있습니다.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)
Foundry와 연동된 문서 기반 PII 탐색 Playground가 정식 지원되어 개인정보 검출 및 컴플라이언스 평가가 대폭 간소화되었습니다.

Foundry는 조직의 AI 에이전트 개발, 거버넌스, 데이터 보호 과정을 표준화·자동화하는 Azure 혁신의 핵심 플랫폼으로 성장하고 있습니다.

---

## 💾 Microsoft Fabric

이번 달 Microsoft Fabric 관련 미리 보기 업데이트는 Azure와 Fabric 간 데이터 이동·집계의 통합, AI/BI 분석 연계 등이 강조됩니다.

### [Azure Monitor Logs mirroring into Microsoft Fabric (Preview)](https://azure.microsoft.com/updates?id=568322)
Log Analytics 로그를 Microsoft Fabric OneLake에 실시간 연동하여 조직의 운영·비즈니스 데이터 통합 분석이 가능해집니다.

### [Export historical data from Log Analytics workspace with Export jobs (Preview)](https://azure.microsoft.com/updates?id=566591)
Log Analytics Workspace에서 특정 쿼리를 기반으로 필요한 데이터만 수출, 장기 보관, 외부 분석을 지원합니다.

### [Protect sensitive generative AI telemetry in Application Insights and Microsoft Foundry (Preview)](https://azure.microsoft.com/updates?id=567594)
Fabric과 연계된 AI 텔레메트리 데이터 보호 기능으로 민감 정보의 안전한 관리와 접근 권한 제어가 강화됩니다.

### [Azure DDoS Protection custom policy (Preview)](https://azure.microsoft.com/updates?id=568063)
Fabric 연계 인프라에 맞춘 DDoS 방어 임계값 설정 기능이 미리 보기로 도입되어 클라우드 전체에 보안 정책을 통합할 수 있습니다.

### [AI Gateway in Azure API Management (Preview)](https://azure.microsoft.com/updates?id=568184)
Fabric 내 AI 자산 연동 API 게이트웨이 기능이 도입되어 AI 모델·툴의 엔터프라이즈 사용·관리 효율화가 이루어지고 있습니다.

이번 달 Fabric 관련 기능은 클라우드-데이터-운영 가시성의 확장과 데이터 기반 의사결정 프로세스 혁신을 선도하고 있습니다.

---

## 🌐 글로벌 리전 확장 및 지역별 업데이트

인프라 지역과 서비스 리전 확장이 글로벌 Azure 이용 환경의 다양성을 더욱 높이고 있습니다.

### [Azure Database for PostgreSQL flexible server in India South Central](https://azure.microsoft.com/updates?id=568334)
인도 South Central 신규 리전에서 PostgreSQL 서버 정식 지원으로 지역 인프라 확장과 데이터 주권 요구를 충족합니다.

### [Azure Red Hat OpenShift in Chile Central](https://azure.microsoft.com/updates?id=566732)
칠레 최초의 Azure 리전에서 OpenShift 정식 지원, 현지 규제 및 데이터 주권 요구를 만족하며 하이브리드 클라우드 확장에 기여합니다.

### [Microsoft Azure now available from new cloud region in India (India South Central)](https://azure.microsoft.com/updates?id=568013)
인도 내 네 번째 데이터센터(하이데라바드, Telangana) 개설로 지역 성장, AI 준비, 클라우드 인프라 수요 대응력이 제고됐습니다.

### [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)
UK West 지역에서 SQL Serverless 정식 지원, 분석 워크로드의 속도·자동화·유연성이 지역별로 확대됩니다.

### [Azure Sphere OS version 26.09 is now available for evaluation](https://azure.microsoft.com/updates?id=568466)
Azure Sphere OS 26.09 버전이 평가용으로 제공되며, 장기 지원 및 보안 커널 발전에 있어 고객 평가를 적극 독려합니다.

글로벌 리전 확장은 데이터 주권, 성능 최적화, 규제 준수를 충족하며 다양한 산업군의 Azure 도입을 한층 촉진하고 있습니다.

---

## 🗂️ 관리 및 거버넌스, 서비스 정책

플랫폼 관리, 거버넌스, 서비스 정책 업데이트는 장기 운영 안정성과 규제 준수를 확보하기 위한 다양한 변화와 개선으로 나타납니다.

### [Microsoft Defender security assessments for Azure Database for PostgreSQL Flexible Server](https://azure.microsoft.com/updates?id=567527)
Defender CSPM 평가가 PostgreSQL Flexible Server에 도입되어 취약점 분석, 개선 추천, 컴플라이언스 대응을 자동화합니다.

### [New Powershell module: Az.PostgreSQLFlexibleServer](https://azure.microsoft.com/updates?id=566209)
PostgreSQLFlexibleServer PowerShell 모듈이 정식 지원되어 PostgreSQL 18 지원, 탄력적 클러스터 관리, REST API 연동 등 관리 효율성을 크게 높입니다.

### [Support 5x churn in Azure Site Recovery](https://azure.microsoft.com/updates?id=566966)
Site Recovery에서 VM당 500MB/s까지 지원되어 고속 IOPS 워크로드 복구 역량이 극적으로 향상됐습니다.

### [Retirement: Support for Python-2.7; 3.8 and PowerShell- 7.1; 7.2 종료 예정](https://azure.microsoft.com/updates?id=567556)
10월1일부터 해당 런타임 버전의 지원 종료가 예정되어 운영자들은 필히 최신 버전으로 업그레이드 해야 합니다.

### [Announcing: Reservation exchanges for Azure services supported by savings plans will no longer be available starting February 1, 2027](https://azure.microsoft.com/updates?id=568514)
2027년 2월부터 저장 공간, 컴퓨트, 데이터베이스 등 주요 서비스의 예약 교환이 savings plan 적용 시 제한됩니다.

이는 장기적으로 Azure 서비스의 운영 신뢰성, 관리 효율, 규제 준수를 강화하는 방향으로 변화를 유도하고 있습니다.

---

## 총평 및 다음 달 전망

2026년 7월 Azure 업데이트는 AI&데이터 분석, 클라우드 인프라 자동화, 네트워크·스토리지의 신뢰성 강화, 글로벌 리전 확장 등 전방위 혁신의 흐름을 보여줬습니다. 최신 Kubernetes, Databricks, Foundry, Fabric 등 클라우드 내외부 워크로드 운영 효율성과 보안, 컴플라이언스 요구가 동시에 높아진 점이 특징입니다. 런타임 지원 종료 및 예약 교환 정책 변화는 장기적 플랫폼 안정성에 대한 Microsoft의 의지가 반영된 것으로 분석됩니다.

다음 달에는 AI 모델 및 인프라 서비스의 지속적인 업데이트와 함께, 리전별 세부 기능 고도화, Fabric·Foundry·Automation 연계 강화, 보다 구체적인 거버넌스 정책 적용이 예상됩니다. 클라우드 내 데이터·AI 자산 통합 관리와 보안 자동화, 글로벌 확장 속도가 더욱 가속될 전망입니다.