# Azure 월간 업데이트 요약 - 2026년 07월

## 주요 트렌드 및 핵심 인사이트

2026년 7월 Azure 업데이트에서는 인공지능과 데이터 분석, 보안, 네트워크 확장, 관리 효율화, 멀티 클라우드 및 지역별 서비스 확장에 대한 강화된 움직임이 뚜렷하게 나타났습니다.  
특히 AI 및 데이터 분석 부문에서는 Azure Databricks가 빠르게 최신 AI 모델(Claude Sonnet 5, Claude Opus 5, GPT-5.6 등)을 지원하며 엔터프라이즈 혁신을 가속화하는 모습이 두드러졌습니다. Microsoft Foundry 및 Fabric 관련 기능(PII Playground, Toolbox, 로그 미러링 등)은 데이터 관리와 AI 거버넌스를 통합하는 신뢰 기반을 제공하며, 다양한 환경에서의 적용성과 확장성을 모두 충족하고 있습니다.

컴퓨트 및 컨테이너 부문에서는 AKS 기반의 최신 게이트웨이 API 적용, Python 3.14 지원, PowerShell 7.6 지원 등 최신 언어 및 인프라 기능이 정식 지원되어 개발자의 생산성과 운영 안정성이 대폭 상승했습니다.  
네트워크와 보안 영역에서는 Azure Firewall의 HTTP 헤더 삽입, VPN Gateway의 IPv6 지원, NAT64, DDoS Protection 맞춤 정책, Azure Enclave 등 다양한 보안 기능과 네트워크 경계 관리 역량이 강화되었고, Storage도 Blob에 클라이언트 무결성 보호, SFTP를 위한 Entra ID 접근과 애플리케이션간 암호화 등 확장성과 신뢰성을 높였습니다.

관리 및 거버넌스에서는 Chaos Studio의 시나리오 중심 테스트, Site Recovery 고효율 변화 지원, Monitor 및 로그 연동, 오토메이션 운영환경 업데이트 및 사용 중단 공지 등 플랫폼 안정성과 고도화에 중점이 실렸 습니다.  
새로운 지역(Azure India South Central, Chile Central) 개설은 글로벌 클라우드 확장과 데이터 주권을 보장하며, Azure PostgreSQL, Red Hat OpenShift 등 주요 플랫폼 서비스가 각 지역에 빠르게 적용되고 있습니다.

마지막으로, Azure의 리타이어먼트 및 정책 변경(예: 예약 교환 정책 개편, Python/PowerShell 구버전 지원 종료 등)은 장기적인 플랫폼 품질 보존 및 혁신 가속을 위한 견고한 구조 개편의 신호탄입니다.

## 컴퓨트 및 컨테이너 🚀

이번 달 컴퓨트 및 컨테이너 부문에서는 현대적 인프라와 언어 지원에 대폭적인 전환이 있었습니다.  
AKS에서 Gateway API 기반의 애플리케이션 라우팅이 정식 지원되어 표준화된 인그레스 관리 모델을 제공하며, 기존 nginx 인그레스 방식에서의 점진적 마이그레이션도 쉽게 지원됩니다.  
Azure Functions는 Python 3.14와 PowerShell 7.6(정식 지원 및 미리 보기)을 동시에 도입해 개발자와 운영팀의 최신 환경 전환을 지원하고, AKS Prepared Image Spec 미리보기로 컨테이너 노드 초기화 시간 단축 및 예측 가능성이 높아졌습니다.  
Kubernetes Fleet Manager의 리소스 배치와 실패 허용 설정(미리보기)은 대규모 멀티 클러스터 관리에서의 유연성과 자동화 트렌드를 반영한 혁신입니다.

### [Application Routing with Gateway API](https://azure.microsoft.com/updates?id=567944)
AKS에서 Gateway API 기반 애플리케이션 라우팅이 정식 지원되어 더욱 표준화된 인그레스 관리 모델로 전환할 수 있습니다.

### [Azure Functions support for Python 3.14](https://azure.microsoft.com/updates?id=567646)
Python 3.14이 Azure Functions에서 정식 지원됨에 따라, 최신 보안과 장기적 호환성을 확보할 수 있습니다.

### [Azure Automation supports PowerShell 7.6 runbooks and Runtime environment](https://azure.microsoft.com/updates?id=568102)
Azure Automation이 PowerShell 7.6 런북 및 최신 런타임 환경 정식 지원으로 코드 이식성과 모듈 충돌 최소화가 가능해졌습니다.

### [Prepared Image Specification in AKS (미리 보기)](https://azure.microsoft.com/updates?id=567949)
AKS에서 미리 지정된 이미지 사양을 적용해 노드 시작 시간을 단축하고 성능을 예측할 수 있습니다.

### [Maximum allowed failures for update runs in Kubernetes Fleet Manager (미리 보기)](https://azure.microsoft.com/updates?id=567939)
Fleet Manager의 업데이트 실패 허용 임계값 기능으로 대규모 클러스터 롤아웃 시 실패 관리가 더욱 유연해졌습니다.

## AI 및 데이터 분석 💡

AI 및 데이터 분석 영역에서는 Azure Databricks가 Anthropic Claude Sonnet 5, Opus 5, OpenAI GPT-5.6 등 최신 LLM을 신속히 도입하면서 엔터프라이즈의 고도화된 AI 활용을 지원하고 있습니다.  
특히 데이터 웨어하우스의 Serverless 옵션 확대와 함께 고성능 자동 확장, 비용 효율, 거버넌스 연계가 강화되었습니다.  
또한 Azure Event Hubs와 Databricks의 보안(Confidential Computing), 네트워크 격리(Perimeter)도 기업의 데이터 보호 및 신뢰성 확보에 크게 기여하고 있습니다.

### [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)
UK West 지역에서 Databricks SQL Serverless가 도입되어 신속한 분석과 자동 확장이 가능한 환경을 제공합니다.

### [Claude Opus 5 on Azure Databricks](https://azure.microsoft.com/updates?id=568316)
최신 AI 모델 Claude Opus 5로 고도화된 추론, 코딩, 전문가 작업을 Azure Databricks에서 구현할 수 있습니다.

### [Open AI GPT-5.6 on Azure Databricks](https://azure.microsoft.com/updates?id=567431)
GPT-5.6이 Databricks에서 지원되며, Foundry 연계로 AI 기반 비즈니스 혁신을 심화할 수 있습니다.

### [Confidential Computing support for Azure Event Hubs Dedicated](https://azure.microsoft.com/updates?id=567212)
Event Hubs Dedicated가 Confidential Computing을 지원해 메모리 내 데이터 보호를 한층 강화했습니다.

### [Network Security Perimeter support for Azure Event Hubs](https://azure.microsoft.com/updates?id=567203)
Event Hubs에서 네트워크 보안 경계(Network Security Perimeter) 기능 도입으로 PaaS 자원의 논리적 격리와 공용 네트워크 접근 제어가 가능해졌습니다.

## 네트워크 및 보안 🔒

네트워크와 보안 카테고리에서는 Azure Firewall의 HTTP 헤더 삽입, VPN Gateway IPv6/IPv4 듀얼 스택 지원, NAT64, DDoS Protection 맞춤 정책, Front Door의 엣지 액션과 WAF 예외 기능(모두 미리 보기) 등 네트워크 경계 강화와 트래픽 처리 다양화가 두드러졌습니다.  
Azure Enclave는 정부와 규제 산업, 고보안 요구 환경에 선도적인 네트워크 분리, 권한 관리, 모니터링을 제공합니다.  
Key Vault는 AES 기반 대칭키(미리 보기)로 포스트 양자 암호화 대비 기능을 실현합니다.

### [HTTP header insertion in Azure Firewall](https://azure.microsoft.com/updates?id=568115)
Azure Firewall에서 HTTP 헤더 삽입 기능이 도입되어 인증, 접근제어, 뒤 서비스 연동이 용이해졌습니다.

### [IPv6 support for Azure VPN Gateway](https://azure.microsoft.com/updates?id=567847)
VPN Gateway에 IPv6 내부 트래픽 지원이 추가되어 듀얼 스택 환경을 통한 현대적 워크로드 적용이 가능해졌습니다.

### [NAT64 on StandardV2 NAT Gateway](https://azure.microsoft.com/updates?id=568409)
IPv6 기반 워크로드가 IPv4 전용 인터넷으로 접근할 수 있는 NAT64 지원이 추가되었습니다.

### [Azure DDoS Protection custom policy (미리 보기)](https://azure.microsoft.com/updates?id=568063)
DDoS Protection에 맞춤형 정책 설정이 가능해져 인바운드 트래픽에 대해 세분화된 보호 설정을 적용할 수 있습니다.

### [Azure Enclave (미리 보기)](https://azure.microsoft.com/updates?id=568377)
Azure Enclave가 민감한 워크로드 보안과 격리를 위한 관리형 인프라 패턴 제공으로 정부 및 규제산업 데이터 보호를 한층 높입니다.

## 스토리지 및 데이터베이스 🗄️

이번 달 스토리지 및 데이터베이스 부문은 무결성·보안·이식성·운영 효율에 집중되었습니다.  
Blob Storage는 클라이언트 무결성 보호와 SFTP Entra ID 접근을 지원하고, Azure Files는 AKS NFS 볼륨 암호화(정식 지원)로 생산환경 데이터 보안성을 높입니다.  
Storage Mover는 Google Cloud Storage에서 Blob으로 이식(미리 보기)을 지원하며, NetApp Files는 SMB Oplocks 설정(미리 보기)을 추가하여 하이브리드 환경 및 백업 시나리오의 활성화를 촉진합니다.

### [Client-side data integrity protections in Azure Blob Storage](https://azure.microsoft.com/updates?id=566895)
Blob Storage SDK에 CRC64-NVME 기반 클라이언트 무결성 보호가 도입되어 엔드투엔드 데이터 신뢰성을 제공합니다.

### [Microsoft Entra ID-based access for Azure Blob Storage SFTP](https://azure.microsoft.com/updates?id=567085)
Entra ID 인증 기반 SFTP 접근 정식 지원으로 사용자 관리 간소화와 보안 강화가 가능해졌습니다.

### [Encryption in Transit for Azure Files NFS Shares in AKS](https://azure.microsoft.com/updates?id=567787)
Azure Files NFS 볼륨과 AKS 사이의 데이터 전송 암호화(정식 지원)로 보안 및 규제 대응능력이 향상됩니다.

### [Public Preview: Azure Storage Mover now supports migration from Google Cloud Storage (GCS)](https://azure.microsoft.com/updates?id=566948)
Storage Mover가 GCS에서 Blob Storage로의 클라우드간 데이터 이식을 지원하며 안전한 네트워크와 자동화 기반 등록을 제공합니다.

### [Support for SMB Opportunistic Locking (Oplocks) configuration (미리 보기)](https://azure.microsoft.com/updates?id=568396)
NetApp Files에서 SMB Oplocks 설정이 가능해 클라이언트 캐싱 최적화 및 볼륨간 독립 설정이 효율적으로 이루어집니다.

## 관리, 운영 및 마이그레이션 ⚙️

플랫폼 관리와 마이그레이션 부문에서는 운영 자동화의 언어 환경 고도화, Site Recovery의 대상 변화량 대폭 강화, Chaos Studio의 시나리오 중심 자동화 테스트, Log Analytics와 Monitor의 Fabric 연계(미리 보기), 오토메이션·플랫폼 언어 사용 중단과 예약 교환 정책 개편 등 클라우드 운영 체계의 안정성과 변화 대응 능력이 한층 강화되었습니다.

### [Azure Automation supports PowerShell 7.6 runbooks and Runtime environment](https://azure.microsoft.com/updates?id=568102)
최신 PowerShell 7.6 런북과 런타임 환경 정식 지원으로 스크립트 실행 및 업그레이드 체계가 간소화됩니다.

### [Support 5x churn in Azure Site Recovery](https://azure.microsoft.com/updates?id=566966)
Site Recovery의 변화량 지원이 VM 당 500MB/s로 확대되어 빅데이터, 고IOPS 워크로드 보호가 가능합니다.

### [Azure Chaos Studio Workspaces and Scenarios (미리 보기)](https://azure.microsoft.com/updates?id=567184)
Chaos Studio가 워크스페이스와 시나리오 중심 테스트 기능을 도입해 실제 장애상황 재현과 보고서를 손쉽게 생성합니다.

### [Azure Monitor Logs mirroring into Microsoft Fabric (미리 보기)](https://azure.microsoft.com/updates?id=568322)
Azure Monitor 로그를 Fabric으로 직접 미러링하여 실시간 분석, OneLake 저장, 고급 분석이 가능해졌습니다.

### [Support for Python-2.7; 3.8 and PowerShell- 7.1; 7.2 will be retired on September 30, 2026](https://azure.microsoft.com/updates?id=567556)
Automation 환경에서 Python 2.7, 3.8, PowerShell 7.1/7.2 지원 종료 예고로 최신 버전 전환이 필수화되었습니다.

## Microsoft Foundry & Fabric 🏭

Microsoft Foundry는 AI 서비스와 데이터 거버넌스, 도구 집합 구성 등 조직 내 혁신 역량을 대폭 강화했습니다.  
PII Playground와 Toolbox는 실시간 평가와 공통 도구 호출이 실현되어 개발팀간 자산 재사용과 거버넌스 일관성을 높입니다.  
Fabric 연계(미리 보기)는 Azure Monitor 데이터의 OneLake 즉시 연계와 엔터프라이즈 분석의 신속성·효율성을 극대화합니다.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)
PII Playground 정식 지원으로 문서 기반 개인정보 식별·평가의 신속성과 실시간 인사이트 활용이 가능해졌습니다.

### [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)
Toolbox 기능 정식 지원으로 조직 내 통합 도구 호출 및 거버넌스 정책 활용이 간결하게 설계되었습니다.

### [Document PII playground sample in Microsoft Foundry NextGen (미리 보기)](https://azure.microsoft.com/updates?id=563331)
Foundry NextGen 포털에서 문서 기반 PII 탐색 샘플 기능(미리 보기)이 도입되어 실시간 결과 평가가 가능해졌습니다.

### [Azure Monitor Logs mirroring into Microsoft Fabric (미리 보기)](https://azure.microsoft.com/updates?id=568322)
모니터링 데이터를 Fabric에 실시간 미러링해 비즈니스 데이터와 통합 분석, 고급 머신러닝 적용이 가능합니다.

### [Protect sensitive generative AI telemetry in Application Insights and Microsoft Foundry (미리 보기)](https://azure.microsoft.com/updates?id=567594)
Foundry 및 Application Insights에서 생성형 AI 텔레메트리 보호 기능이 강화되어 민감 데이터 접근관리, 규제 준수성이 크게 향상되었습니다.

## 지역 및 글로벌 확장 🌏

이번 달에는 인도 South Central, 칠레 Central 등 신규 Azure 지역이 개설되어 글로벌 확장성과 현지 데이터 주권, 규제 대응에 초점을 맞춘 혁신이 지속되었습니다.  
해당 지역에서 PostgreSQL, Red Hat OpenShift 등 주요 서비스가 정식 지원되어 현지 고객의 클라우드 중심 전환과 고성능 워크로드 적용이 용이해졌습니다.

### [Microsoft Azure now available from new cloud region in India (India South Central)](https://azure.microsoft.com/updates?id=568013)
인도 Hyderabad에 새로운 데이터센터 지역 개설로 현지 AI, 클라우드 서비스 수요 대응 및 데이터 주권 강화가 실현되었습니다.

### [Azure Database for PostgreSQL flexible server in India South Central](https://azure.microsoft.com/updates?id=568334)
India South Central 지역에서 PostgreSQL Flexible Server를 정식 지원해 데이터베이스 업무 확장성이 높아졌습니다.

### [Azure Red Hat OpenShift in Chile Central](https://azure.microsoft.com/updates?id=566732)
칠레 Central 지역에서 OpenShift 정식 지원으로 현지 클라우드 인프라, 규제 산업 고객이 안정적으로 하이브리드 Kubernetes 환경을 활용할 수 있게 되었습니다.

### [New Powershell module: Az.PostgreSQLFlexibleServer](https://azure.microsoft.com/updates?id=566209)
새로운 Az.PostgreSQLFlexibleServer PowerShell 모듈로 최신 PostgreSQL 기능 관리 및 운영 효율이 강화되었습니다.

### [Microsoft Defender security assessments for Azure Database for PostgreSQL Flexible Server](https://azure.microsoft.com/updates?id=567527)
Azure PostgreSQL Flexible Server 보안 평가 정식 지원으로 지속적 취약점 점검, 규제 준수, 자동화 보호가 실현되었습니다.

## 정책 변경, 사용 중단 및 공지 📣

이번 달에는 Azure 예약 교환 정책이 2027년 2월부터 변경될 예정이며, 일부 Compute·Database 서비스 예약 교환이 종료됩니다.  
또한 Python 2.7, 3.8, PowerShell 7.1, 7.2은 2026년 9월 30일 이후 지원이 종료될 예정이므로 운영 자동화 환경의 최신 전환이 필수화되었습니다.

### [Reservation exchanges for Azure services supported by savings plans will no longer be available starting February 1, 2027](https://azure.microsoft.com/updates?id=568514)
2027년 2월 이후 Savings Plan이 적용된 Azure 서비스(Compute, Database 등)에 대한 예약 교환이 종료될 예정입니다.

### [Support for Python-2.7; 3.8 and PowerShell- 7.1; 7.2 will be retired on September 30, 2026](https://azure.microsoft.com/updates?id=567556)
2026년 9월 30일 이후 해당 런타임 버전의 오토메이션 통합 지원이 종료되어 보안 및 기능 유지를 위해 최신 버전으로의 업그레이드가 필요합니다.

---

## 이번 달 총평 및 다음 달 전망

2026년 7월 Azure 업데이트는 AI, 데이터 분석, 네트워크·보안, 멀티 클라우드 및 글로벌 확장에 중점을 둔 대규모 혁신이 계속되고 있음을 보여줍니다.  
기능의 정식 지원과 미리 보기(Preview)의 보폭이 넓어지고, 데이터 신뢰성·보안·관리 효율성·규제 대응이 강화되었습니다.  
특히 AI 모델의 신속한 도입과 Foundry/Fabric 기반 데이터 거버넌스는 엔터프라이즈 디지털 전환 체계를 견고하게 만들고 있습니다.

다음 달에는 Fabric 및 Foundry 중심의 AI·데이터 관리 기능 확대, AKS 및 Kubernetes 운영 자동화 강화, 글로벌 지역별 추가 확장 및 고성능 워크로드 대응에 대한 지속적인 혁신이 예상됩니다.  
보안·네트워크 부문에서는 DDoS, Enclave, Firewall 등 지속적인 강화와 사용자 맞춤화 정책이 계속 될 것으로 전망됩니다.  
정책 변경과 사용 중단 공지를 통한 클라우드 체계의 품질 고도화와 미래 대비 움직임도 꾸준히 이어질 것입니다.