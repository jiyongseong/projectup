# Azure 월간 업데이트 요약 - 2026년 07월

## 전반적인 트렌드와 핵심 인사이트

2026년 7월 Azure 업데이트에서는 엔터프라이즈 클라우드 및 AI 워크플로우 혁신, 보안 및 네트워크 강화, 자동화 그리고 멀티 클라우드 및 지역 데이터 센터 확장 등 여러 핵심 영역에서 의미 있는 진전이 있었습니다. AI와 데이터 분석 영역은 Databricks에서 GPT-5.6, Claude Sonnet 5, Claude Opus 5와 같은 최신 대형 모델의 정식 지원 및 Microsoft Foundry와 Fabric의 AI·분석 통합 기능 강화가 두드러집니다. 클라우드 네이티브 애플리케이션 관점에서는 AKS·Fleet Manager의 자원 배치, 업그레이드 자동화, 네트워크 및 스토리지 관련 기능 확장, AKS Gateway API 도입 등 운영 효율화와 현대화가 가속화되었습니다.

보안과 컴플라이언스 영역에서 Confidential Computing(Event Hubs), 네트워크 격리(NSP), 세분화된 키 관리 및 세밀한 접근제어(Entra ID, Azure Key Vault Premium, Firewall, DDoS)가 강화되었습니다. 스토리지 측면에서는 Blob, Files, NetApp Files의 데이터 무결성·암호화·유연한 네트워크 연결 옵션이 보완되었으며, Entra ID 기반의 SFTP 통합 및 Azure Storage Mover의 멀티클라우드 지원도 눈에 띕니다. 자동화 및 관리에서는 PowerShell/파이썬 최신 버전 지원, 복구·업그레이드 성능 개선, Chaos Studio의 시나리오 기반 테스팅, 예약 정책 변경 등 지속적인 플랫폼 운영 최적화가 진행 중입니다.

특히, Microsoft Foundry 및 Fabric 업데이트를 통해 기업은 AI 자산과 비즈니스 데이터의 연계 분석·제어·거버넌스가 OneLake, AI Gateway, Toolboxes 등의 통합서비스를 통해 혁신적으로 이루어지고 있습니다. 지역 확장에서는 인도 남중앙 및 칠레 중앙과 같은 신규 데이터센터 개설로 데이터 레지던시, 레이턴시 개선, 규제 준수를 지원하며, 다양한 글로벌 서비스와 지역별 AI·클라우드 수요에 대응합니다.

이번 달 업데이트는 네트워크·보안의 세분화, 멀티클라우드 통합, 최신 언어·운영체제 지원, AI와 데이터 분석의 엔터프라이즈 적용 확대, 관리 자동화와 효율화가 핵심 트렌드로 파악됩니다. 앞으로 Azure는 AI 시대를 선도하며, 하이브리드·멀티클라우드 환경에 대한 보안, 관리, 성능 혁신을 지속적으로 강화할 것으로 전망됩니다.

---

## ☁️ 클라우드 인프라 및 컨테이너

이번 달에는 AKS 애플리케이션 라우팅 정식 지원, Kubernetes Fleet Manager의 자원 배치·업데이트 내구성 강화, Azure Functions 최신 파이썬 및 PowerShell 지원, Azure Red Hat OpenShift의 신규 리전 개설 등 클라우드 네이티브 플랫폼 및 컨테이너 관리의 현대화가 두드러집니다. Prepared Image Specification 미리 보기 등으로 AI, 고성능 워크로드 대상 빠른 클러스터 시작이 가능해졌고, AKS에서 NFS 암호화 전송 등 보안과 네트워킹 옵션이 개선되었습니다.

### [Application Routing with Gateway API](https://azure.microsoft.com/updates?id=567944)
AKS에서 Kubernetes Gateway API 기반 애플리케이션 라우팅이 정식 지원되어 서비스 메시 없이도 유연한 인그레스 관리가 가능합니다.

### [Azure Functions support for Python 3.14](https://azure.microsoft.com/updates?id=567646)
Azure Functions에서 Python 3.14 지원으로 보안 및 호환성, 장기 지원이 강화되었으며 개발환경이 최신화되었습니다.

### [Resource placement in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567931)
Fleet Manager에서 Kubernetes 리소스의 자동 분산 관리가 가능해져 멀티 클러스터 운영 효율화가 실현되었습니다.

### [Prepared Image Specification (미리 보기)](https://azure.microsoft.com/updates?id=567949)
AKS 노드 이미지를 미리 준비해 빠른 스케일아웃 및 워크로드 시작이 지원됩니다.

### [Maximum allowed failures for update runs in Fleet Manager (미리 보기)](https://azure.microsoft.com/updates?id=567939)
업데이트 실패 임계값 설정 기능으로 대규모 클러스터 업데이트의 내구성과 유연성이 향상되었습니다.

---

## 🛡️ 보안 및 네트워킹

Azure는 네트워크·보안 기능을 대폭 강화하였습니다. Event Hubs Confidential Computing, Network Security Perimeter, NAT64 지원, DDoS 및 Firewall의 커스텀 정책, WAF 예외 처리 등이 주요 내용입니다. Entra ID 기반 SFTP 통합, IPv6 VPN Gateway, Azure Enclave와 같은 고급 격리 환경도 도입되었습니다.

### [Confidential Computing support for Azure Event Hubs Dedicated](https://azure.microsoft.com/updates?id=567212)
Event Hubs 전용 환경에서 Confidential Computing으로 스트리밍 데이터의 실시간 메모리 보호가 가능해져 민감 데이터 보호가 강화되었습니다.

### [Network Security Perimeter 지원 Event Hubs](https://azure.microsoft.com/updates?id=567203)
Event Hubs에서 네트워크 격리 및 중앙 정책 기반 접근제어가 정식 지원되어 데이터 유출 리스크가 한층 감소합니다.

### [IPv6 support for Azure VPN Gateway](https://azure.microsoft.com/updates?id=567847)
Azure VPN Gateway의 IPv6 듀얼 스택 지원으로 차세대 네트워크·워크로드의 유연성이 확대되었습니다.

### [NAT64 on StandardV2 NAT Gateway](https://azure.microsoft.com/updates?id=568409)
NAT64 기능 도입으로 IPv6 워크로드와 IPv4 인터넷 간 통신이 자동화, 복잡한 네트워크 요구에 대응을 강화합니다.

### [Azure Enclave (미리 보기)](https://azure.microsoft.com/updates?id=568377)
안전하고 격리된 클라우드 환경을 빠르게 구축·관리할 수 있는 Azure Enclave가 공개되어 정부 및 규제 산업에서 민감 워크로드 운영이 강화됩니다.

---

## 📦 스토리지 및 데이터 관리

Blob Storage의 데이터 무결성 검증, NFS 암호화 전송, NetApp Files의 Oplocks, Entra ID 기반 SFTP 접속, Storage Mover의 GCS 연동 등 데이터 관리와 보안이 대폭 개선되었습니다. Storage Mover, Blob Storage SDK, Key Vault Premium의 대칭키, Azure Files Premium 영역별 암호화 등 최신 기능이 추가되며 멀티클라우드·네트워크·컴플라이언스까지 지원 범위가 확장되었습니다.

### [Client-side data integrity protections in Azure Blob Storage](https://azure.microsoft.com/updates?id=566895)
Blob Storage SDK를 통한 CRC64-NVME 무결성 검증으로 어플리케이션부터 물리 스토리지까지 전방위 데이터 보호가 실현됩니다.

### [Azure Files NFS Encryption in Transit 정식 지원](https://azure.microsoft.com/updates?id=567787)
AKS 및 Azure Files 연동 시 TLS 기반 암호화 전송이 가능해져 생산 환경 보안이 강화되고 컴플라이언스 준수가 수월해졌습니다.

### [Microsoft Entra ID-based access for Azure Blob Storage SFTP](https://azure.microsoft.com/updates?id=567085)
Entra ID 인증을 활용한 SFTP 접속으로 별도 계정 관리 부담 없이 RBAC·ABAC·ACL 기반 고도화된 접근제어가 가능합니다.

### [Azure Storage Mover now supports migration from Google Cloud Storage (GCS)](https://azure.microsoft.com/updates?id=566948)
GCS에서 Azure Blob Storage로의 클라우드 간 데이터 마이그레이션이 에이전트리스·프라이빗 네트워크 옵션까지 지원됩니다.

### [Symmetric keys on Azure Key Vault Premium (미리 보기)](https://azure.microsoft.com/updates?id=566746)
AES 기반 대칭키 관리 지원으로 중앙화된 키 관리 및 포스트 양자암호 대비 기능이 추가되었습니다.

---

## 🤖 AI · 머신러닝 · 데이터 분석

Databricks와 Foundry를 통한 엔터프라이즈 AI 모델 서비스, PII 문서 샘플 평가·Playground, 신속한 데이터 분석, AI Gateway 등 AI·데이터 분석 플랫폼 혁신이 두드러졌습니다. GPT-5.6, Claude Sonnet 5/Opus 5, Anthropic, OpenAI의 최신 모델이 다양한 어플리케이션과 연동, 고급지능·코딩·비즈니스 데이터를 AI와 결합하는 개발환경이 강화되었습니다.

### [Open AI GPT-5.6 on Azure Databricks](https://azure.microsoft.com/updates?id=567431)
Databricks에서 GPT-5.6 모델, Foundry 연동 통한 실시간 AI 모델·앱 배포·관리·거버넌스가 정식 지원됩니다.

### [Claude Opus 5 on Azure Databricks](https://azure.microsoft.com/updates?id=568316)
Claude Opus 5 지원으로 고차원 AI reasoning, 복잡한 업무·코딩을 위한 엔터프라이즈 지능형 작업이 가능해졌습니다.

### [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)
따로 서버 관리 없이 Databricks SQL Serverless가 영국 서부 리전에서 사용 가능해져 분석 워크로드 효율화가 실현됩니다.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)
PII 검출 Playgroun을 통해 개인식별정보 검출 테스트·적용이 쉬워져 컴플라이언스 팀의 데이터 보호 실무가 단축됩니다.

### [AI Gateway in Azure API Management (미리 보기)](https://azure.microsoft.com/updates?id=568184)
AI Gateway 티어 제공으로 Foundry, AWS, Google, OpenAI 등 다양한 AI 모델을 통합적으로 연결·거버넌스·보안 통제 가능해집니다.

---

## 📝 관리 및 자동화

PowerShell 7.6·Python 3.14 지원, Site Recovery 고성능화, Automation Runtime 환경 업그레이드, Chaos Studio 시나리오 및 CLI 연동 등 관리·운영 자동화가 강화되었습니다. 예약 정책 변경, 런타임 지원 종료, 역사 데이터 Export 등 플랫폼 현대화에 따라 안정성, 보안, 관리 효율화가 지속적으로 진행 중입니다.

### [Azure Automation supports PowerShell 7.6 runbooks and Runtime environment](https://azure.microsoft.com/updates?id=568102)
PowerShell 7.6 런북과 Runtime 환경의 정식 지원으로 관리 스크립트의 최신화와 효율적 운영이 가능합니다.

### [Support 5x churn in Azure Site Recovery](https://azure.microsoft.com/updates?id=566966)
Site Recovery의 데이터 처리량이 크게 향상되어 대용량 산업용 워크로드까지 안정적 복구를 지원합니다.

### [Export historical data from Log Analytics workspace with Export jobs (미리 보기)](https://azure.microsoft.com/updates?id=566591)
Log Analytics 데이터 Export 기능으로 감사, 보안분석, 비즈니스 인텔리전스 등 다양한 외부 활용이 가능해졌습니다.

### [Azure Chaos Studio Workspaces and Scenarios (미리 보기)](https://azure.microsoft.com/updates?id=567184)
Chaos Studio에서 워크스페이스·시나리오 기반 장애 테스트와 보고서 생성을 통한 장애 복원력·컴플라이언스 대응이 강화됩니다.

### [Support for Python-2.7, 3.8 and PowerShell 7.1, 7.2 지원 종료](https://azure.microsoft.com/updates?id=567556)
9월 30일자로 자동화에서 해당 런타임 지원이 종료되어, 보안 및 기능 업데이트를 위해 빠른 업그레이드가 요구됩니다.

---

## 🔗 Microsoft Foundry & Fabric

Foundry Toolboxes 등 AI Prompt Agent 통합·거버넌스, PII 샘플 Playground, Application Insights AI 텔레메트리 보호, Fabric에서 Azure Monitor 로그 내보내기 등 엔터프라이즈 AI·데이터 거버넌스 혁신이 두드러집니다. AI Gateway API 통합, OneLake에서 실시간 분석, 센서 데이터와 비즈니스 데이터 연계 등 Fabric-Foundry 중심의 차별화된 데이터 활용이 가능해졌습니다.

### [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)
이제 Foundry에서 AI Prompt Agent용 공통 Tool을 조직 단위로 통합·거버넌스해 중복 코딩 없이 연동과 관리가 가능합니다.

### [Protect sensitive generative AI telemetry in Application Insights and Microsoft Foundry (미리 보기)](https://azure.microsoft.com/updates?id=567594)
Foundry 및 Application Insights의 AI 텔레메트리 접근제어 강화로 PII/PHI 등 민감 데이터 보호가 한층 보완됩니다.

### [Azure Monitor Logs mirroring into Microsoft Fabric (미리 보기)](https://azure.microsoft.com/updates?id=568322)
Fabric OneLake에서 Azure Monitor 로그를 파케이 형식으로 실시간 연동, 크로스 비즈니스·운영 데이터 통합 분석이 가능해졌습니다.

### [Public Preview: Document PII playground sample in Microsoft Foundry NextGen](https://azure.microsoft.com/updates?id=563331)
Foundry NextGen 환경에서 PII 문서 샘플 Playground가 제공되어 AI 기반 개인정보 보호·컴플라이언스 테스트가 더욱 쉽고 신속해졌습니다.

### [AI Gateway in Azure API Management (미리 보기)](https://azure.microsoft.com/updates?id=568184)
Foundry, OpenAI 등 다양한 AI 모델을 API Gateway로 통합, 강력한 정책·보안·관찰성을 바탕으로 자산 관리를 혁신합니다.

---

## 🌎 지역 및 글로벌 확장

Azure는 인도 남중앙과 칠레 중앙 리전을 신규 개설하여 기업 고객의 지역 데이터 레지던시, AI 인프라 지원, 규제 준수를 보장합니다. PostgreSQL Flexible Server, Red Hat OpenShift, Databricks 등 핵심 서비스들이 신규 리전에서 일괄적으로 출시되어 현지 클라우드 수요와 디지털 트랜스포메이션을 적극 지원합니다.

### [Microsoft Azure now available from new cloud region in India (India South Central)](https://azure.microsoft.com/updates?id=568013)
인도 남중앙 리전 개설로 지역 데이터 레지던시, AI 인프라, 낮은 레이턴시가 보장됩니다.

### [Azure Database for PostgreSQL flexible server in India South Central](https://azure.microsoft.com/updates?id=568334)
PostgreSQL Flexible Server가 남중앙 인도 리전에서 정식 지원되어 데이터베이스·AI 워크로드의 현지화가 강화됩니다.

### [Azure Red Hat OpenShift in Chile Central](https://azure.microsoft.com/updates?id=566732)
칠레 중앙 Azure 리전에서 OpenShift 클러스터가 정식 지원되어 현지 엔터프라이즈/규제 산업의 클라우드 도입이 활성화됩니다.

### [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)
영국 서부 리전에서 서버리스 Databricks SQL로 분석 워크로드의 지역화와 효율적 운영이 실현됩니다.

### [Document PII Playground 등 글로벌 컴플라이언스 및 규제 대응](https://azure.microsoft.com/updates?id=564382)
PII Playground, Red Hat OpenShift, Data Residency 정책 등 다양한 서비스가 리전별 규제와 컴플라이언스 요구에 맞추어 출시되었습니다.

---

## 총평 및 다음 달 전망

2026년 7월, Azure는 AI와 데이터 분석, 멀티 클라우드 관리, 네트워크·보안 강화, 자동화 업그레이드, 글로벌 리전 확대를 중심으로 한층 진화된 엔터프라이즈 클라우드 플랫폼을 선보였습니다. 특히 Foundry·Fabric 중심의 AI/데이터 거버넌스, 최신 소프트웨어 스택의 신속한 지원, 대규모 분산환경 운영 효율화는 시장 리더십을 확고히 하는 모습입니다. 향후에는 더욱 세밀한 보안·감사 제어 기능, AI 모델 관리 자동화, 하이브리드·멀티클라우드 환경을 위한 통합 운영 툴, 그리고 글로벌 리전 확장에 따라 지역별 맞춤형 클라우드 기능이 추가될 것으로 예상됩니다. Azure는 AI 시대의 신뢰, 성능, 정책 중심 클라우드 혁신을 지속적으로 주도할 것으로 기대됩니다.