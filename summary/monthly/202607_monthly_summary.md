# Azure 월간 업데이트 요약 - 2026년 07월

## 전반적인 트렌드와 핵심 인사이트

2026년 7월 Azure 업데이트는 AI와 자동화, 강화된 보안, 다중 클라우드 및 오픈 소스의 확대, 클라우드 네이티브 인프라의 세분화, 데이터 거버넌스와 관리 간소화, 그리고 개발자 경험을 향상시키는 기능들이 주요 트렌드를 이뤘다. AI 및 머신러닝은 Databricks와 Foundry, Azure AI Language와 같은 서비스에서 Claude Opus 5, Sonnet 5, GPT-5.6 지원 등 신규 모델의 기능 강화 및 엔터프라이즈 워크플로우 최적화를 통해 조직의 AI 활용 영역을 넓혔다.

컨테이너와 Kubernetes 중심의 업데이트는 게이트웨이 API 기반 인그레스 관리, Fleet Manager의 자동 리소스 배치, AKS 준비 이미지, AKS에서 파일 암호화 기능 등으로 클러스터 관리와 운영 자동화, 보안 강화, 그리고 더욱 유연한 스케일링 방식으로 진화하고 있다. 동시에 Site Recovery의 고속 처리를 지원, PowerShell/Python 최신 런타임 지원, Chaos Studio 시나리오 기반 테스트 등 운영 및 관리 효율을 높이는 서비스가 계속 등장했다.

스토리지 영역에선 클라이언트 측 데이터 무결성(BLOB Storage), SFTP 인증 및 ABAC 지원(Blob Storage), Google Cloud Storage에서 Azure로 마이그레이션 지원, NetApp Files의 SMB 구성을 포함해 플랫폼 및 네트워크 관점에서의 데이터 보호, 운영 효율성, 다중 클라우드 통합에 집중했다. 네트워킹에서는 NAT64, IPv6, Perimeter 기반 보안 정책, Front Door 엣지 액션 등 현대 인프라 환경의 네트워크 다양성과 보안 요구를 반영하는 기능 추가가 두드러졌다.

Microsoft Foundry와 Microsoft Fabric은 각각 AI 에이전트 개발의 효율성, 도구 통합, 민감 정보 관리, 그리고 Fabric 내 로그 데이터 통합 등으로 조직의 생산성과 데이터 활용을 크게 증대시켰다. 인도 남부의 신규 클라우드 리전 개설은 지역별 데이터 거버넌스, 로컬 성능 개선, AI·클라우드 수요 확대에 대응하는 Microsoft의 글로벌 전략의 일환이다.

전체적으로 이번 달 업데이트는 플랫폼의 보안, 신속한 대규모 배포, AI 통합, 하이브리드 환경의 확장과 복잡성 해소, 운영 자동화 그리고 데이터 분석 역량 강화라는 핵심 방향성을 명확하게 제시한다. 복잡한 멀티/하이브리드 클라우드, AI 기반 서비스 확산, 관리 효율 및 거버넌스 강화를 위한 Azure의 꾸준한 혁신이 이어지고 있다.

---

## 🖥️ 컴퓨트 & 컨테이너

7월에는 Azure Kubernetes Service(AKS)와 Fleet Manager에 여러 신규 기능이 출시되었으며, 운영 자동화와 인그레스 관리, 애플리케이션 보안이 크게 강화됐다. AKS의 Gateway API 기반 인그레스 관리 정식 지원, AKS에서 Azure Files NFS 암호화 전송, Fleet Manager 리소스 배치 및 실패 허용 기능 미리 보기 등은 대규모 환경에서의 관리 효율을 극대화한다. Azure Functions는 Python 3.14 지원과 PowerShell 7.6 미리 보기로 개발 언어 최신화와 호환성을 확대했다.

### [Application Routing with Gateway API](https://azure.microsoft.com/updates?id=567944)
AKS에서 게이트웨이 API로 인그레스 관리가 정식 지원되어 표준화된 라우팅 모델을 제공하며 서비스 메시 없이 경량화된 구성이 가능해졌다.

### [Resource placement in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567931)
리소스 배치를 통한 멀티 클러스터 관리가 용이해져 대규모 배포 시 일관성을 보장하고 운영 리스크를 낮춘다.

### [Azure Functions support for Python 3.14](https://azure.microsoft.com/updates?id=567646)
Python 3.14 지원으로 보안 및 호환성이 개선되며, 개발자들은 최신 툴과 장기간 지원을 활용할 수 있다.

### [Encryption in Transit for Azure Files NFS Shares in Azure Kubernetes Service (AKS)](https://azure.microsoft.com/updates?id=567787)
AKS 내 Azure Files NFS v4.1 데이터 전송이 TLS 기반 암호화로 보안과 컴플라이언스 요구를 충족한다.

### [Prepared Image Specification](https://azure.microsoft.com/updates?id=567949)
AKS 노드 이미지 사전 준비로 대규모, 고성능 워크로드의 신속한 스케일아웃과 운영 효율이 향상된다.

---

## 📊 AI & 머신러닝, 데이터 & 분석

Databricks와 AI Language, Microsoft Foundry를 중심으로 최신 AI 모델 통합, 데이터 분석 서비스 확장, 민감 정보 탐지 자동화 기능이 강화된다. 다양한 AI 모델(GPT-5.6, Claude Opus/Sonnet), PII 정보 검출 Playground, AI Gateway 미리보기 등 AI 워크로드의 실무 통합·관리 성능이 크게 향상된다.

### [Claude Opus 5 on Azure Databricks](https://azure.microsoft.com/updates?id=568316)
최신 Anthropic 모델 지원으로 고도화된 추론, 소프트웨어 개발, 전문가 업무용 AI 에이전트 구축이 가능해졌다.

### [Open AI GPT-5.6 on Azure Databricks](https://azure.microsoft.com/updates?id=567431)
AI 모델 서빙을 통한 GPT-5.6 도입으로 엔터프라이즈 데이터 기반 AI 활용성과 거버넌스가 강화된다.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)
PII 정보 자동 검출 서비스가 정식 지원되어 실무 적용 전 빠른 샘플 테스트와 비교 분석이 즉시 가능하다.

### [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)
Serverless SQL 창고 지원 확대로 즉각적 컴퓨트, 자동 확장, 인프라 관리 부담 감소를 제공한다.

### [AI Gateway in Azure API Management (미리보기)](https://azure.microsoft.com/updates?id=568184)
AI 모델·자산 노출 및 보안 일원화, 플랫폼 내 통합 정책 적용 등 AI 워크로드 관리 편의성을 높이고 있다.

---

## 🔒 네트워킹 & 보안

네트워크와 보안 부분에서는 NAT64, IPv6, DDoS 맞춤 정책, 네트워크 페리미터, Azure Enclave 등 다양한 네트워킹 옵션과 강화된 보안이 주도적인 변화다. Azure Firewall의 HTTP 헤더 삽입, VPN Gateway의 IPv6 지원도 기업 환경에서 보안·유연한 네트워크 설계를 돕는다.

### [NAT64 on StandardV2 NAT Gateway](https://azure.microsoft.com/updates?id=568409)
IPv6 워크로드와 IPv4 인터넷 목적지 사이 NAT64 변환 지원으로 차세대 네트워킹 환경이 강화된다.

### [IPv6 support for Azure VPN Gateway](https://azure.microsoft.com/updates?id=567847)
VPN Gateway에서 IPv6 기반 작업 지원이 확장되어 듀얼 스택 구성이 가능해지고 네트워크 통합성이 높아진다.

### [HTTP header insertion in Azure Firewall](https://azure.microsoft.com/updates?id=568115)
Azure Firewall에서 HTTP 요청 헤더 조작이 가능해져 보안·접근 관리 시나리오를 네이티브 방식으로 구현 가능하다.

### [Azure DDoS Protection custom policy (미리보기)](https://azure.microsoft.com/updates?id=568063)
DDoS 보호 정책을 리소스별 맞춤화할 수 있어 고유 트래픽 패턴을 가진 워크로드에도 효과적인 보안 제어가 가능하다.

### [Azure Enclave (미리보기)](https://azure.microsoft.com/updates?id=568377)
보안이 요구되는 워크로드용 격리 환경 관리·배포를 간소화하는 Azure Enclave로 정부 및 규제 산업에 최적화된다.

---

## 🗄️ 스토리지 & 데이터베이스

스토리지와 데이터베이스 영역에서는 Blob Storage와 Azure Files의 클라이언트 측 무결성 보호, SFTP 인증 방식, NetApp Files SMB 구성, PostgreSQL 관리 모듈 등의 기능이 대폭 확장되었다. 클라우드 간 마이그레이션 지원과 보안·컴플라이언스 향상 또한 주요 업데이트 축이다.

### [Client-side data integrity protections in Azure Blob Storage](https://azure.microsoft.com/updates?id=566895)
Blob Storage SDK에서 CRC64-NVME 검증 지원으로 애플리케이션에서부터 Azure 스토리지까지 엔드투엔드 데이터 무결성 보장이 가능하다.

### [Microsoft Entra ID-based access for Azure Blob Storage SFTP](https://azure.microsoft.com/updates?id=567085)
Entra ID 기반 SFTP 인증이 모든 리전에서 정식 지원되며, MFA/조건부 접근 정책 및 외부 협업이 더욱 간편해진다.

### [Azure Database for PostgreSQL flexible server in India South Central](https://azure.microsoft.com/updates?id=568334)
인도 남부 신규 리전에서 PostgreSQL flexible server 배포가 가능, 데이터 인프라의 지역 확장성이 크게 향상된다.

### [Public Preview: Azure Storage Mover now supports migration from Google Cloud Storage (GCS)](https://azure.microsoft.com/updates?id=566948)
GCS에서 Azure Blob Storage로 자동화된 데이터 마이그레이션이 지원되어 멀티 클라우드 통합이 효율화된다.

### [New Powershell module: Az.PostgreSQLFlexibleServer](https://azure.microsoft.com/updates?id=566209)
PostgreSQL 관리 통합 모듈이 Powershell에서 정식 지원, 자동화와 최신 플랫폼 기능 활용이 쉬워진다.

---

## ⚙️ 관리, 모니터링 & 운영 자동화

운영 자동화와 관리 영역에서는 최신 PowerShell 런타임 도입, Site Recovery의 고속 처리, Chaos Studio CLI/시나리오 미리 보기, Azure Automation 런타임 환경 개선 등 개발자와 운영자의 생산성 제고가 중심이다. 예약 정책 변경, 로그 내 AI 민감 정보 관리 등 정책 기반 거버넌스도 주요 변화다.

### [Azure Automation supports PowerShell 7.6 runbooks and Runtime environment](https://azure.microsoft.com/updates?id=568102)
PowerShell 7.6 및 런타임 환경 정식 지원으로 스크립트 최신화·보안 강화·버전별 자동 관리가 쉬워진다.

### [Support 5x churn in Azure Site Recovery](https://azure.microsoft.com/updates?id=566966)
Site Recovery의 5배 데이터 처리 속도 지원으로 대규모 고성능 워크로드에 안정적 재해 복구가 가능하다.

### [Azure Chaos Studio Workspaces and Scenarios (미리보기)](https://azure.microsoft.com/updates?id=567184)
애플리케이션 단위 장애 시나리오·워크스페이스 기반 테스트로 서비스 resiliency 검증이 가속화된다.

### [Azure Monitor Logs mirroring into Microsoft Fabric (미리보기)](https://azure.microsoft.com/updates?id=568322)
Azure Monitor 로그를 Fabric OneLake 연동으로 실시간 분석·비즈니스 데이터 통합이 지원된다.

### [Retirement: Support for Python-2.7; 3.8 and PowerShell-7.1; 7.2 will be retired on September 30, 2026](https://azure.microsoft.com/updates?id=567556)
오래된 Python/PowerShell 러untime 지원 종료 예정으로 업그레이드 필요성이 강조된다.

---

## 🌐 Microsoft Foundry & Microsoft Fabric

Foundry에서는 Toolboxes 정식 출시, PII 정보 탐지 Playground, 민감 AI 텔레메트리 보호 등 조직 내 AI 에이전트 개발·관리의 일원화와 효율성이 크게 높아지고 있다. Microsoft Fabric은 Azure Monitor 로그를 Fabric 레이크로 미러링하여 비즈니스·운영 데이터 통합 분석이 가능해진다.

### [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)
AI 에이전트 개발·운영을 위한 통합 툴박스 정식 도입으로 조직 내 도구 활용성과 거버넌스가 극대화된다.

### [Document PII playground sample in Microsoft Foundry NextGen (미리보기)](https://azure.microsoft.com/updates?id=563331)
PII 검출 Playground를 통해 빠른 샘플 테스트와 실무 적용 전 데이터 검증이 가능해졌다.

### [Protect sensitive generative AI telemetry in Application Insights and Microsoft Foundry (미리보기)](https://azure.microsoft.com/updates?id=567594)
AI 기반 민감 텔레메트리 데이터의 분리 관리·접근 제어가 강화, 개인정보와 컴플라이언스 요구에 대응한다.

### [Azure Monitor Logs mirroring into Microsoft Fabric (미리보기)](https://azure.microsoft.com/updates?id=568322)
Azure Monitor 로그를 Fabric OneLake으로 실시간 연동, AI 및 비즈니스 인사이트 분석이 가능하다.

### [AI Gateway in Azure API Management (미리보기)](https://azure.microsoft.com/updates?id=568184)
Foundry 등 AI 자산을 API 게이트웨이 일원화로 관리, 보안·거버넌스·운영 효율을 대폭 향상한다.

---

## 🇮🇳 지역 리전 확장

인도 남부 클라우드 리전 신규 개설, PostgreSQL flexible server 도입 등은 현지 데이터 거버넌스와 클라우드 기반 AI·DB 인프라 확장이 주요 변화다. 지역별 서비스 제공 지역의 다각화가 가속화된다.

### [Microsoft Azure now available from new cloud region in India (India South Central)](https://azure.microsoft.com/updates?id=568013)
인도 하이데라바드 신규 리전으로 현지 AI·클라우드 수요, 데이터 거버넌스, 레지던시·컴플라이언스 강화가 가능해졌다.

### [Azure Database for PostgreSQL flexible server in India South Central](https://azure.microsoft.com/updates?id=568334)
인도 남부 리전에서 PostgreSQL flexible server 배포가 가능해져 데이터 인프라의 지역 다변화가 확대된다.

---

## Azure 월간 총평 및 전망

2026년 7월 Azure 업데이트는 AI 통합, 자동화, 운영 효율, 보안·컴플라이언스, 멀티클라우드/하이브리드 확장 등 최신 클라우드 트렌드의 요구에 부응하는 혁신이 다양하게 이루어졌다. 특히 Databricks와 Foundry를 중심으로 AI 기반 워크플로우 강화, 네이티브 보안·네트워킹 옵션 확대, 클라우드 관리 자동화가 두드러진다. 인도 신규 리전 개설은 글로벌 데이터 레지던시와 로컬 서비스 제공 역량 확대를 상징한다.

다음 달에는 Python/PowerShell 구버전 지원 종료 사전 안내를 포함, 관리 정책 변화 및 서비스 API 전환, Fabric 내 데이터 분석 서비스 확대, AI 모델·클라우드 네이티브 기능의 미리 보기 기반 정식 출시 등이 예상된다. Azure는 복잡한 멀티클라우드 환경, 급속히 진화하는 AI 인프라, 글로벌 규제 준수와 함께 관리·보안 자동화에 더욱 집중할 전망이다.