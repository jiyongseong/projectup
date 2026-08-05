# Azure 월간 업데이트 요약 - 2026년 07월

## 전반적인 트렌드와 핵심 인사이트

2026년 7월의 Azure 업데이트는 AI 기반 클라우드 혁신과 인프라 현대화, 보안 강화, 멀티 리전 확장, 그리고 오픈 소스 및 자동화 생태계의 탁월한 발전을 보여준다. 세계적으로 AI와 데이터 분석 서비스의 정식 지원 확대가 두드러지며, Anthropic Claude Opus 5, Claude Sonnet 5, OpenAI GPT-5.6 등 최신 AI 모델이 Azure Databricks와 Microsoft Foundry를 통해 본격적으로 도입되어 AI 기반 업무 자동화와 복잡한 엔터프라이즈 데이터 활용이 한층 가속화되고 있다.

또한, Kubernetes 생태계와 관리 경험의 혁신도 표면적으로 부상하고 있다. Gateway API 기반의 애플리케이션 라우팅, Kubernetes Fleet Manager의 리소스 일괄 배포와 업데이트 실패 허용치 설정 등으로 클라우드 네이티브 환경에서 운영 자동화와 민첩성이 크게 향상됐다. 인프라에선 인도 South Central과 칠레 Central 같은 신규 리전 출시로 글로벌 확장과 데이터 주권, 레이턴시 최소화가 강조되고 있으며, Storage, Networking, Databases 등 주요 서비스에는 신기능이 안정적으로 적용되고 있다.

보안과 컴플라이언스 역시 강화 추세다. Azure Event Hubs Dedicated의 기밀 컴퓨팅, Azure Blob Storage의 클라이언트 측 데이터 무결성, Azure VPN Gateway의 IPv6 지원, Azure Firewall의 HTTP 헤더 삽입 등 다양한 계층에서 규제 요건과 신뢰성 확보를 위한 기술적 기능들이 대거 정식 지원된다. 자동화에서는 PowerShell 7.6 과 Python 3.14의 지원으로 지속적인 언어 환경 업그레이드와 스크립트 관리의 효율성이 증대되고, 미리 보기 단계의 다양한 신기능(예: Azure API Management의 AI Gateway, Chaos Studio의 시나리오, Azure Disk Storage의 Instant Access 등)이 ‘유연성·통제·보안’을 한층 다각적으로 실현한다.

특히 Microsoft Foundry와 Microsoft Fabric에선 AI 에이전트 툴박스, PII 플레이그라운드(문서 기반 개인정보 검출), Azure Monitor와 Microsoft Fabric의 실시간 로그 미러링 등 조직 내 생산성·데이터 분석 통합·보안 체계 혁신을 주도하는 초거대 기능들이 발표됐다. 결론적으로 이번 달은 AI, 데이터, 자동화, 보안의 시너지가 Azure 전역에 걸쳐 실질적 변화로 나타난 시점이며, 글로벌 리전 확대와 신기능으로 엔터프라이즈 클라우드의 미래 경쟁력이 한층 확고해지고 있다.

---

## 1. ☁️ 컴퓨트 및 컨테이너

이번 달 컴퓨트 및 컨테이너 분야는 Kubernetes 관리 모델의 진화와 함수 런타임의 최신 언어 지원, AKS의 암호화와 이미지 규격 혁신이 주요 트렌드로 나타났다. 특히 Gateway API 기반 애플리케이션 라우팅과 Fleet Manager의 일관된 리소스 배포, 그리고 AKS 노드 이미지의 사전 준비 이미지 스펙 도입으로 대규모 클라우드 네이티브 환경 구축이 쉬워지고 머신 유지보수와 확장성, 보안이 전보다 효율적으로 개선됐다. Azure Functions에서는 Python 3.14와 PowerShell 7.6으로 개발 환경이 현대화되었고, Instant Access VM Restore Points와 Azure Sphere OS 26.09 평가판 출시로 관리, 복구, IoT 기반 운영 신뢰도가 크게 향상됐다.

### [Application Routing with Gateway API](https://azure.microsoft.com/updates?id=567944)
AKS에서 Gateway API 기반 애플리케이션 라우팅을 정식 지원하여 기존 ingress-nginx 기반 라우팅보다 표준화된 모델을 도입. 점진적 마이그레이션을 지원하며, 서비스 메쉬 없이 경량화된 구성 가능.

### [Azure Functions support for Python 3.14](https://azure.microsoft.com/updates?id=567646)
Azure Functions에서 Python 3.14를 정식 지원하여 개발 환경의 최신화와 보안성 및 장기 지원이 보장됨.

### [Public Preview: Azure Functions Support for PowerShell 7.6](https://azure.microsoft.com/updates?id=567651)
PowerShell 7.6이 Azure Functions에 미리 보기로 제공되어, 확장성 높은 함수 개발과 최신 스크립트 환경을 활용할 수 있게 됨.

### [Resource placement in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567931)
Fleet Manager에서 리소스 일괄 배포 기능이 정식 지원됨. 쿠버네티스 리소스들을 여러 클러스터에 자동 배포할 수 있어 운영 효율성 향상.

### [Azure Sphere OS version 26.09 is now available for evaluation](https://azure.microsoft.com/updates?id=568466)
Azure Sphere OS 26.09 평가판이 출시되어, IoT 디바이스의 보안 커널·장기 지원 운영체제 환경으로 전환 테스트가 가능해짐.

---

## 2. 🛰️ 네트워킹 및 보안

네트워킹과 보안 영역은 기업용 네트워크 경계 강화와 서비스별 트래픽 제어, 다양한 보안 정책의 유연성 및 IPv6 기반 글로벌 연결성 향상을 중심으로 진화했다. Azure Firewall의 헤더 삽입, VPN Gateway의 IPv6 지원, NAT64 도입, Azure DDoS Protection의 커스텀 정책, Front Door의 Edge Actions, 그리고 Enclave 미리 보기 등 네트워크 및 보안 운영 자동화와 규정 준수·데이터 보호의 다양성이 뛰어나게 확대되었다.

### [HTTP header insertion in Azure Firewall](https://azure.microsoft.com/updates?id=568115)
Azure Firewall에서 HTTP 헤더 삽입을 정식 지원, 온프레미스 프록시 대체 및 엔터프라이즈 Tenant 제어에 필수 기능.

### [IPv6 support for Azure VPN Gateway](https://azure.microsoft.com/updates?id=567847)
IPv6 지원이 VPN Gateway에 적용되어, 듀얼 스택 구성 및 브랜치/ 원격 연결에서 IPv6 트래픽 지원 가능.

### [NAT64 on StandardV2 NAT Gateway](https://azure.microsoft.com/updates?id=568409)
StandardV2 NAT Gateway가 NAT64를 지원해 IPv6 워크로드의 IPv4 목적지 통신을 자연스럽게 DNS64·NAT64 기반으로 처리.

### [Azure DDoS Protection custom policy](https://azure.microsoft.com/updates?id=568063)
Azure DDoS Protection에서 커스텀 정책을 미리 보기로 제공, 서비스별 임계치 조절로 이벤트별 맞춤 대응이 가능.

### [Azure Enclave](https://azure.microsoft.com/updates?id=568377)
Azure Enclave가 미리 보기로 공개되어, 정부 및 규제 산업에 격리된 네트워크 경계와 데이터·사용자 권한 중앙화 관리 기능 제공.

---

## 3. 📊 데이터베이스 및 분석

AI 및 Big Data 분석 서비스가 대거 정식 지원됐고, PostgreSQL 관리 모듈/Powershell, 지역별 신규 지원, Event Hubs 기밀 컴퓨팅과 네트워크 경계 기능 추가로 데이터 보호 및 컴플라이언스 대응이 다각적으로 확장됐다. Azure Databricks에 최신 AI 모델이 연이어 출시되어 데이터 기반 인사이트·코딩 작업의 자동화가 강화됐으며, Azure Database for PostgreSQL에선 클라우드 보안 평가 및 관리 PowerShell 모듈이 추가됐다.

### [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)
UK West 리전에서 Azure Databricks SQL Serverless 정식 지원, 즉시 컴퓨트 및 자동 확장·인프라 관리 절감 효과.

### [Claude Opus 5 on Azure Databricks](https://azure.microsoft.com/updates?id=568316)
Anthropic Claude Opus 5 AI 모델이 Databricks에서 지원됨. 고도 추론, 코딩, 에이전트 자동화 등 복잡한 업무에 활용.

### [Azure Database for PostgreSQL flexible server in India South Central](https://azure.microsoft.com/updates?id=568334)
Azure Database for PostgreSQL의 India South Central 리전 정식 지원으로, 클라우드 데이터베이스의 지역 확장과 데이터 접근 최적화.

### [Microsoft Defender security assessments for Azure Database for PostgreSQL Flexible Server](https://azure.microsoft.com/updates?id=567527)
PostgreSQL Flexible Server 대상 Microsoft Defender CSPM(Security Posture Management) 평가 도입, 지속적 보안 점검과 취약점 분석 가능.

### [New Powershell module:  Az.PostgreSQLFlexibleServer](https://azure.microsoft.com/updates?id=566209)
Az.PostgreSQLFlexibleServer PowerShell 모듈 신규 출시, 최신 플랫폼 기능과 PostgreSQL 18 관리·Elastic 클러스터 지원.

---

## 4. 🏗️ 스토리지 및 마이그레이션

스토리지 및 마이그레이션은 데이터 무결성, 암호화, 네트워크 격리, 마이그레이션 간소화와 클라우드 오퍼레이션 성능 최적화에 중점을 두었다. Blob Storage의 클라이언트 무결성 기능과 SFTP Entra ID 인증, Azure Files의 NFS 암호화, Storage Mover의 GCS 지원은 조직의 데이터 전략을 안전하고 효율적으로 전환하는 데 도움이 됐다.

### [Client-side data integrity protections in Azure Blob Storage](https://azure.microsoft.com/updates?id=566895)
Azure Blob Storage SDK (.NET, C++, JS)에 클라이언트 측 CRC64-NVME 데이터 무결성 검증 도입. 완전한 end-to-end 데이터 보호 제공.

### [Microsoft Entra ID-based access for Azure Blob Storage SFTP](https://azure.microsoft.com/updates?id=567085)
Entra ID 기반 SFTP 접속을 통합하여 외부 협업 및 보안 강화, 온프레미스 사용자 관리 없이 추가 인증과 액세스 정책 적용 가능.

### [Encryption in Transit for Azure Files NFS Shares in Azure Kubernetes Service (AKS)](https://azure.microsoft.com/updates?id=567787)
AKS에서 Azure Files NFS v4.1 볼륨의 데이터 전송 암호화 정식 제공(TLS 기반), 스토리지 클래스로 활성화 가능.

### [Public Preview: Azure Storage Mover now supports migration from Google Cloud Storage (GCS)](https://azure.microsoft.com/updates?id=566948)
Storage Mover가 Google Cloud Storage와 호환되어 Azure로 데이터 이전·통합이 Agentless·보안·비공개 네트워크 방식으로 가능.

### [Instant Access via application consistent restore points](https://azure.microsoft.com/updates?id=565758)
Azure Disk Storage에서 즉각 VM 디스크 복구를 지원하는 ‘Instant Access’ 미리 보기 출시, 신속한 복구 및 일관된 애플리케이션 상태 확보.

---

## 5. 🛠️ 관리 및 거버넌스·운영 자동화

관리 및 운영 자동화 영역은 PowerShell 7.6, Python 3.14 확장, Site Recovery 고성능 지원, Chaos Studio의 워크스페이스·시나리오, Log Analytics 데이터 이관 등으로 실시간 관리와 대규모 환경 내 신속한 복구·시나리오 검증·데이터 활용성이 극대화됐다. 자동화 런타임의 정식 지원과 고성능 마이그레이션 정책, Azure Monitor와 Fabric 통합으로 엔터프라이즈 환경의 효율성과 보안성도 한층 강화됐다.

### [Azure Automation supports PowerShell 7.6 runbooks and Runtime environment](https://azure.microsoft.com/updates?id=568102)
PowerShell 7.6 런북·런타임 정식 지원. 스크립트 환경 업그레이드와 Azure CLI 명령 지원, 모듈 분리 없이 효율적인 운영 가능.

### [Support 5x churn in Azure Site Recovery](https://azure.microsoft.com/updates?id=566966)
Site Recovery가 VM당 최대 500MB/s 처리량 지원, 고성능 분석/데이터베이스 등 대규모 IOPS 워크로드에 탄탄한 재해복구 제공.

### [Azure Chaos Studio Workspaces and Scenarios](https://azure.microsoft.com/updates?id=567184)
Chaos Studio에 작업 공간/시나리오 미리 보기 출시. 실제 장애 패턴 자동화 검증, DORA 및 컴플라이언스 보고서 내장.

### [Manage Azure Chaos Studio from the Azure CLI](https://azure.microsoft.com/updates?id=567225)
CLI 기반 Chaos Studio 시나리오 관리 미리 보기로, 자동화된 작업 공간 구성 및 간편한 시나리오 테스트 제공.

### [Export historical data from Log Analytics workspace with Export jobs](https://azure.microsoft.com/updates?id=566591)
Log Analytics Export Job 미리 보기 출시. 지정 쿼리/기간 기반 데이터 외부 이동, 고급 분석 및 기록 보존에 활용.

---

## 6. 🧩 Microsoft Foundry 및 Microsoft Fabric

Foundry와 Fabric은 조직별 AI·데이터 통합·보안 자동화에 특화된 새로운 기능들을 대거 선보인다. Toolboxes의 에이전트 툴 일괄화, 문서 PII 검출 플레이그라운드, Application Insights의 GenAI 보호, Fabric과 Azure Monitor 로그 미러링 등으로 생산성·AI 보안·대량 로그 분석이 한층 쉬워졌다.

### [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)
Foundry에서 Toolboxes 정식 지원. 에이전트 간 공통 도구 통합 및 재사용, 통제된 MCP 엔드포인트 제공.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)
문서 개인정보 검출 플레이그라운드 정식 지원. 내장 샘플로 빠른 평가 및 각 유형 감지·리뷰 단일 화면 제공.

### [Public Preview: Document PII playground sample in Microsoft Foundry NextGen](https://azure.microsoft.com/updates?id=563331)
미리 보기로 문서 기반 PII 검출 플레이그라운드 샘플 출시, 실시간 Redaction 결과와 신뢰도·엔티티 확인 가능.

### [Protect sensitive generative AI telemetry in Application Insights and Microsoft Foundry](https://azure.microsoft.com/updates?id=567594)
Application Insights, Foundry에서 GenAIContent 테이블 기반 AI 텔레메트리 권한 분리. 신규 관리 역할 적용으로 PII/PHI 등 민감 정보 보호.

### [Azure Monitor Logs mirroring into Microsoft Fabric](https://azure.microsoft.com/updates?id=568322)
Azure Monitor Log Analytics 데이터를 Microsoft Fabric OneLake에 실시간 미러링(Delta Parquet), Fabric의 분석·BI·ML과 연계 가능.

---

## 7. 🚀 리전 및 정책, 가격, 지원 종료

전세계 리전 확장, 고가용성 정책, 중장기 가격 정책 변화, 런타임 지원 종료, 예약(Legacy Reservation) 교환 정책 업데이트 등 글로벌 전략의 변화가 두드러졌다. 특히 인도 South Central 리전의 신규 개설과 칠레 Central 리전의 OpenShift 지원은 신흥 시장과 현지 데이터 규제 대응의 대표 사례로 꼽힌다.

### [Microsoft Azure now available from new cloud region in India (India South Central)](https://azure.microsoft.com/updates?id=568013)
인도 South Central 리전 신규 오픈, 현지 데이터 주권·AI 기반 인프라·고가용성 제공.

### [Azure Red Hat OpenShift in Chile Central](https://azure.microsoft.com/updates?id=566732)
칠레 Central 리전에서 OpenShift 정식 지원, 남미 지역 레이턴시·데이터 거버넌스 강화.

### [Announcing: Reservation exchanges for Azure services supported by savings plans will no longer be available starting February 1, 2027](https://azure.microsoft.com/updates?id=568514)
2027년 2월 1일부터 Savings Plan 대상 예약 교환 정책 변경, 서비스별 예약 교환 제한 및 최종 교환 권리 명확화.

### [Retirement: Support for Python-2.7; 3.8 and PowerShell- 7.1; 7.2 will be retired on September 30, 2026](https://azure.microsoft.com/updates?id=567556)
2026년 9월 30일 이후 Python 2.7, 3.8, PowerShell 7.1/7.2 지원 종료, 보안/버그 수정 및 공식 지원 중단.

### [Standard service endpoint](https://azure.microsoft.com/updates?id=561475)
퍼블릭 프리뷰로, Private Link 기반의 대규모 IaaS-to-PaaS 연결 지원. 네트워크 경계 통제와 공공 IP 기반 식별 가능.

---

## 이번 달 총평 및 다음 달 전망

2026년 7월 Azure 업데이트는 ‘혁신적 AI 도입과 거버넌스 강화, 다중 리전 확장, 엔터프라이즈 보안 및 자동화의 실질적 진화’가 핵심이다. 특히 AI와 데이터 분석, Kubernetes 클라우드 네이티브 관리, Storage 환경의 비약적인 변화와 보안 기능의 확대가 실무에 직접적인 영향을 미쳤다. Microsoft Foundry와 Fabric을 포함한 새 기능들은 조직의 생산성과 보안, 혁신을 한 단계 끌어올릴 기반을 마련했다. 또한, 인도와 남미 등 신규 리전 확장으로 글로벌 경쟁력이 강화됐다.

다음 달에는 AI 및 데이터 워크로드 중심의 신규 기능 출시, 전 세계 리전 확대, 자동화·보안·관리 체계 첨단화가 예상된다. 런타임 지원 종료와 정책 변화에 따라 실무 환경의 언어 업그레이드 및 서비스 선택이 중요해질 것이며, 미리 보기 기능의 정식 출시 및 컴플라이언스 규제 대응에 대한 새로운 전략 제시가 기대된다. Azure는 지속적으로 혁신과 신뢰성을 앞세워 클라우드 시장 리더십을 강화하고 있다.