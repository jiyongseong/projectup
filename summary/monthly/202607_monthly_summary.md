# Azure 월간 업데이트 요약 - 2026년 07월

## 전반적인 트렌드와 핵심 인사이트

2026년 7월의 Azure 업데이트는 AI, 클라우드 기반 개발, 데이터 보안, 멀티클라우드 및 레거시 환경 관리, 네트워크 혁신 등 다양한 분야에서 기술적 진보와 고객 중심의 변화가 두드러졌습니다. 이번 달은 특히 정식 지원을 통한 서비스 안정화, 공개 미리 보기(Preview)로 혁신 기술 실험 확대, 플랫폼 간 통합 및 자동화 개선에 집중되었습니다.

데이터 및 워크로드의 글로벌 확대에 맞춰 인도, 칠레 등 신규 지역에서 Azure 서비스가 활성화되며, 지역 특성과 규제 대응이 점점 강화되고 있습니다. Kubernetes 및 컨테이너 운영 환경에서는 최신 API, 보안 및 효율적 자원 분배 기능이 적용되어 기업의 DevOps/클라우드 네이티브 운영을 지원합니다. AI와 머신러닝 관련 신기술은 Databricks 플랫폼과 Microsoft Foundry의 엔터프라이즈용 통합으로 확장되며, 대규모 데이터 분석과 보안, 컴플라이언스까지 포괄하는 솔루션이 제공되는 모습이 눈에 띕니다.

네트워킹과 스토리지 영역에서는 클라우드 간 마이그레이션, 네트워크 경계 설정, 데이터 무결성/보안 강화 등이 꾸준히 개선되고 있으며, 데이터 보호와 접근 정책의 유연성이 높아지는 점이 올해 Azure 업데이트의 주요 방향으로 보입니다. 또한, 관리 및 자동화 도구의 최신 런타임 환경·스크립트 지원, 퇴출 정책 안내 등 고객의 운영 효율성과 보안 유지를 위한 변화도 지속적으로 반영되고 있습니다.

결국, Azure는 글로벌 확장, 혁신적 AI 도구, 보안과 컴플라이언스 강화, 멀티클라우드 운영 효율 제고, 네이티브 통합 및 자동화 기술 고도화라는 2026년 하반기 트렌드를 선도하고 있습니다.

---

## ☁️ 컴퓨트, 컨테이너, IoT

이번 달 Azure는 Kubernetes 인그레스 관리, AKS API 표준화, Python 3.14 및 PowerShell 7.6 런타임 지원 등 개발환경 진화를 중점적으로 추진했습니다. AKS와 Kubernetes Fleet Manager는 자원 배치, 이미지 사양, 업데이트 실패 허용 등 운영 자동화와 대규모 관리 유연성을 크게 높였습니다. Azure Functions, Sphere OS 등은 최신 언어와 환경 지원을 통해 개발자 경험과 보안을 강화하였습니다.

### [Application Routing with Gateway API](https://azure.microsoft.com/updates?id=567944)
AKS에서 Kubernetes Gateway API 기반의 인그레스 관리 기능이 정식 지원되며, 기존 nginx 인그레스는 11월까지 지원됩니다. 오픈소스 migration tool도 제공되어 점진적 전환이 가능해졌습니다.

### [Azure Automation supports PowerShell 7.6 runbooks and Runtime environment](https://azure.microsoft.com/updates?id=568102)
PowerShell 7.6 기반 런북과 런타임 환경이 정식 지원되어, 최신 스크립트 보안 및 성능 향상, Azure CLI와의 통합 등 최신 언어관리 효율이 개선되었습니다.

### [Azure Functions support for Python 3.14](https://azure.microsoft.com/updates?id=567646)
Python 3.14로 함수 개발 지원이 추가되고, 보안성·지원기간·개발 도구 호환성 등 전반적인 개발 환경이 개선되었습니다.

### [Azure Sphere OS version 26.09 is now available for evaluation](https://azure.microsoft.com/updates?id=568466)
Sphere OS 26.09 RC1이 평가용 릴리즈. 주요 Linux 커널 업그레이드로 장기 지원·보안 고도화를 제공하며, 9월까지 평가 후 정식 배포 예정입니다.

### [Resource placement in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567931)
멀티 클러스터 자원 분배 API 및 정책이 정식 지원되어, Fleet 기반 일관성 있는 자원 배치와 관리가 중앙화 및 효율적으로 변화하였습니다.

---

## 🔍 데이터베이스 & AI/머신러닝 (Databricks 연동 포함)

AI와 데이터 분석 기술이 기업 업무에 깊이 침투하며, Databricks 기반 고성능 모델(Claude Opus 5, GPT-5.6, Sonnet 5)과 SQL Serverless 기능의 지역 확대가 눈에 띕니다. 데이터베이스와 보안 기능도 PostgreSQL의 강화와 관련 클라우드 관리 효율성이 개선되었습니다.

### [Claude Opus 5 on Azure Databricks](https://azure.microsoft.com/updates?id=568316)
Anthropic Claude Opus 5 모델이 Databricks AI Model Serving에서 지원되어, 고도의 추론과 개발 보조 기능을 통한 데이터 기반 AI 작업 효율성이 확장되었습니다.

### [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)
UK West 지역에서 Databricks SQL Serverless를 활용하여 즉시 컴퓨트와 자동 확장, 관리 편의성을 제공, 대규모 분석 워크로드 대응이 가능하게 되었습니다.

### [Open AI GPT-5.6 on Azure Databricks](https://azure.microsoft.com/updates?id=567431)
Microsoft Foundry 연계 GPT-5.6 모델이 Databricks에서 정식 지원되어, 통합 AI Gateway, 보안 등 엔터프라이즈 AI 모델 운영이 강화되었습니다.

### [Generally available: Anthropic Claude Sonnet 5 on Azure Databricks](https://azure.microsoft.com/updates?id=567194)
Claude Sonnet 5 모델이 Databricks에 도입되어, 효율성과 적응형 추론(에이전트 워크플로우, 대규모 SW 개발 등)이 확장되었습니다.

### [New Powershell module: Az.PostgreSQLFlexibleServer](https://azure.microsoft.com/updates?id=566209)
PostgreSQL 관리용 Az.PostgreSQLFlexibleServer 모듈 공개, PostgreSQL 18, 탄력적 클러스터 등 최신 기능에 PowerShell 기반 관리가 효율적으로 변화되었습니다.

---

## 💾 스토리지 & 네트워킹

스토리지 및 네트워킹 분야에서는 데이터 무결성·내부 보안이 강화되고, 클라우드 간 마이그레이션, 네트워크 경계설정, IPv6 지원 등 다변화된 환경이 현실적으로 대응 가능해졌습니다.

### [Client-side data integrity protections in Azure Blob Storage](https://azure.microsoft.com/updates?id=566895)
.NET, C++, JS SDK 기반 클라이언트 엔드-투-엔드 데이터 무결성 검증(CRC64-NVME)이 도입되어, 애플리케이션-스토리지 간 데이터 보호가 강화되었습니다.

### [Encryption in Transit for Azure Files NFS Shares in Azure Kubernetes Service (AKS)](https://azure.microsoft.com/updates?id=567787)
AKS 아키텍처에서 Azure Files NFS 볼륨 간 데이터 암호화(TLS) 통신 기능이 정식 지원, 생산 환경의 보안 및 컴플라이언스 요구에 부합합니다.

### [Microsoft Entra ID-based access for Azure Blob Storage SFTP](https://azure.microsoft.com/updates?id=567085)
Entra ID 인증 기반 Blob Storage SFTP 접근이 전 지역에서 지원되어, 온프레미스/파트너 협업의 통합 및 보안·운영 효율이 크게 향상되었습니다.

### [IPv6 support for Azure VPN Gateway](https://azure.microsoft.com/updates?id=567847)
IPv6 트래픽 및 듀얼스택 VPN 터널 지원이 모든 프로덕션 SKU 게이트웨이에서 적용되어, 향후 네트워크 확장성과 보안이 강화되었습니다.

### [Public Preview: Azure Storage Mover now supports migration from Google Cloud Storage (GCS)](https://azure.microsoft.com/updates?id=566948)
Google Cloud Storage에서 Azure Blob Storage로 데이터 마이그레이션을 지원, 멀티클라우드 환경의 전환·통합이 보다 간편화되었습니다.

---

## 🛡️ 보안, 네트워킹, 관리/운영 혁신

보안 및 네트워크 관점에서는 네트워크 경계, DDoS, 다양한 인증 및 보호 정책의 미리 보기와 정식 지원 서비스가 대폭 강화되었습니다. 관리·컴플라이언스 분야도 런타임 지원 정책, 퇴출 안내 등 운영 리스크가 줄어들고 있습니다.

### [Confidential Computing support for Azure Event Hubs Dedicated](https://azure.microsoft.com/updates?id=567212)
Event Hubs Dedicated에서 Confidential Computing이 적용되어, 데이터 처리 시 메모리 내 보호 및 강력한 컴플라이언스 대응이 가능해졌습니다.

### [HTTP header insertion in Azure Firewall](https://azure.microsoft.com/updates?id=568115)
Azure Firewall에서 HTTP/HTTPS 헤더 삽입이 가능해져, 보안 통제·접근 정책·엔터프라이즈 통합 관리 편의성이 강화되었습니다.

### [NAT64 on StandardV2 NAT Gateway](https://azure.microsoft.com/updates?id=568409)
NAT64 지원으로 IPv6 워크로드가 IPv4만 지원하는 인터넷과 통신 가능, 클라우드 네이티브 네트워크 유연성이 확대되었습니다.

### [Network Security Perimeter support for Azure Event Hubs](https://azure.microsoft.com/updates?id=567203)
Event Hubs 네트워크 경계(NSP) 기능이 정식 지원되어, 퍼블릭 네트워크 접속 통제 등 중앙화된 보안 정책 수립이 용이해졌습니다.

### [Azure DDoS Protection custom policy (Preview)](https://azure.microsoft.com/updates?id=568063)
DDoS 보호 맞춤 정책 미리 보기를 통해, 트래픽 임계값 세분화 설정이 가능, 대형 이벤트·게임·고 IOPS 워크로드 등 상황 맞춤 네트워크 보호가 현실적으로 구현됩니다.

---

## 🧑‍💼 관리 및 거버넌스 (운영 자동화·이관·컴플라이언스)

운영 자동화와 이관·관리 툴의 발전, 스크립트 지원 정책 및 퇴출(지원 종료) 안내 등 Azure의 안정적 플랫폼 운용 역량이 확장되고 있습니다.

### [Support 5x churn in Azure Site Recovery](https://azure.microsoft.com/updates?id=566966)
Site Recovery에서 최대 5배 이상(500MB/s/VM) 변경점(Churn) 지원으로, 대량 데이터/빅데이터/분석 시스템의 재해복구 신뢰성·효율성이 크게 높아졌습니다.

### [Support for SMB Opportunistic Locking (Oplocks) configuration](https://azure.microsoft.com/updates?id=568396)
Azure NetApp Files에서 SMB 옵포튜니스틱 락(oplock) 설정이 가능, 캐시 최적화·볼륨 복제 등 효율운영이 지원됩니다.

### [Export historical data from Log Analytics workspace with Export jobs (Preview)](https://azure.microsoft.com/updates?id=566591)
Log Analytics 데이터의 시점별 쿼리·이동 기능 미리 보기로, 감사, 보안, 특수분석 등 데이터 관리 자동화가 강화되었습니다.

### [Support for Python-2.7; 3.8 and PowerShell- 7.1; 7.2 will be retired on September 30, 2026](https://azure.microsoft.com/updates?id=567556)
Automation 런북에서 위 버전 지원 종료 안내가 나왔으며, 최신 버전 업그레이드 필요성이 강조되고 있습니다.

### [Instant Access via application consistent restore points (Preview)](https://azure.microsoft.com/updates?id=565758)
VM 복구 지점 즉시 액세스 기능 미리 보기로, 백업 데이터에서 바로 복구 가능·RTO(복구시간) 단축 등 운영 효율성이 크게 향상되었습니다.

---

## 🏭 Microsoft Foundry & 🟥 Microsoft Fabric 업데이트

Foundry는 엔터프라이즈 AI, 개인정보 검출 Playground, Toolboxes 등 혁신적 AI 관리·운영 기능이 확대되고 있습니다. Fabric과 연계된 Azure Monitor Logs 미러링 등 비즈니스와 운영 데이터 통합 분석이 가능해졌습니다.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)
Foundry NextGen의 PII Playground가 정식 지원되어, 개인정보 검출·불필요한 업무 오버헤드를 최소화하는 실시간 평가 환경이 마련되었습니다.

### [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)
Foundry Toolboxes가 GA로, 통합된 엔드포인트와 조직의 재사용 가능한 AI 도구 관리 정책이 확립되었습니다.

### [Public Preview: Document PII playground sample in Microsoft Foundry NextGen](https://azure.microsoft.com/updates?id=563331)
Foundry NextGen에서 PII 샘플 Playground 미리보기 제공, 개인정보 검출 워크플로우 실증·평가가 효율화되었습니다.

### [Azure Monitor Logs mirroring into Microsoft Fabric (Preview)](https://azure.microsoft.com/updates?id=568322)
Azure Monitor 로그가 Microsoft Fabric OneLake에 실시간으로 미러링되어, ERP/CRM 등과 연계된 크로스 도메인 분석·AI 학습 지원이 강화되었습니다.

### [Protect sensitive generative AI telemetry in Application Insights and Microsoft Foundry (Preview)](https://azure.microsoft.com/updates?id=567594)
Application Insights 및 Foundry에서 민감한 AI 텔레메트리 보호 기능 강화, GenAIContent 테이블 별도 구축·액세스 제어로 규제 업종의 데이터 보안이 향상되었습니다.

---

## 🌏 신규 리전/한국 관련 업데이트

이번 달은 인도, 칠레 등 신흥 시장에서 Azure 신규 지역 기반 서비스 정식 지원이 돋보이며, 한국 리전 관련 특화 업데이트는 없었습니다.

### [Azure Database for PostgreSQL flexible server in India South Central](https://azure.microsoft.com/updates?id=568334)
인도 South Central 리전에서 PostgreSQL Flexible Server 배포가 가능해져, 데이터 지역성 및 서비스 다양성 반영이 개선되었습니다.

### [Microsoft Azure now available from new cloud region in India (India South Central)](https://azure.microsoft.com/updates?id=568013)
Hyderabad에 신규 인도 리전이 개설되며, AI 클라우드 인프라, 데이터 레지던시, 레이턴시 개선 등이 기업의 현지화 성공을 견인합니다.

### [Azure Red Hat OpenShift in Chile Central](https://azure.microsoft.com/updates?id=566732)
칠레 최초 Azure 리전에서 완전 관리형 OpenShift가 지원되어, 데이터 주권·규제 준수형 클라우드 확장에 최적화된 환경을 제공합니다.

---

## 총평 및 다음 달 전망

7월 Azure 업데이트는 글로벌 및 지역 클라우드 확장과 엔터프라이즈 AI 플랫폼의 고도화, 멀티클라우드 운영 효율화, 데이터 보호와 네트워크 경계 설정, 자동화 및 관리 정책의 안정성 강화가 핵심 트렌드로 보입니다. 정식 지원 기능이 늘고, 혁신 기술의 미리 보기(Preview)와 퇴출 정책 안내가 병행되어, 최신에 꼭 맞는 운영 환경 확장이 돋보였습니다.

다음 달에는 Azure 신규 리전, Foundry 통합 AI 통제, Fabric 기반 빅데이터 분석, 보안 및 컴플라이언스 특화 기술이 추가로 공개될 전망입니다. 멀티클라우드 및 온프레미스 연계, 행정 및 규제 업종의 데이터 보호 중심 신기술, 자동화 및 운영 효율화 기능에 대한 지속적 발전이 예상됩니다. Azure는 변동성과 혁신이 교차하는 클라우드 시장에서 글로벌 비즈니스의 새로운 성장 점을 꾸준히 제시할 것으로 기대됩니다.