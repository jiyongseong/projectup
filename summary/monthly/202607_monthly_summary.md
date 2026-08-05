# Azure 월간 업데이트 요약 - 2026년 07월

## 전반적인 트렌드 및 핵심 인사이트

2026년 7월, Azure의 업데이트는 클라우드 네이티브 인프라의 고도화, 멀티 클라우드 지원 강화, AI 서비스 통합, 보안 및 거버넌스의 현대화, 지역별 서비스 확대 등 전 영역에서 혁신이 계속되고 있음을 보여줍니다. 가장 두드러진 트렌드는 Kubernetes와 AKS 등 컨테이너 관리 기술의 표준 채택과 자동화를 통한 효율성 증대, OpenAI 및 Anthropic Claude 등 첨단 AI 모델의 Databricks 및 Foundry 등 플랫폼 연계, 엔터프라이즈 보안 요구에 대응하기 위한 Confidential Computing, Network Security Perimeter, Entra 기반 인증 등입니다.

지역별로 인도 South Central·칠레 등 신규 리전이 열린 것은 글로벌 공급망 안정성과 데이터 주권 요구에 적극 대응하는 것으로 해석됩니다. 스토리지 서비스의 데이터 무결점 강화, 클라우드 간 저장소 이동 간편화, Azure Site Recovery의 고성능 강화 등 데이터 관리 신뢰도도 높아졌습니다. AI 통합에서는 Foundry Toolboxes와 Databricks AI 모델 서빙, Fabric 연계 모니터링의 실시간 분석, Foundry 내 PII 샘플 Playground 등 실사용 중심 혁신이 돋보입니다.

실행 환경에서는 Python 3.14, PowerShell 7.6 등 최신 언어 지원 확대와 기존 버전 지원 종료의 안내가 병행되고, 네트워킹 영역에서는 NAT64, IPv6, DDoS 맞춤 정책 등 차세대 인프라 지원이 확대되었습니다. 또 저장소·보안·네트워크·모니터링 각 분야에서 SDK와 관리툴 통합이 빨라져, DevOps와 관리 거버넌스 확장성도 크게 향상되었습니다.

전반적으로 Azure는 멀티 클라우드, 글로벌, AI 및 고도 보안 요구에 선제적으로 대응하며, 기업들의 지속적인 디지털 전환을 보다 쉽고 빠르게 지원할 수 있는 플랫폼으로 성장하고 있습니다. 이번 달에는 특히 데이터 보안·컴플라이언스, 최신 AI 활용, Kubernetes 및 자동화, 클라우드 마이그레이션의 실제 효율성이 크게 개선된 점이 눈에 띄었습니다.

---

## 1️⃣ 컴퓨팅 & 컨테이너

이번 달 컴퓨팅·컨테이너 부문은 Kubernetes 기반 혁신, Azure Functions 언어 지원 확대, Fleet Manager의 효율적 리소스 배치, AKS 데이터 암호화, 이미지 사양 표준화 등이 강조되었습니다. Python·PowerShell 최신 버전 지원으로 모던 워크로드 실행 환경 개선, AKS Gateway API 등 인그레스 표준화를 통한 운영 효율성 개선도 주목할 만합니다.

### [Application Routing with Gateway API](https://azure.microsoft.com/updates?id=567944)
AKS에서 Gateway API 기반 애플리케이션 라우팅이 정식 지원되어, 기존 인그레스 환경에서 최신 표준으로 점진적 전환을 지원합니다.

### [Azure Functions support for Python 3.14](https://azure.microsoft.com/updates?id=567646)
Azure Functions가 Python 3.14에 정식 지원을 제공, 최신 보안·지원 창구 확대와 개발자 생산성 향상.

### [Azure Functions support for PowerShell 7.6 (미리 보기)](https://azure.microsoft.com/updates?id=567651)
PowerShell 7.6 미리 보기 기반 Azure Functions 개발 가능해졌으며, 향후 자동화 확장성 개선 전망.

### [Resource placement in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567931)
Fleet Manager의 리소스 배치가 정식 지원되어, 여러 AKS·Arc 클러스터에 대한 일관적 배포와 거버넌스 용이.

### [Prepared Image Specification (미리 보기)](https://azure.microsoft.com/updates?id=567949)
AKS 노드 이미지 사전 준비로 노드 초기화 시간 단축 및 확장성·운영 효율성 강화.

---

## 2️⃣ 저장소 & 데이터 관리

이번 달에는 Blob/NFS 저장소 암호화, SFTP 인증 모델 개선, 클라우드 간 데이터 이관 도구 확대, NetApp Files SMB 락 구성 등 데이터 신뢰성과 안전성이 향상되었습니다. SDK 통합과 클라우드 간 마이그레이션 지원, Azure Files의 NFS 데이터 암호화 전송 정식 지원 등 엔터프라이즈급 데이터 운용도 강화되었습니다.

### [Client-side data integrity protections in Azure Blob Storage](https://azure.microsoft.com/updates?id=566895)
Blob Storage에서 CRC64-NVME 체크섬 지원으로 클라이언트단 데이터 무결성 검증 가능, 엔드투엔드 신뢰성 확보.

### [Microsoft Entra ID-based access for Azure Blob Storage SFTP](https://azure.microsoft.com/updates?id=567085)
Entra ID 기반 SFTP 접근이 정식 지원, 인증·온보딩·협업 단순화 및 보안 강화.

### [Encryption in Transit for Azure Files NFS Shares in AKS](https://azure.microsoft.com/updates?id=567787)
AKS에서 Azure Files NFS 볼륨의 TLS 암호화 데이터 전송 정식 지원, 컴플라이언스 대응 및 보안 강화.

### [Azure Storage Mover에서 Google Cloud Storage 이동 지원 (미리 보기)](https://azure.microsoft.com/updates?id=566948)
Google Cloud Storage에서 Blob Storage로의 클라우드 간 이동이 미리 보기로 지원되어, 멀티 클라우드 통합이 용이해짐.

### [SMB Opportunistic Locking 구성 지원 (미리 보기)](https://azure.microsoft.com/updates?id=568396)
NetApp Files에서 SMB/듀얼 프로토콜 볼륨의 Oplock 설정 가능, 클라이언트 캐싱 효율 개선.

---

## 3️⃣ 네트워킹 & 보안

네트워크는 NAT64로 IPv6~IPv4 접속 지원 확대, VPN Gateway에서 IPv6 정식 지원, Azure Firewall의 HTTP 헤더 삽입, DDoS 맞춤 정책, Front Door Edge Actions 등 컨트롤·확장성·보안 혁신이 이어졌습니다. Key Vault 프리미엄의 대칭키 미리 보기 등 보안 컴플라이언스 요구와 실제 서비스 연결성 개선이 두드러집니다.

### [NAT64 on StandardV2 NAT Gateway](https://azure.microsoft.com/updates?id=568409)
NAT64로 IPv6 워크로드가 IPv4 전용 인터넷으로 자연스럽게 통신 가능, DNS64 연계 통한 자동 트래픽 변환.

### [HTTP header insertion in Azure Firewall](https://azure.microsoft.com/updates?id=568115)
Azure Firewall에서 HTTP/HTTPS 헤더 삽입 지원, 엔터프라이즈 보안 및 접근 제어 시나리오 확대.

### [IPv6 support for Azure VPN Gateway](https://azure.microsoft.com/updates?id=567847)
VPN Gateway에서 IPv6 트래픽 정식 지원, 듀얼 스택 환경의 네트워크 운영 확대.

### [Azure DDoS Protection custom policy (미리 보기)](https://azure.microsoft.com/updates?id=568063)
DDoS Protection에서 커스텀 정책 미리 보기 지원, 워크로드별 임계치 설정 가능.

### [Symmetric keys on Azure Key Vault Premium (미리 보기)](https://azure.microsoft.com/updates?id=566746)
Key Vault Premium에서 대칭키(AES) 미리 보기 지원, CNSA-2.0 및 미래 암호화 대응에 유리.

---

## 4️⃣ AI & 머신러닝 · 데이터 분석

AI+분석 영역은 Databricks에서 Claude Opus 5, Sonnet 5, OpenAI GPT-5.6 등 최신 모델의 정식 지원, Event Hubs의 Confidential Computing과 NSP, PII Playground 등 실무용 기능 확대에 주목할 만합니다. Foundry와 Databricks의 모델 서빙·통합, Azure AI Language의 실시간 문서 PII 평가 등 AI 활용의 실효적 확대가 핵심입니다.

### [Claude Opus 5 on Azure Databricks](https://azure.microsoft.com/updates?id=568316)
Databricks에서 Anthropic Claude Opus 5 정식 지원, 고난도 AI업무·코딩·에이전트 워크플로우 활용 가능.

### [Generally available: Anthropic Claude Sonnet 5 on Azure Databricks](https://azure.microsoft.com/updates?id=567194)
Sonnet 5가 Databricks에서 정식 지원, 중대 분석·에이전트 워크플로우에서 최신 AI 사용 가능.

### [Open AI GPT-5.6 on Azure Databricks](https://azure.microsoft.com/updates?id=567431)
GPT-5.6의 Foundry 구매 모델을 Databricks에서 서빙할 수 있어, 실무용 AI 개발/운영 통합 지원.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)
Azure AI 서비스의 문서 PII 검출 Playground 정식 지원, 샘플 기반 실시간 검출·평가 가능.

### [Network Security Perimeter support for Azure Event Hubs](https://azure.microsoft.com/updates?id=567203)
Event Hubs에서 NSP 지원, 네트워크 격리 및 보안 정책 일관화 가능.

---

## 5️⃣ 관리·운영·컴플라이언스 & 마이그레이션

관리 및 마이그레이션 영역에서는 Automation의 최신 언어 지원과 기존 버전 지원 종료, Site Recovery 고속 작업, Storage Mover 도구, Azure Chaos Studio의 시나리오 관리 및 CLI 통합, 예약 교환 정책 변경 등 실제 운영의 자동화·효율성·컴플라이언스 대응이 강화되었습니다.

### [Azure Automation supports PowerShell 7.6 runbooks and Runtime environment](https://azure.microsoft.com/updates?id=568102)
PowerShell 7.6 런북·실행환경 정식 지원, 자동화 스크립트 현대화와 운영 효율성 증대.

### [Support 5x churn in Azure Site Recovery](https://azure.microsoft.com/updates?id=566966)
Site Recovery가 5배의 IOPS 지원, 중대 워크로드에서도 신속 복구 가능.

### [Log Analytics Export jobs (미리 보기)](https://azure.microsoft.com/updates?id=566591)
Log Analytics의 데이터를 쿼리 기반 외부 저장소로 내보내는 기능 미리 보기 지원, 컴플라이언스·분석·이관 편의 제공.

### [Manage Azure Chaos Studio from the Azure CLI (미리 보기)](https://azure.microsoft.com/updates?id=567225)
Chaos Studio 시나리오를 CLI에서 간편히 관리·실행, 자동화·통합 관리 효율 강화.

### [Support for Python-2.7; 3.8 and PowerShell- 7.1; 7.2 will be retired](https://azure.microsoft.com/updates?id=567556)
Automation 환경에서 Python 2.7, 3.8, PowerShell 7.1, 7.2 지원 종료 안내—보안·운영 측면 최신 버전으로 업그레이드 필수.

---

## 6️⃣ Microsoft Foundry

Foundry는 Toolboxes의 정식 지원, PII Playground 샘플 미리 보기, AI Gateway 연계 모델 서빙 등 조직 내 AI 자산 관리·유통·프로덕션 배포 여건을 크게 개선했습니다. 통합된 툴 관리, 사용자별 접근 제어, 안전한 데이터 보호 등 엔터프라이즈 AI 혁신 중심입니다.

### [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)
Toolboxes 정식 지원으로 모든 조직에 AI 툴 사용·관리 효율성 대폭 향상.

### [Document PII playground sample in Microsoft Foundry NextGen (미리 보기)](https://azure.microsoft.com/updates?id=563331)
Foundry NextGen의 PII Playground 미리 보기 제공, 샘플 기반 신속 평가 및 API 연동 가능.

### [AI Gateway in Azure API Management (미리 보기)](https://azure.microsoft.com/updates?id=568184)
AI Gateway 미리 보기, Foundry 및 다양한 AI 모델 관리·서빙과 보안정책 통합.

### [Protect sensitive generative AI telemetry in Application Insights and Microsoft Foundry (미리 보기)](https://azure.microsoft.com/updates?id=567594)
Foundry와 Application Insights에서 생성형 AI 데이터 보호 강화.

### [Azure Monitor Logs mirroring into Microsoft Fabric (미리 보기)](https://azure.microsoft.com/updates?id=568322)
Azure Monitor 로그를 Fabric에 실시간 복사 지원, 경영·운영 데이터 및 AI 통합 분석 가능.

---

## 7️⃣ Azure 지역·데이터센터

지역 확장에서는 인도 South Central과 칠레 Central 리전 오픈, PostgreSQL Flexible Server 신규 리전 배포, 네트워크 및 컴플라이언스의 지역별 확장 등 글로벌 클라우드 가용성과 데이터 주권을 강화하는 전략이 실현되고 있습니다.

### [Microsoft Azure now available from new cloud region in India (India South Central)](https://azure.microsoft.com/updates?id=568013)
인도 South Central 지역 신규 오픈, AI·클라우드 인프라 수요 대응 및 데이터 주권 보장.

### [Azure Database for PostgreSQL flexible server in India South Central](https://azure.microsoft.com/updates?id=568334)
PostgreSQL flexible server 신규 리전 배포로 데이터베이스 서비스 확장.

### [Azure Red Hat OpenShift in Chile Central](https://azure.microsoft.com/updates?id=566732)
칠레 최초 Azure 리전 오픈과 함께 OpenShift 정식 지원, 규제 산업 및 대기업의 클라우드 전환 가속화.

### [Standard service endpoint (미리 보기)](https://azure.microsoft.com/updates?id=561475)
IaaS~PaaS 통합 엔드포인트, 지역별 Private Link 네트워크 격리·확장 대응.

### [New Powershell module: Az.PostgreSQLFlexibleServer](https://azure.microsoft.com/updates?id=566209)
PostgreSQL 관리 PowerShell 모듈 개편, 신기능·신규 리전 대응 효율성 강화.

---

## 총평 및 다음 달 전망

2026년 7월의 Azure 업데이트는 글로벌 커버리지의 확장과 실제 엔터프라이즈 요구에서 비롯된 AI·데이터·보안·운영 혁신이 유기적으로 결합된 한 달이었습니다. 특히 AKS 표준화, Foundry와 Databricks 등 AI 플랫폼의 통합, 데이터 저장소의 신뢰성 혁신, 멀티 클라우드 지원 도구 강화, 자동화 및 언어 지원 현대화, 네트워크·보안 컨트롤의 디테일한 혁신 등이 두드러졌으며, 컴플라이언스 및 지역별 데이터 주권 강화까지 구체적으로 현실화된 점이 인상적입니다.

다음 달에는 AI 및 데이터 통합관리, 자동화와 운영 정책의 세분화, 네트워크 현대화와 멀티 리전 지원, 기존 버전 지원 종료에 따른 실제 업그레이드 가이드·도구 강화, Fabric과 Foundry 중심의 Analytics·Governance 혁신이 지속될 것으로 전망됩니다. Enterprise 고객은 Azure 최신 기능을 적극적으로 도입하여 운영 효율성과 보안, 데이터 신뢰성을 동시에 극대화하는 여건이 마련될 것입니다.