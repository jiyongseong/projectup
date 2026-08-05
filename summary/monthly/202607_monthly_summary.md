# Azure 월간 업데이트 요약 - 2026년 07월

## 🧭 트렌드 및 핵심 인사이트

2026년 7월의 Azure 업데이트는 클라우드 현대화와 AI 활용을 더욱 빠르게 가속하는 방향으로 집중되었습니다. 확장성과 효율성, 보안 및 거버넌스 강화, 멀티클라우드 지원, 개인 정보 보호 등 실무에 직결되는 요구사항에 대한 대응이 두드러집니다.

먼저, Kubernetes와 컨테이너 관리 영역에서는 Gateway API 기반 애플리케이션 라우팅, Fleet Manager의 리소스 자동 배치 및 실패 허용 업데이트 정책 도입 등 복잡한 환경에서의 관리 효율성을 높이고 있습니다. AKS와 OpenShift의 지역별 확대와 준비된 이미지 규격 기능 도입을 통해 대규모 워크로드의 민첩한 확장과 하이브리드/멀티클라우드 연동이 더욱 쉬워졌습니다.

AI 및 머신러닝 분야에서는 Anthropic Claude Sonnet 5, Opus 5, OpenAI GPT-5.6 등 첨단 AI 모델의 지원과 Microsoft Foundry, Databricks 통합 등 개발자와 데이터 사이언티스트 모두가 생산성을 높일 수 있는 기반이 강화되고 있습니다. AI Gateway 미리보기로 다양한 AI 자산의 안전한 API 공유와 관리 체계도 구축되고 있습니다.

스토리지와 네트워킹 영역에서는 Client-side 데이터 무결성, Entra ID기반 SFTP, NFS 암호화, NAT64, IPv6 지원 등 데이터 보안 및 네트워크 유연성의 극적인 개선이 이뤄졌고, 기존 인프라의 현대화와 지능형 운영이 가능해졌습니다. Key Vault Premium의 대칭키 지원, 이벤트 허브의 NSP, Confidential Computing 등은 규제 대응 및 데이터 격리 필요가 큰 조직에 최적화되고 있습니다.

DevOps 및 거버넌스 관점에서는 Azure Automation, Site Recovery, Chaos Studio의 시나리오 기반 테스트 자동화와 CLI 연동, Monitor 로그 데이터의 Microsoft Fabric 연동 등 실질적인 운영 효율과 업무 자동화에 중점이 맞춰졌습니다.

지역 확장 및 멀티클라우드 지원에서는 인도 South Central, 칠레 Central 등 신규 리전 출시와 PostgreSQL, Databricks 등 주요 서비스의 지역별 정식 지원이 이루어져 글로벌, 로컬 비즈니스 모두에 대응력이 향상되었습니다.

전반적으로 이번 달 Azure는 "최신화, 자동화, 보안, 글로벌 확장"을 키워드로, 대규모 복잡한 워크로드의 민첩하고 안전한 이동과 운영을 실현하는 방향으로 발전하고 있음을 확인할 수 있습니다. Microsoft Foundry, Fabric, Databricks 등 전략 플랫폼의 기능이 본격적으로 확대되고, AI와 보안이 운영 전반에서 기본 요소로 자리 잡았음이 뚜렷합니다.

---

## 🚀 출시 및 정식 지원 (Launched)

이번 달 출시/정식 지원된 주요 기능은 AKS Gateway API 기반 라우팅, Azure Automation PowerShell 7.6 지원, PostgreSQL Flexible Server 인도 South Central 리전 확대 등 클라우드 운영의 자동화와 지역 확장을 모두 아우르고 있습니다. 리소스 관리 효율성과 데이터 무결성 강화, 보안 기능 고도화가 핵심 이슈로 나타났습니다.

### [Application Routing with Gateway API](https://azure.microsoft.com/updates?id=567944)
AKS에서 Gateway API 기반 인그레스 관리를 정식 지원하여, 기존 nginx 방식에서 표준화된 라우팅으로 점진적 전환이 가능해졌습니다.

### [Azure Automation supports PowerShell 7.6 runbooks and Runtime environment](https://azure.microsoft.com/updates?id=568102)
PowerShell 7.6 런북과 런타임 환경의 정식 지원으로, 유지보수 및 업무 자동화의 보안성과 효율성이 크게 향상되었습니다.

### [Azure Database for PostgreSQL flexible server in India South Central](https://azure.microsoft.com/updates?id=568334)
Azure PostgreSQL Flexible Server의 인도 South Central 리전 정식 지원으로, 지역 데이터 레지던시와 성능 요구에 대응합니다.

### [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)
Databricks SQL Serverless의 UK West 리전 지원으로, 분석 워크로드의 자동 확장성과 단순한 인프라 관리가 가능해졌습니다.

### [Azure Functions support for Python 3.14](https://azure.microsoft.com/updates?id=567646)
Python 3.14 기반 Azure Functions의 정식 지원으로 장기 지원 및 최신 보안 패치 반영이 가능합니다.

---

## 🧪 미리보기 및 신규 기능 (In preview)

프리뷰에서는 AI Gateway, Chaos Studio Workspaces, DDoS Protection 커스텀 정책, Enclave, Front Door Edge actions 등 최신 신기술을 빠르게 실험할 수 있는 기반이 강화되고 있습니다. 네트워크, 스토리지, DevOps 등 다양한 영역에서 대규모 환경에 맞는 맞춤형 설정과 자동화 정책이 가능해졌습니다.

### [AI Gateway in Azure API Management](https://azure.microsoft.com/updates?id=568184)
AI Gateway가 미리보기로 공개되어, 다양한 AI 모델(API, 툴, 서버 등)을 안전하게 폭넓게 관리할 수 있게 되었습니다.

### [Azure Chaos Studio Workspaces and Scenarios](https://azure.microsoft.com/updates?id=567184)
Chaos Studio에서 워크스페이스와 시나리오 기반 자동화 테스트를 지원, 실제 장애 상황에 대한 신속한 검증 및 보고 기능이 제공됩니다.

### [Azure DDoS Protection custom policy](https://azure.microsoft.com/updates?id=568063)
DDoS 보호 커스텀 정책으로, 트래픽 유형별 임계값 조절 및 예측 가능한 이벤트 대응이 가능해졌습니다.

### [Azure Enclave](https://azure.microsoft.com/updates?id=568377)
민감한 워크로드 및 정부/규제 산업 대상 격리된 클라우드 환경을 쉽고 신속하게 배치 및 관리할 수 있는 Enclave가 프리뷰로 도입되었습니다.

### [Azure Front Door edge actions](https://azure.microsoft.com/updates?id=567402)
Front Door에서 엣지 액션(서버리스)이 지원돼 실시간 요청 처리 유연성과 성능, 보안이 극대화됩니다.

---

## 🌐 네트워크 및 보안

이번 달 네트워크와 보안 강화는 퍼블릭/프라이빗 네트워크의 식별 및 격리, NAT64, IPv6 지원 확대, Confidential Computing과 NSP, Key Vault 대칭키 등 데이터 방어와 연결의 유연성을 모두 잡았습니다.

### [HTTP header insertion in Azure Firewall](https://azure.microsoft.com/updates?id=568115)
Azure Firewall에서 HTTP/HTTPS 헤더 삽입 지원으로, 보안 및 SaaS 접속관리가 유연해졌습니다.

### [IPv6 support for Azure VPN Gateway](https://azure.microsoft.com/updates?id=567847)
VPN Gateway에서 IPv6 및 듀얼스택 지원, 온프레미스와 Azure 간 브랜치 연결의 확장성을 높입니다.

### [NAT64 on StandardV2 NAT Gateway](https://azure.microsoft.com/updates?id=568409)
NAT64 지원으로 IPv6 워크로드와 IPv4-only 인터넷 목적지에 대한 연결 번역을 실현했습니다.

### [Confidential Computing support for Azure Event Hubs Dedicated](https://azure.microsoft.com/updates?id=567212)
Confidential Computing으로 메모리 내 이벤트 스트림 데이터의 보안성이 획기적으로 강화됩니다.

### [Network Security Perimeter support for Azure Event Hubs](https://azure.microsoft.com/updates?id=567203)
NSP 지원으로, PaaS 자원에 대한 네트워크 격리 경계와 공공 접근 제어가 효과적으로 구현됩니다.

---

## 📦 스토리지 및 데이터 관리

스토리지 및 데이터 관리 섹션에서는 클라이언트 무결성 보호, Entra ID SFTP 접근 등 인프라 보안성과 운영 편의성을 확대하는 동시에, Google Cloud Storage의 미리보기 마이그레이션 기능, Azure Files의 NFS 암호화와 NetApp Files의 SMB Oplocks 등이 전면적으로 강화되고 있습니다.

### [Client-side data integrity protections in Azure Blob Storage](https://azure.microsoft.com/updates?id=566895)
Blob Storage SDK의 클라이언트 무결성 검증 강화로, 엔드-투-엔드 안전한 데이터 처리가 실현됩니다.

### [Microsoft Entra ID-based access for Azure Blob Storage SFTP](https://azure.microsoft.com/updates?id=567085)
Entra ID 기반 SFTP 접근 권한으로 운영 편의와 보안이 대폭 개선되었습니다.

### [Encryption in Transit for Azure Files NFS Shares in Azure Kubernetes Service (AKS)](https://azure.microsoft.com/updates?id=567787)
AKS에서 Azure Files NFS 암호화 지원으로, 트랜잭션 보안과 규제 요구에 대응합니다.

### [Public Preview: Azure Storage Mover now supports migration from Google Cloud Storage (GCS)](https://azure.microsoft.com/updates?id=566948)
구글 클라우드 스토리지에서 Blob Storage로의 보안 마이그레이션이 무중단/대규모로 가능해졌습니다.

### [Support for SMB Opportunistic Locking (Oplocks) configuration](https://azure.microsoft.com/updates?id=568396)
Azure NetApp Files의 SMB Oplocks 설정 지원으로 클라이언트 캐싱 및 데이터 동기화 정책 맞춤이 용이합니다.

---

## 💻 컴퓨팅, 컨테이너, 운영 자동화

컴퓨팅과 컨테이너 관리에서 AKS Gateway API, Fleet Manager 리소스 자동 배치, 파워셸/파이썬 최신 버전 지원 등 관리 효율성과 자동화가 두드러집니다. VM Restore Point의 인스턴트 액세스, Prepared Image Specification 등 실제 대규모 서비스 운영에 핵심적인 기능들이 다수 공개되었습니다.

### [Resource placement in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567931)
Fleet Manager에서 Kubernetes 리소스의 자동 배포와 일관성 있는 운용이 정식 지원됩니다.

### [Public Preview: Azure Functions Support for PowerShell 7.6](https://azure.microsoft.com/updates?id=567651)
Azure Functions에서 PowerShell 7.6 지원 미리보기로, 자동화 스크립트의 최신화와 보안이 강화되었습니다.

### [Instant Access via application consistent restore points](https://azure.microsoft.com/updates?id=565758)
VM Restore Point의 즉시 디스크 복구 기능으로 데이터 복구 속도와 안정성이 크게 향상되었습니다.

### [Prepared Image Specification](https://azure.microsoft.com/updates?id=567949)
AKS 노드 이미지 사전 준비 기능으로 대규모 워크로드의 빠르고 예측 가능한 확장이 가능한 환경이 마련되었습니다.

### [Maximum allowed failures for update runs in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567939)
업데이트 허용 실패 한도 설정으로 실패 상황에서도 지속적인 업데이트와 운영 신뢰성이 보장됩니다.

---

## 📊 Analytics, AI & ML, Microsoft Foundry, Fabric

AI와 분석 영역에서는 Databricks SQL Serverless, Claude Sonnet/Opus 5, GPT-5.6 등 첨단 모델의 정식 지원, Microsoft Foundry Toolboxes, Document PII Playground 등 AI 개발 환경의 혁신이 지속되고 있습니다. 또한 Microsoft Fabric과 Azure Monitor 연동으로 운영 및 비즈니스 데이터 분석의 통합이 가속화되고 있습니다.

### [Claude Opus 5 on Azure Databricks](https://azure.microsoft.com/updates?id=568316)
Anthropic Claude Opus 5를 Databricks AI Model Serving에서 정식 지원합니다.

### [Generally available: Anthropic Claude Sonnet 5 on Azure Databricks](https://azure.microsoft.com/updates?id=567194)
AI 에이전트 및 코딩, 장기 워크플로우에 최적화된 Claude Sonnet 5를 사용할 수 있습니다.

### [Open AI GPT-5.6 on Azure Databricks](https://azure.microsoft.com/updates?id=567431)
GPT-5.6(Microsoft Foundry 구매) 모델을 Databricks에서 사용할 수 있게 되어, 고급 AI 통합이 본격화되었습니다.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)
PII 문서 탐색 Playground가 Microsoft Foundry GA로 공개되어, 개인정보 탐지·적용 테스트가 실무에 바로 활용 가능해졌습니다.

### [Azure Monitor Logs mirroring into Microsoft Fabric](https://azure.microsoft.com/updates?id=568322)
Azure Monitor 로그를 Microsoft Fabric으로 실시간 미러링 지원, 업무 데이터와 운영 데이터의 통합 분석이 가능해졌습니다.

---

## 🔒 관리, 거버넌스, 마이그레이션, 사용 종료 (Retirement & Compliance)

운영 자동화, 관리, 구독 정책, 지원 종료가 주요 영역입니다. Azure Automation의 Python/PowerShell 구버전 지원 종료, Site Recovery 고부하 지지, PostgreSQLFlexibleServer PowerShell 모듈 등 실무 운영에 필수적인 관리 고도화와 업데이트 정책 변화가 두드러집니다.

### [Microsoft Defender security assessments for Azure Database for PostgreSQL Flexible Server](https://azure.microsoft.com/updates?id=567527)
Defender CSPM 보안 평가가 PostgreSQL Flexible Server에 정식 지원, 실시간 취약점 분석 및 권장 조치가 가능해졌습니다.

### [Support 5x churn in Azure Site Recovery](https://azure.microsoft.com/updates?id=566966)
Site Recovery가 5배 수준의 고변동성 워크로드 지원으로 데이터베이스 및 빅데이터 재해 복구가 한층 강화되었습니다.

### [New Powershell module:  Az.PostgreSQLFlexibleServer](https://azure.microsoft.com/updates?id=566209)
Az.PostgreSQLFlexibleServer PowerShell 모듈 출시로, 최신 기능과 효율적 운영관리가 가능해졌습니다.

### [Retirement: Support for Python-2.7; 3.8 and PowerShell- 7.1; 7.2 will be retired on September 30, 2026](https://azure.microsoft.com/updates?id=567556)
2026년 9월 30일 이후 Python 2.7/3.8과 PowerShell 7.1/7.2 지원 종료, 업무 자동화 환경의 최신화가 필수적입니다.

### [Announcing: Reservation exchanges for Azure services supported by savings plans will no longer be available starting February 1, 2027](https://azure.microsoft.com/updates?id=568514)
2027년 2월부터 Savings Plan 적용 서비스의 예약 교환 중단, 효율적 비용 관리 정책의 변화가 예고됩니다.

---

## 🔭 총평 및 다음 달 전망

2026년 7월 Azure의 업데이트는 "현대 클라우드 운영의 표준화와 자동화"가 핵심입니다. AKS 등 컨테이너 관리의 효율성, AI/데이터 분석의 실용화, 스토리지·네트워크의 보안성 강화, 글로벌 리전 확대가 동시다발적으로 이루어졌습니다. Microsoft Foundry와 Fabric의 접목, Databricks AI 모델 생태계 확장 등 전략 플랫폼의 영향력이 커지고 있으며, 실무 운영자와 개발자 모두가 최신 기능 적용을 통한 경쟁력 확보가 필요한 시기임을 보여줍니다.

다음 달에는 AI Gateway, Azure Enclave 등 프리뷰 기능의 정식화 기대가 높고, AKS, Databricks, 지역 리전 추가와 같은 글로벌 확장 기조가 지속될 전망입니다. 또한, Python/PowerShell 지원 종료 등 운영 환경의 최신화 요구가 꾸준히 강조될 것이며, 자동화, 보안, 모니터링 등 클라우드 인프라의 기반 기술 혁신이 계속 이어질 것으로 예상됩니다. 

Azure의 지속적인 혁신은 이용자의 요구를 체계적으로 반영하며, 클라우드 운영의 미래 표준을 선도할 것으로 평가됩니다.