# Azure 월간 업데이트 요약 - 2026년 07월

---

## 트렌드 및 핵심 인사이트

2026년 7월 Azure 업데이트에는 클라우드 운영의 현대화, AI/ML 기능 강화, 보안 및 네트워크 혁신, DevOps 및 애플리케이션 관리 효율화가 두드러졌습니다. AKS 및 Kubernetes 기반 서비스에 대한 신규 기능이 대거 정식 지원되면서 컨테이너 기반 워크로드의 관리 효율성이 크게 향상되었습니다. Azure Databricks는 Anthropic Claude Sonnet 5, Claude Opus 5, 그리고 OpenAI GPT-5.6 등 첨단 AI 모델을 추가로 지원하며, AI Gateway, 인프라 운영 자동화, 데이터 분석과 서비스 확장 등 Microsoft Foundry와 Microsoft Fabric을 중심으로 AI, 데이터 연계, 보안 컴플라이언스를 촉진합니다.

또한 네트워크 및 보안 분야에서는 NAT64 및 IPv6 지원 확대, Azure Firewall의 HTTP 헤더 삽입, VPN Gateway의 IPv6 지원, Azure DDoS Protection의 커스텀 정책 등 혁신적인 기능이 출시되었습니다. 신규 리전(인도 South Central) 출범과 함께 지역별 다각화도 이루어졌고, Azure Storage Mover 등 멀티클라우드 환경에서의 데이터 이동 및 관리 자동화가 강조됐습니다.

운영 및 개발 측면에서는 PowerShell 7.6, Python 3.14 등 최신 런타임 지원이 확대되고, 기존 버전 지원 종료, Kubernetes Fleet Manager의 리소스 분산 및 장애 허용 업데이트 등 지속적인 운영 효율성 제고에 초점을 맞추고 있습니다. DevOps 및 관리 도구에서는 Azure Monitor와 Chaos Studio에서 신규 기능들이 미리 보기로 공개되며, 로그 데이터 연동, 시나리오 기반 장애 테스트, 인사이트 보호 강화 등이 적용되었습니다.

총평하자면, 이번 달은 Azure의 전반적인 현대화와 자동화, AI 활용 확장, 멀티클라우드 유연성, 보안 수준 향상, 그리고 관리 효율화가 핵심 키워드였습니다. 조직은 최신 기능을 적극적으로 도입하면서 운영 안정성과 보안을 강화할 필요가 있습니다.

---

## 🖥️ 컴퓨트 및 컨테이너

전반적인 요약  
컴퓨트와 컨테이너 영역에서는 Azure Kubernetes Service(AKS)의 Gateway API 신규 정식 지원 및 리소스 분산, Azure Functions의 Python 3.14 지원, PowerShell 7.6 미리 보기, VM 복구성과 AKS 운영 효율성 개선 등 플랫폼의 최신화와 운영 자동화가 두드러집니다. 컨테이너와 서버리스 워크로드 관리의 표준화와 보안성이 강화되면서, 업무 효율과 운영 안정성이 크게 향상되고 있습니다.

### [Application Routing with Gateway API](https://azure.microsoft.com/updates?id=567944)  
AKS에서 Gateway API 기반 어플리케이션 라우팅이 정식 지원되어, 인그레스 표준화 및 기존 nginx 인그레스와의 점진적 전환이 가능합니다.

### [Azure Functions support for Python 3.14](https://azure.microsoft.com/updates?id=567646)  
Azure Functions가 Python 3.14를 지원함으로써 개발자들은 보안, 지원 기간, 최신 런타임 기능을 활용할 수 있습니다.

### [Resource placement in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567931)  
여러 AKS 및 Arc 클러스터에 Kubernetes 리소스를 일관성 있게 배치하는 기능이 정식 지원되어, 대규모 환경의 운영 자동화가 가능해집니다.

### [Public Preview: Azure Functions Support for PowerShell 7.6](https://azure.microsoft.com/updates?id=567651)  
PowerShell 7.6을 Azure Functions 계획에 미리 보기로 지원함으로써, 스크립트 호환성과 최신 운영환경으로의 전환을 쉽게 할 수 있습니다.

### [Prepared Image Specification](https://azure.microsoft.com/updates?id=567949)  
AKS 노드 이미지 사양을 사전 준비된 이미지 형태로 미리 지정해, 워크로드의 초기화 속도와 확장성을 대폭 향상할 수 있습니다.

---

## 📊 AI, 데이터 및 애널리틱스

전반적인 요약  
AI 및 데이터 분석 카테고리에서는 Claude Sonnet 5, Claude Opus 5, GPT-5.6 등 최첨단 AI 모델을 Azure Databricks에서 지원하게 되면서, 엔터프라이즈 AI 적용 범위가 크게 확대되었습니다. 이벤트 허브의 기밀 컴퓨팅, 데이터 통합 및 분석 워크로드의 서버리스 지원, PII 탐지 기능 강화 등 데이터 보호와 분석 유연성이 함께 발전합니다.

### [Open AI GPT-5.6 on Azure Databricks](https://azure.microsoft.com/updates?id=567431)  
GPT-5.6 모델이 Azure Databricks에서 지원되어, 엔터프라이즈 데이터 기반의 AI 애플리케이션 구축 및 배포가 가능합니다.

### [Claude Opus 5 on Azure Databricks](https://azure.microsoft.com/updates?id=568316)  
Anthropic의 신형 Claude Opus 5 모델이 Databricks에 추가되어, 고도 추론 및 복잡한 AI 작업 지원이 확대됩니다.

### [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)  
Serverless SQL 웨어하우스가 UK West 리전에 정식 지원되며, 분석 워크로드의 인프라 관리 효율성과 비용 최적화가 촉진됩니다.

### [Confidential Computing support for Azure Event Hubs Dedicated](https://azure.microsoft.com/updates?id=567212)  
기밀 컴퓨팅이 Event Hubs Dedicated에 적용되어, 메모리 내 데이터까지 보안이 강화됩니다.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)  
문서 PII 탐지 기능이 Playground 형태로 정식 지원되어, 데이터 보호 및 컴플라이언스 업무가 간소화됩니다.

---

## 🛡️ 보안, 네트워크 및 컴플라이언스

전반적인 요약  
네트워크와 보안 부문에서는 IPv6 지원 확대, NAT64 및 Azure Firewall의 헤더 삽입, VPN Gateway의 IPv6, DDoS Protection 맞춤 정책 등 네트워크 유연성과 보안 기능이 대폭 강화되었습니다. 이벤트 허브 및 블롭 스토리지의 클라이언트-서버 간 데이터 무결성 보장, Azure Enclave로 격리된 환경 제공 등 엔터프라이즈 보안 요구사항을 반영한 기능들이 주목받고 있습니다.

### [IPv6 support for Azure VPN Gateway](https://azure.microsoft.com/updates?id=567847)  
Azure VPN Gateway에서 IPv6 트래픽이 지원되어, 듀얼스택 네트워크 운영과 현대적 워크로드 연계가 가능해졌습니다.

### [NAT64 on StandardV2 NAT Gateway](https://azure.microsoft.com/updates?id=568409)  
NAT64가 정식 지원되어 IPv6 워크로드가 IPv4 전용 인터넷 대상으로 NAT 변환을 통해 연결할 수 있습니다.

### [HTTP header insertion in Azure Firewall](https://azure.microsoft.com/updates?id=568115)  
Azure Firewall에서 HTTP/HTTPS 헤더 삽입 기능이 정식 지원되어, 테넌트 제한, SaaS 접근 제어 등 다양한 시큐리티 시나리오를 구현 가능합니다.

### [Azure DDoS Protection custom policy](https://azure.microsoft.com/updates?id=568063)  
DDoS Protection 맞춤 정책이 미리 보기로 공개되어, 고객별 트래픽 패턴에 맞춰 독자적인 임계값 준비가 가능합니다.

### [Azure Enclave](https://azure.microsoft.com/updates?id=568377)  
Azure Enclave가 미리 보기로 공개되어 정부 및 규제 산업의 민감 워크로드에 격리된 클라우드 환경 배포가 가능해집니다.

---

## 🗄️ 스토리지 및 데이터 관리

전반적인 요약  
스토리지 카테고리에서는 Azure Blob Storage SFTP에서 Entra ID 기반 접근, 클라이언트-서버 데이터 무결성 강화, Storage Mover의 Google Cloud Storage 지원, Azure Files NFS의 전송 암호화 등 데이터 보호와 멀티클라우드 연동이 확장되었습니다. Azure NetApp Files와 Key Vault Premium의 기능 미리 보기도 출시되어 데이터 관리의 안정성과 보안성이 높아졌습니다.

### [Client-side data integrity protections in Azure Blob Storage](https://azure.microsoft.com/updates?id=566895)  
Azure Blob Storage에서 CRC64-NVME를 활용한 클라이언트 측 데이터 무결성 검증 기능이 정식 지원되어, 엔드-투-엔드 데이터 보호가 강화됩니다.

### [Microsoft Entra ID-based access for Azure Blob Storage SFTP](https://azure.microsoft.com/updates?id=567085)  
Entra ID를 통한 SFTP 접근이 정식 지원되면서, 운영 복잡성 감소 및 보안성 강화가 실현됩니다.

### [Encryption in Transit for Azure Files NFS Shares in Azure Kubernetes Service (AKS)](https://azure.microsoft.com/updates?id=567787)  
AKS 볼륨의 Azure Files NFS 전송 구간 암호화가 정식 지원되어, 데이터 이동시 보안과 컴플라이언스를 충족합니다.

### [Public Preview: Azure Storage Mover now supports migration from Google Cloud Storage (GCS)](https://azure.microsoft.com/updates?id=566948)  
Storage Mover가 Google Cloud Storage와 Azure Blob Storage 간 데이터를 모델 기반으로 전환할 수 있는 기능을 미리 보기로 지원합니다.

### [Support for SMB Opportunistic Locking (Oplocks) configuration](https://azure.microsoft.com/updates?id=568396)  
Azure NetApp Files에서 SMB Oplocks 설정이 미리 보기로 지원되어 파일 접근동기화와 캐싱 효율이 개선됩니다.

---

## 🛠️ 관리, 거버넌스 및 DevOps

전반적인 요약  
관리 및 거버넌스 카테고리에서는 Azure Automation의 최신 런타임 지원 확대, Site Recovery의 복구 성능 향상, Chaos Studio의 Workspace 시나리오, Log Analytics의 데이터 연동과 내보내기 등 운영 효율화와 복원력 향상, DevOps 자동화가 강조됩니다. Python/PowerShell 등 기존 버전 지원 종료(September 2026) 일정 발표와 함께 최신화 권장이 이루어집니다.

### [Azure Automation supports PowerShell 7.6 runbooks and Runtime environment](https://azure.microsoft.com/updates?id=568102)  
PowerShell 7.6 런북 정식 지원으로 최신 스크립트 환경, 보안, 이동성을 확보할 수 있습니다.

### [Support 5x churn in Azure Site Recovery](https://azure.microsoft.com/updates?id=566966)  
Site Recovery에서 VM당 최대 500MB/s의 복구가 가능해져, 대용량 IOPS 환경의 디지털 복구 탄력성이 강화됩니다.

### [Azure Chaos Studio Workspaces and Scenarios](https://azure.microsoft.com/updates?id=567184)  
Chaos Studio가 Workspaces와 시나리오 기능을 미리 보기로 제공해, 실제 장애 테스트와 컴플라이언스 보고에 활용됩니다.

### [Export historical data from Log Analytics workspace with Export jobs](https://azure.microsoft.com/updates?id=566591)  
Log Analytics Export Job이 미리 보기로 공개되어, 데이터 내보내기 및 분석, 컴플라이언스, BI 활용 범위가 확장됩니다.

### [Retirement: Support for Python-2.7; 3.8 and PowerShell- 7.1; 7.2 will be retired on September 30, 2026](https://azure.microsoft.com/updates?id=567556)  
2026년 9월 30일 이후 위 런타임 지원 종료가 예고되며, 최신 버전으로 전환이 필수화됩니다.

---

## 🏭 Microsoft Foundry 및 Microsoft Fabric

전반적인 요약  
Foundry와 Fabric 영역에서는 AI/PII 데이터 탐지, Toolboxes 제공, 로그 데이터 연동, 생성형 AI 텔레메트리 보호 등 데이터와 모델을 효율적이고 보안적으로 연결하는 명확한 현대화 흐름이 있습니다. Fabric에서는 Azure 모니터 로그를 원본 형식(Delta Parquet)으로 연동하여, 크로스 도메인 분석 및 ML 활용이 확장됩니다.

### [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)  
Foundry Toolboxes가 정식 지원되어, 정책 기반 AI 툴 통합 및 재사용성, 개발 편의성이 극대화됩니다.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)  
PII 탐지 Playground가 정식 지원되어, 온보딩과 컴플라이언스 시나리오 가속화가 가능합니다.

### [Public Preview: Document PII playground sample in Microsoft Foundry NextGen](https://azure.microsoft.com/updates?id=563331)  
Foundry NextGen에서 샘플 Playground가 미리 보기로 제공되어, PII 탐지 정확성 평가가 신속히 이루어집니다.

### [Azure Monitor Logs mirroring into Microsoft Fabric](https://azure.microsoft.com/updates?id=568322)  
Azure Monitor 로그를 Fabric OneLake에 실시간 미러링하는 기능이 미리 보기로 출시되어, 분석 및 ML 연계가 강화됩니다.

### [Protect sensitive generative AI telemetry in Application Insights and Microsoft Foundry](https://azure.microsoft.com/updates?id=567594)  
Application Insights의 생성형 AI 텔레메트리를 테이블 단위로 보호할 수 있는 기능이 미리 보기로 공개되어, 민감 정보 보안성 향상이 가능해졌습니다.

---

## 🌏 지역 및 리전 확장 소식

전반적인 요약  
지역 확대 소식에서 인도 South Central 신규 리전 출범, Azure Database for PostgreSQL Flexible Server의 해당 지역 지원, Azure Red Hat OpenShift의 칠레 Central 지원 등 글로벌 인프라의 저지연, 데이터 레지던시, 지역 규제 대응이 강화되었습니다.

### [Microsoft Azure now available from new cloud region in India (India South Central)](https://azure.microsoft.com/updates?id=568013)  
인도 Hyderabad에 신규 리전이 출범하며, AI 및 클라우드 인프라의 현지화와 레지던시 보장이 이루어집니다.

### [Azure Database for PostgreSQL flexible server in India South Central](https://azure.microsoft.com/updates?id=568334)  
PostgreSQL flexible server가 인도 South Central 리전에서 정식 지원되어, 현지 데이터베이스 운영이 가능합니다.

### [Azure Red Hat OpenShift in Chile Central](https://azure.microsoft.com/updates?id=566732)  
칠레 Central 리전에서 OpenShift가 지원되어, 남미 지역에서 OpenShift 기반 클라우드 네이티브 운영이 가능합니다.

### [Generally available: Anthropic Claude Sonnet 5 on Azure Databricks](https://azure.microsoft.com/updates?id=567194)  
UK West 등 신규 리전에서 첨단 AI 모델 지원이 이루어집니다.

### [Azure Sphere OS version 26.09 is now available for evaluation](https://azure.microsoft.com/updates?id=568466)  
Azure Sphere OS의 대형 버전 및 장기적 지원이 준비되어, IoT 운영 안정성이 확보됩니다.

---

## 총평 및 다음 달 전망

2026년 7월 Azure 업데이트는 대대적인 서비스 현대화와 AI/데이터 활용의 혁신, 운영 안정성과 컴플라이언스 보강이 돋보였습니다. AKS, Functions, Databricks, Foundry, Fabric 등 핵심 플랫폼의 기능 확장과 보안 제공이 이루어졌으며, 지역별 인프라 집중 투자로 글로벌 고객의 요구에 더욱 능동적으로 대응하고 있습니다. 네트워크 및 스토리지 보안성 향상, 클라우드 거버넌스, 멀티클라우드 통합의 가속은 앞으로도 Azure 중심 전략의 핵심이 될 것입니다.

다음 달에는 Fabric 기반 데이터 분석, 현대화된 DevOps 자동화, AI 운영 통합, 신규 보안 및 네트워크 기능 확장, 지역별 신규 리전과 서비스 출시가 예고됩니다. 최신 기능 도입 시 운영팀은 기존 환경과의 호환성, 보안 정책 강화, 장애 복원력 점검에 특별히 주의해야 하며, 내년까지 서비스 마이그레이션 및 최신화 계획을 선제적으로 검토할 필요가 있습니다. Azure의 글로벌 역량과 AI 플랫폼 국면은 조직의 디지털 혁신을 효과적으로 뒷받침할 것입니다.