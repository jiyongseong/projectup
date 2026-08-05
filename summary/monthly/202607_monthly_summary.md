# Azure 월간 업데이트 요약 - 2026년 07월

## 전반적인 트렌드와 핵심 인사이트

2026년 7월 Azure 업데이트는 AI 혁신, 보안강화, 관리 효율화, 네트워크 및 데이터센터 확장, 컨테이너와 멀티클라우드 최적화 등 다방면의 진보가 명확하게 드러납니다. 특히 AI 및 머신러닝 관련 기능의 대대적인 보강과 Microsoft Foundry‧Fabric의 엔터프라이즈 연동 기술 확대, Kubernetes 운용 환경의 현대화, 다양한 네트워크·스토리지 신기술 미리 보기 공개가 눈에 띕니다.

Azure Databricks, Azure AI Language, Azure Functions 등 주요 서비스에서 최근 AI 모델(GPT-5.6, Claude Sonnet 5, Claude Opus 5 등)을 기반으로 한 업무 자동화‧지능형 분석 기능이 강화되어 데이터 중심 기업들의 업무 효율성이 크게 향상될 것으로 전망됩니다. 이와 함께 Microsoft Foundry, Fabric 연동성 증강, Toolboxes와 Document PII Playground 등 AI 에이전트 및 데이터 거버넌스 도구의 정식 지원은 조직의 MLOps 및 데이터 보호 전략에 실질적인 가치와 신뢰성을 제공합니다.

보안 및 네트워크 부분에서는 Confidential Computing, Network Security Perimeter, Azure Enclave, DDoS Protection 커스텀 정책 등 데이터/트래픽 보호 기능의 대형 강화가 이루어졌습니다. 이는 점차 엄격해지는 산업별 규제와 클라우드 거버넌스 요구에 적극 대응하는 방향으로 보입니다. 또한 IPv6와 NAT64 등 차세대 네트워크 지원 확대는 미래 인프라 운영에 필수적인 기반을 제공하며, Azure Site Recovery, Chaos Studio 등 관리·재해복구 서비스의 발전은 클라우드 운용의 안정성과 신속성을 더욱 높이고 있습니다.

Kubernetes/컨테이너 영역에서는 Gateway API 기반 라우팅, Azure Kubernetes Fleet Manager 자원관리, AKS Prepared Image 등 운영 효율화를 목표로 한 기능이 다수 정식 지원 또는 미리 보기로 제공되어, DevOps 환경에서의 배포 자동화와 대규모 클러스터 관리가 대폭 향상됩니다. 그 외 Azure Storage, NetApp Files, Blob Storage 및 Azure Private Link, Azure Disk Storage 등 스토리지·네트워크 서비스도 관리성 및 보안성 증대로 대규모 기업용 운영 환경에 민첩성과 신뢰성을 주는 점이 두드러집니다.

지역별로는 인도 South Central 신규 데이터센터와 칠레 Central OpenShift 지원 등 글로벌 확장세가 지속되고 있으며, 각 업데이트마다 Azure의 엔터프라이즈 고객 맞춤 기술, 하이브리드 운용, 멀티클라우드 통합 지원 등의 방향성이 확실하게 자리 잡은 모습을 확인할 수 있습니다.

---

## 💡 AI 및 머신러닝

이번 달 AI 및 머신러닝 분야는 최신 AI 모델 도입, 데이터 분석 및 자동화 기능 강화, 실시간 에이전트 및 도구화가 두드러집니다. Databricks를 중심으로 GPT-5.6, Claude Sonnet 5, Claude Opus 5 등 선진 모델이 통합되어 AI 활성화가 가속화되며, Microsoft Foundry의 Toolboxes와 PII Playground 제공은 조직 내 AI 도구의 신뢰성과 생산성을 대폭 향상시킵니다.

#### [Claude Opus 5 on Azure Databricks](https://azure.microsoft.com/updates?id=568316)
Azure Databricks에서 Anthropic Claude Opus 5 적용. 고급 추론과 전문가 수준의 업무, 장기 플래닝, 코딩 보조 등 AI 활용 폭 확대.

#### [Open AI GPT-5.6 on Azure Databricks](https://azure.microsoft.com/updates?id=567431)
Microsoft Foundry에서 구매한 GPT-5.6 모델을 Databricks에 연동, 기업 데이터 기반으로 안전하고 통합된 AI 서비스 구축 가능.

#### [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)
Databricks SQL Serverless가 UK West에 정식 지원되어 실시간 분석과 자동 확장, 인프라 관리 최소화가 가능해짐.

#### [Generally available: Anthropic Claude Sonnet 5 on Azure Databricks](https://azure.microsoft.com/updates?id=567194)
클라우드 AI 모델 성공적 통합, 적응형 사고와 대규모 엔터프라이즈 AI 자동화 지원.

#### [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)
Foundry Toolboxes 정식 지원, 에이전트/도구의 일관된 거버넌스와 재사용성 확보.

---

## 🚀 컨테이너 및 Kubernetes

컨테이너 환경은 Gateway API 표준 도입, 자원 관리 자동화, 이미지 준비 등 현대화가 중심입니다. AKS 라우팅 현대화, Fleet Manager 자원 분배, 업데이트 내 실패 내성 지원이 더해져 클러스터 관리의 유연성·효율성이 더욱 향상됐습니다.

#### [Application Routing with Gateway API](https://azure.microsoft.com/updates?id=567944)
AKS에서 Kubernetes Gateway API 기반의 인그레스 라우팅 정식 지원. 기존 nginx 방식에서 표준화된 네트워크 관리로 유연한 전환 가능.

#### [Resource placement in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567931)
Fleet Manager에서 Kubernetes 자원 배치 자동화, 여러 클러스터로 자원 배포 및 운영 간소화.

#### [Azure Functions support for Python 3.14](https://azure.microsoft.com/updates?id=567646)
Azure Functions에서 Python 3.14 지원, 보안 및 장기 지원 기반 앱 개발 가능.

#### [Public Preview: Azure Functions Support for PowerShell 7.6](https://azure.microsoft.com/updates?id=567651)
PowerShell 7.6 미리 보기 지원, 최신 스크립트 환경에서 Functions 배포 효율화.

#### [Maximum allowed failures for update runs in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567939)
Fleet Manager 업데이트 실패 허용치 설정 미리 보기, 대규모 클러스터 업데이트의 유연성과 회복력 보장.

---

## 🏢 데이터베이스 및 분석

데이터베이스와 분석 서비스는 PostgreSQL 및 Databricks 관련 신기술 확대, 데이터 보호 및 관리성 강화가 특징입니다. PowerShell 모듈 갱신, Defender 평가 지원 등 예방적 보안 및 운영 효율성 확대가 이뤄지고 있습니다.

#### [Azure Database for PostgreSQL flexible server in India South Central](https://azure.microsoft.com/updates?id=568334)
인도 South Central에서 PostgreSQL flexible server 정식 지원, 지역 분산 및 데이터 주권 강화.

#### [New Powershell module:  Az.PostgreSQLFlexibleServer](https://azure.microsoft.com/updates?id=566209)
새 PowerShell 모듈로 PostgreSQL 18, 탄력적 클러스터, 운영 효율성 향상 지원.

#### [Microsoft Defender security assessments for Azure Database for PostgreSQL Flexible Server](https://azure.microsoft.com/updates?id=567527)
Defender CSPM 평가 정식 지원, 지속적 보안 상태 평가 및 취약점 조치 자동화.

#### [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)
Databricks SQL Serverless 영국 서부 지역 지원, 분석기능과 자동 확장 구현.

#### [Claude Opus 5 on Azure Databricks](https://azure.microsoft.com/updates?id=568316)
Databricks 내 AI 모델 서빙 강화, 고급 분석 및 코드 자동화 가능.

---

## ⚙️ 관리 및 거버넌스

클라우드 관리·거버넌스 영역에서 PowerShell/Runbook 신기능, Chaos Studio 시나리오, Site Recovery 고성능, 예약 정책 등 관리 효율성과 보안 준수 기능이 지속적으로 도입되고 있습니다.

#### [Azure Automation supports PowerShell 7.6 runbooks and Runtime environment](https://azure.microsoft.com/updates?id=568102)
Automation에서 PowerShell 7.6 런북과 실행환경 정식 지원, 스크립트 보안‧이식성‧관리성 강화.

#### [Support 5x churn in Azure Site Recovery](https://azure.microsoft.com/updates?id=566966)
Site Recovery의 고성능 지원 확대(최대 500MB/s), 고IOPS 재해복구 • 데이터집약 시스템 보호능력 향상.

#### [Support for Python-2.7; 3.8 and PowerShell- 7.1; 7.2 will be retired on September 30, 2026](https://azure.microsoft.com/updates?id=567556)
Python 2.7/3.8, PowerShell 7.1/7.2 지원 종료 예정, 최신 버전으로 마이그레이션 필수.

#### [Azure Chaos Studio Workspaces and Scenarios](https://azure.microsoft.com/updates?id=567184)
Chaos Studio Workspaces‧Scenarios 미리 보기, 실제 장애패턴 시뮬레이션 및 애플리케이션 복원력 평가 간소화.

#### [Manage Azure Chaos Studio from the Azure CLI](https://azure.microsoft.com/updates?id=567225)
CLI로 Chaos Studio 자동화, 시나리오 실행 및 운영 효율 최적화.

---

## 🔒 보안 및 네트워크

보안 및 네트워크 영역은 Confidential Computing, Entra ID, NAT64, IPv6, DDoS Protection, 네트워크 경계 등 다양한 서비스에서 미리 보기 포함 정식 지원이 활발히 이루어졌습니다. 서비스별 세분화된 접근제어, 트래픽 보호, 다중 인증 등 신뢰성 강화가 두드러졌습니다.

#### [Confidential Computing support for Azure Event Hubs Dedicated](https://azure.microsoft.com/updates?id=567212)
Event Hubs Dedicated에서 Confidential Computing 지원, 데이터/이벤트 스트리밍 실시간 암호화 및 보호 강화.

#### [Microsoft Entra ID-based access for Azure Blob Storage SFTP](https://azure.microsoft.com/updates?id=567085)
Blob Storage SFTP에 Entra ID 및 외부 ID 연동, 운영 부담 없이 강력한 인증/보안 지원.

#### [Client-side data integrity protections in Azure Blob Storage](https://azure.microsoft.com/updates?id=566895)
Blob Storage용 SDK에 CRC64-NVME 통합, 클라이언트-스토리지 간 데이터 무결성 검증 강화.

#### [Network Security Perimeter support for Azure Event Hubs](https://azure.microsoft.com/updates?id=567203)
Event Hubs 네트워크 경계 지원, PaaS 리소스의 중앙 통제 및 데이터 유출 위험 감소.

#### [IPv6 support for Azure VPN Gateway](https://azure.microsoft.com/updates?id=567847)
VPN Gateway IPv6 지원, 듀얼스택 인프라 및 글로벌 확장에 대응하는 보안 연결 실현.

---

## 🗄️ 스토리지 및 인프라

스토리지 / 인프라 영역에서는 파일 암호화, SFTP 인증, Storage Mover, Azure Disk Storage 등 데이터 이동·보안·유지관리 측면에서 신기술이 미리 보기 포함 정식 지원됩니다. 네트워크 경계, NAT64, NetApp Files 등 대규모 이관‧통합 편의성이 강조됩니다.

#### [Encryption in Transit for Azure Files NFS Shares in Azure Kubernetes Service (AKS)](https://azure.microsoft.com/updates?id=567787)
AKS에서 Azure Files NFS 암호화 정식 지원(TLS), 클라우드-컨테이너 보안 및 준수역량 향상.

#### [Public Preview: Azure Storage Mover now supports migration from Google Cloud Storage (GCS)](https://azure.microsoft.com/updates?id=566948)
Storage Mover에서 GCS → Azure Blob Storage 이관 미리 보기, 완전한 관리형 경험 및 멀티클라우드 통합 지원.

#### [Symmetric keys on Azure Key Vault Premium](https://azure.microsoft.com/updates?id=566746)
Key Vault Premium에서 대칭키 적용 미리 보기, AES 256 기반 암호화와 중앙 관리 지원.

#### [NAT64 on StandardV2 NAT Gateway](https://azure.microsoft.com/updates?id=568409)
NAT Gateway에서 NAT64 지원, IPv6 ↔ IPv4 통신 전환 자동화.

#### [Support for SMB Opportunistic Locking (Oplocks) configuration](https://azure.microsoft.com/updates?id=568396)
NetApp Files의 SMB Oplocks 설정 지원, 캐싱 최적화 및 크로스 리전 복제 운용성 강화.

---

## 🧩 Microsoft Foundry 및 Microsoft Fabric

Microsoft Foundry와 Fabric은 엔터프라이즈 AI 에이전트, 데이터 거버넌스, 새로운 도구 체계 확대가 핵심으로, AI 도구의 재사용성·OneLake 기반 데이터 활용성·PII 보호 등 조직 내 데이터 혁신의 기틀을 마련합니다.

#### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)
Document PII Playground 정식 지원, 엔터프라이즈 개인정보 식별·평가 경험 강화.

#### [Public Preview: Document PII playground sample in Microsoft Foundry NextGen](https://azure.microsoft.com/updates?id=563331)
Foundry NextGen 포털 내 PII 샘플 Playground 미리 보기, 개인정보 탐지·redaction 체험 제공.

#### [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)
Foundry Toolboxes 정식 지원, 일관된 툴 거버넌스와 재사용, 운영자·개발자 경험 최적화.

#### [Protect sensitive generative AI telemetry in Application Insights and Microsoft Foundry](https://azure.microsoft.com/updates?id=567594)
Application Insights와 Foundry에서 민감 AI 텔레메트리 보호 강화, 제한적 접근·데이터 거버넌스 구현.

#### [Azure Monitor Logs mirroring into Microsoft Fabric](https://azure.microsoft.com/updates?id=568322)
Monitor Log Analytics 워크스페이스 telemetry를 Fabric OneLake에 실시간 동기화 지원, 비즈니스·운영 데이터 결합 분석 가능.

---

## 🌏 지역별 확장 및 인프라

글로벌 데이터센터 확장, 신규 인프라 지역 배포, OpenShift 클라우드 네이티브 환경 증대가 눈에 띄는 한 달입니다. 인도 South Central 및 칠레 Central 등 신흥 시장에서 Azure 서비스의 기반 확충이 이루어져 글로벌 고객의 데이터 요구 및 레이턴시 개선이 주목됩니다.

#### [Microsoft Azure now available from new cloud region in India (India South Central)](https://azure.microsoft.com/updates?id=568013)
인도 Hyderabad 지역 신규 데이터센터 개설, AI 인프라‧데이터 주권‧성능 개선 실현.

#### [Azure Database for PostgreSQL flexible server in India South Central](https://azure.microsoft.com/updates?id=568334)
인도 South Central에 PostgreSQL flexible server 지원, Data residency 및 혁신적 클라우드 환경 마련.

#### [Azure Red Hat OpenShift in Chile Central](https://azure.microsoft.com/updates?id=566732)
칠레 Central에서 OpenShift(Azure Red Hat) 정식 지원, 남미 시장의 클라우드 기반 AI‧데이터 혁신.

#### [Network Security Perimeter support for Azure Event Hubs](https://azure.microsoft.com/updates?id=567203)
지역별 Event Hubs 자원에 경계 기반 보호 도입, 데이터 주권과 네트워크 통제력 제고.

#### [Azure Blob Storage client-side integrity in Korea Central/Korea South](
https://azure.microsoft.com/updates?id=566895)
담당 지역 관련 SDK 업데이트가 없으나, 모든 지역에서 일괄 지원됨을 확인.

---

## 총평과 다음 달 전망

2026년 7월 Azure 업데이트는 AI와 데이터, 보안, 네트워크, 관리 효율화에 집중하며 조직의 클라우드 혁신 속도와 신뢰성을 크게 높이는 결과를 보여줍니다. 정식 지원, 미리 보기, 안내 공지가 고르게 이어지는 이번 달은 실질적인 엔터프라이즈 서비스 고도화와 미래형 업무환경을 구축하는 데 초점을 맞추고 있습니다.

다음 달에는 AI 모델 성능 및 확장성 개선, 지역별 신규 서비스 출시, Kubernetes 및 컨테이너 운용 첨단 기능의 미리 보기 정식 전환, 스토리지 데이터 보호 강화 등 조직의 AI 비즈니스와 안전 운영을 위한 신기술의 지속적 업데이트가 기대됩니다. Azure는 앞으로도 다방면의 클라우드 혁신을 선도하며, 글로벌 환경 대응 및 고객 맞춤 기능 진화를 계속 추진할 전망입니다.