# Azure 월간 업데이트 요약 - 2026년 07월

## 전반적인 트렌드와 핵심 인사이트

2026년 7월의 Azure 업데이트는 하이브리드 환경과 멀티클라우드 전략의 강화, AI 및 머신러닝 플랫폼 진화, 인프라 자동화 및 보안 강화에 중점을 두었습니다. 특히 전 세계적으로 AKS, Azure Databricks, PostgreSQL 등 주요 리소스의 서비스 영역이 확대되고 있으며, 인도와 칠레 신규 리전 오픈 등 글로벌 확산 전략이 두드러졌습니다. AI 모델 서빙 및 데이터 분석 기능은 더욱 고도화되어 Anthropic Claude Opus 5, GPT-5.6 등 최신 모델들이 Azure Databricks와 Microsoft Foundry에서 정식 지원, 미리보기 형태로 확장되고 있습니다. 플랫폼 표준화와 자동화 측면에서는 PowerShell 7.6, Python 3.14 등 최신 런타임 지원과 Azure Automation·Functions의 쉬운 마이그레이션, AKS의 Kubernetes Gateway API 도입 등 현업에서의 전환을 원활하게 지원하는 기능이 다양하게 추가되었습니다.

보안 측면에서는 데이터 무결성, 네트워크 격리, Confidential Computing, 네트워크 경계 기반 보호(Perimeter), 엔드포인트 암호화, Entra ID 기반 인증 등 여러 계층의 보안 기능이 더 강화되었습니다. Storage 및 Migration 영역에서는 Google Cloud Storage와 Azure 간 이관, Blob Storage SFTP 및 Azure Files NFS의 암호화 기능 도입으로, 타 클라우드와의 연결 및 데이터 보호가 한층 용이하게 되었습니다.

또한 Microsoft Foundry, Microsoft Fabric 등 새로운 데이터·AI 플랫폼에 대한 연동 및 확장 소식이 보여지며, 조직 내 AI 활용과 데이터 거버넌스, 자동화·관측성 향상을 위한 다양한 기능이 미리 보기로 출시되며 본격적인 기업용 서비스 통합이 진행중임을 알 수 있습니다. 마지막으로 보안 및 운영 지원 종료(Deprecated) 안내와 미리보기 기능 추가 등 지속적인 플랫폼 생태계 관리와 개선이 이뤄지고 있습니다.

이달의 핵심 인사이트로는:
- 최신 플랫폼 및 런타임 표준의 신속한 도입 및 자동화 지원
- AI 모델 서빙 및 데이터 분석 기능 확장의 급속한 진화
- 글로벌 리전 확대를 통한 데이터 레지던시, 현지 규제 대응
- 멀티클라우드 데이터 이동성·보안·거버넌스 강화
- 미리 보기 신기능과 엔터프라이즈 중심의 자동화/관측성 도구 확대

## 🖥️ 컴퓨트, 컨테이너, 서버리스

이달 컴퓨트와 컨테이너 서비스의 주요 동향은 최신 개발환경 표준화, 클러스터 자동화, 대규모 관리 효율성 강화에 집중되었습니다. AKS에서는 Gateway API 기반 애플리케이션 라우팅 정식 지원이 시작되어 네이티브 인그레스 관리가 더욱 현대적이고 표준화된 방식으로 구현이 가능해졌습니다. Azure Functions는 Python 3.14와 PowerShell 7.6을 공식 지원하며 개발자들이 최신 런타임 환경을 쉽게 활용할 수 있게 되었습니다. Azure Kubernetes Fleet Manager에서는 리소스 배치와 실패 허용 업데이트 미리 보기 등 멀티클러스터 관리 자동화 기능이 확대되고 있습니다.

### [Application Routing with Gateway API 정식 지원](https://azure.microsoft.com/updates?id=567944)
AKS에서 Gateway API를 이용한 애플리케이션 라우팅 정식 지원으로, Kubernetes 기반 인그레스 관리가 더 표준화되고 서비스 메시가 없어도 경량 구성으로 현대화 전환을 지원합니다.

### [Azure Automation PowerShell 7.6 런북 및 런타임 환경 정식 지원](https://azure.microsoft.com/updates?id=568102)
최신 PowerShell 7.6을 활용한 Azure Automation 런북 관리가 가능해져 스크립트 이관과 실행 환경 관리가 대폭 간소화되었습니다.

### [Azure Functions Python 3.14 지원 정식 시작](https://azure.microsoft.com/updates?id=567646)
Python 3.14를 통한 함수 개발 및 배포 가능, 보안·성능과 지원 기간이 개선된 환경에서 운영할 수 있습니다.

### [Azure Kubernetes Fleet Manager 리소스 배치 정식 지원](https://azure.microsoft.com/updates?id=567931)
플랫폼·애플리케이션 팀이 Kubernetes 자원을 멀티 클러스터에 효과적으로 배포·관리할 수 있는 기능이 제공됩니다.

### [Azure Kubernetes Fleet Manager 업데이트 실패 허용 미리 보기](https://azure.microsoft.com/updates?id=567939)
업데이트 진행시 일정 수의 실패를 허용할 수 있게 되어 롤아웃의 유연성 및 대규모 클러스터 관리 효율성이 크게 강화됩니다.

## ☁️ 데이터, 분석, AI & 머신러닝

데이터 및 AI 영역에서는 Azure Databricks에서 Claude Opus 5, GPT-5.6, Claude Sonnet 5 등 최신 AI 모델 서빙이 정식 지원 시작과 함께, SQL Serverless, 다양한 데이터베이스 확장, PII 탐지 Playground 등 데이터 분석 및 실무 활용성이 크게 제고되었습니다. AI Gateway와 Microsoft Fabric 연동 등 엔터프라이즈 AI 플랫폼 통합을 지원하는 미리보기 기능도 새롭게 등장했습니다.

### [Claude Opus 5 on Azure Databricks 정식 지원](https://azure.microsoft.com/updates?id=568316)
Anthropic의 최신 AI 모델(Claude Opus 5)을 Databricks에서 활용 가능, 복잡한 추론·코딩·에이전트 워크플로우 지원.

### [Open AI GPT-5.6 on Azure Databricks 정식 지원](https://azure.microsoft.com/updates?id=567431)
Foundry와 Databricks 통합 모델 서빙, Unity AI Gateway 기반 거버넌스가 적용된 엔터프라이즈 AI 환경.

### [Azure Databricks SQL Serverless UK West 출시](https://azure.microsoft.com/updates?id=567444)
UK West 리전에서 Serverless SQL 웨어하우스 기본화, 즉시 컴퓨트 및 자동 확장으로 관리 편의성 증대.

### [Azure AI Language Document PII NextGen Playground 정식 지원](https://azure.microsoft.com/updates?id=564382)
신분 식별정보(PII) 탐지 Playground에서 빠른 평가·샘플 제공, 데이터 컴플라이언스 실무 지원.

### [Azure Event Hubs Dedicated Confidential Computing 지원](https://azure.microsoft.com/updates?id=567212)
Confidential Computing 기반 이벤트 스트리밍 데이터 보호 정식화, 민감한 데이터 메모리 내 보호력 증대.

## 🗃️ 스토리지, 네트워크, 보안

스토리지 분야에서는 Blob Storage/SFTP에 Entra ID 인증과 클라이언트 데이터 무결성(End-to-End CRC64-NVME), Files NFS v4.1 전송 암호화(EiT), Storage Mover의 GCS 지원 등 멀티클라우드 이동 및 보안이 강화되었습니다. 네트워크 측면에서는 NAT64, VPN Gateway IPv6, 네트워크 경계(Perimeter), Azure Firewall HTTP 헤더 삽입 등 최신 프로토콜·보안·유연성을 제공하는 기능 추가가 눈에 띕니다.

### [Azure Blob Storage 클라이언트 데이터 무결성 보호 정식 지원](https://azure.microsoft.com/updates?id=566895)
.NET, C++, JavaScript SDK에서 CRC64-NVME로 데이터 일관성 보장, 실질적 앱-스토리지 보안 강화.

### [Encryption in Transit for Azure Files NFS Shares in AKS 정식 지원](https://azure.microsoft.com/updates?id=567787)
AKS 워크로드와 Azure Files NFS 연결시 전송중 암호화(TLS)로 준수 규제 요건 충족과 데이터 보호.

### [Azure Storage Mover GCS 마이그레이션 미리 보기](https://azure.microsoft.com/updates?id=566948)
Google Cloud Storage에서 Azure로 데이터 무단계 대규모 이동 지원, Private Link와 연동하여 보안 강화.

### [IPv6 지원 Azure VPN Gateway 정식 시작](https://azure.microsoft.com/updates?id=567847)
IPv6 듀얼스택 트래픽 지원, Site-to-Site 및 Point-to-Site 환경에서 IPv6 연결 확대.

### [HTTP 헤더 삽입 Azure Firewall 정식 지원](https://azure.microsoft.com/updates?id=568115)
내부 규제·보안위한 헤더 추가/수정 가능, 개별 앱 접근 정책·인증 시나리오 지원.

## 🔗 마이그레이션, 자동화 및 관리

이달에는 Automation 및 Site Recovery의 최신 런타임·마이그레이션 기능 정식 지원, Storage Mover Google Cloud 지원 미리 보기, PowerShell 모듈 현대화 등 자동화 및 관리 효율화 기능이 출시되었습니다. Site Recovery의 초고속 Churn 지원으로 데이터베이스와 대규모 워크로드도 신속하게 복구가 가능해졌으며, 런타임 지원 종료 안내 등 지속적인 플랫폼 안정성 관리가 진행되고 있습니다.

### [Azure Automation PowerShell 7.6 및 런타임 환경 정식 지원](https://azure.microsoft.com/updates?id=568102)
구 버전 Runbook를 최신 환경으로 빠르게 업그레이드, CLI 커맨드 지원 등 코드 편의성 증대.

### [Azure Site Recovery 5배 Churn 지원 시작](https://azure.microsoft.com/updates?id=566966)
고성능 IOPS 워크로드까지 안정적으로 재해 복구 가능, 대용량 데이터베이스·분석 시스템 지원 확대.

### [Az.PostgreSQLFlexibleServer PowerShell 모듈 신규 출시](https://azure.microsoft.com/updates?id=566209)
PostgreSQL 18, 엘라스틱 클러스터 등 최신 기능, 빠른 환경 구성·관리 효율 증가.

### [런타임 지원 종료 안내: Python 2.7, 3.8, PowerShell 7.1/7.2](https://azure.microsoft.com/updates?id=567556)
2026년 9월 30일부터 공식 지원 종료, Runbook 최신화 필요성 강조.

### [Azure Storage Mover GCS 마이그레이션 미리 보기](https://azure.microsoft.com/updates?id=566948)
클라우드 간 통합 및 대규모 데이터 이동성 실질적 개선, 보안 네트워크 경로 지원.

## 🗺️ 글로벌 리전 및 현지화

Azure의 글로벌 확장 및 현지 운영 지원이 강화되었습니다. 인도 South Central 신규 리전 개설, 칠레 Central 리전에서 ARO(OpenShift) 정식 지원, Azure Database for PostgreSQL 인도 리전 지원 등 지역별 데이터 레지던시와 현지 업무 환경에 적합한 인프라가 확대되었습니다.

### [Microsoft Azure 인도 South Central 신규 리전 개설](https://azure.microsoft.com/updates?id=568013)
현지 AI 준비·보안·데이터 레지던시·지속가능한 클라우드 인프라 제공 시작.

### [Azure Database for PostgreSQL flexible server 인도 South Central 정식 지원](https://azure.microsoft.com/updates?id=568334)
인도 신규 리전에서 PostgreSQL 데이터베이스 구축 가능, 로컬 규제·속도·비용 최적화.

### [Azure Red Hat OpenShift 칠레 Central 정식 지원](https://azure.microsoft.com/updates?id=566732)
칠레 최초 Azure 리전에서 완전관리 OpenShift 클러스터 제공, 현지 데이터 및 규제 대응.

### [UK West region Azure Databricks SQL Serverless 출시](https://azure.microsoft.com/updates?id=567444)
영국 고도화된 데이터 분석 인프라 현지화, 즉시 컴퓨트 및 저비용 확장 지원.

### [Azure Storage Mover Google Cloud Storage 지역간 마이그레이션 지원](https://azure.microsoft.com/updates?id=566948)
다국적 기업의 멀티클라우드 전략·데이터 이관 실효성 증대.

## 🧰 Microsoft Foundry

Microsoft Foundry 영역에서는 PII 탐지 Playground와 Toolboxes 정식 지원, 문서 기반 PII 탐지 미리보기 등 조직 내 AI 솔루션 표준화, 단일화된 에이전트/툴 관리, 실무용 데이터 거버넌스 실현이 돋보입니다.

### [Document PII NextGen Playground 정식 지원](https://azure.microsoft.com/updates?id=564382)
PII 탐지 워크플로우의 신속한 적용·평가, 데이터 컴플라이언스 프로세스 단축.

### [Toolboxes 정식 지원](https://azure.microsoft.com/updates?id=563481)
조직 내 에이전트 간 도구 공유·거버넌스·통합 관리 지원, MCP 기반 단일 엔드포인트로 표준화.

### [Document PII Playground sample 미리 보기](https://azure.microsoft.com/updates?id=563331)
문서 기반 PII 탐지 API/플레이그라운드 첫 경험, 샘플 문서 내 실시간 평가 제공.

### [AI Gateway Azure API Management 연결 미리 보기](https://azure.microsoft.com/updates?id=568184)
Foundry 등 모델·툴 안전하게 외부에 노출, 일관된 인증·정책·관측성 확보.

### [GenAI Application Insights/Foundry 민감 데이터 보호 미리 보기](https://azure.microsoft.com/updates?id=567594)
GenAI 콘텐츠 접속 권한 추가, 의료·금융 등 컴플라이언스 요구 높은 산업에 적합.

## 🧪 Microsoft Fabric

Microsoft Fabric 영역은 Azure Monitor 로그 미러링 등 실시간 관측성 데이터를 원레이크(OneLake) 구조로 연동, AI 및 비즈니스 데이터와 통합 분석 기능을 미리 보기로 제공하며 통합 플랫폼의 실질적 진화가 본격화되고 있습니다.

### [Azure Monitor Logs Microsoft Fabric 미러링 미리 보기](https://azure.microsoft.com/updates?id=568322)
Azure 관측성 로그를 OneLake로 실시간 연동, 데이터 중복 없이 데이터 분석·AI 모델링과 연계 가능.

### [Document PII Playground sample Microsoft Foundry NextGen 미리 보기](https://azure.microsoft.com/updates?id=563331)
Fabric NextGen와 Foundry 활용 시 PII 탐지 워크플로우 기반 통합 데이터 거버넌스 제공.

### [Power BI, Eventhouse, Spark 분석 통합](https://azure.microsoft.com/updates?id=568322)
실시간 관측성과 비즈니스 데이터 통합 분석, 중복 없는 연계 환경 구현.

### [대규모 원레이크 기반 크로스도메인 분석 지원](https://azure.microsoft.com/updates?id=568322)
ERP, CRM, 비즈니스 이벤트 연동, AI·머신러닝·장기 트렌드 분석 가능.

### [데이터 Table별 관리, 민감정보 접근 제어 미리 보기](https://azure.microsoft.com/updates?id=567594)
Log Analytics 기반 테이블별 보안 정책(Foundry 연계) 실현.

## 🎯 기타 주요 미리 보기/공지/지원 종료

2026년 7월 업데이트는 플랫폼 미리 보기, 신기능 공지, 리소스 및 정책 지원 종료 안내가 포함되어 있어 관리 효율성 및 서비스 무중단 혁신의 방향성을 제공합니다.

### [Azure DDoS Protection Custom Policy 미리 보기](https://azure.microsoft.com/updates?id=568063)
트래픽 종류별 맞춤 차단 임계값 지정, 게임/이벤트/대규모 워크로드 최적화.

### [Azure Enclave 미리 보기](https://azure.microsoft.com/updates?id=568377)
정부·규제 산업에 특화된 네트워크 분리 및 보안, Managed Infrastructure기반 빠른 격리 환경 제공.

### [Azure Front Door Edge Actions 미리 보기](https://azure.microsoft.com/updates?id=567402)
서버리스 자바스크립트 실행으로 실시간 트래픽 제어, 성능·보안·관리 유연성 대폭 향상.

### [인스턴트 VM Restore Point 미리 보기](https://azure.microsoft.com/updates?id=565758)
빠른 앱 일관성 복구 및 즉시 디스크 사용 가능, RTO 단축 및 복구정책 유연성 증대.

### [Azure 서비스 Reservation 교환 정책 변경 공지](https://azure.microsoft.com/updates?id=568514)
2027년 2월 1일부터 Savings Plan 지원 서비스에서는 더 이상 Reservation 교환 불가, 기존 예약 건의 경우 최종 1회 교환 허용.

---

## 총평 및 8월 전망

7월의 Azure 업데이트는 최신 개발 환경으로의 빠른 전환, 글로벌 리전 영토 확장, AI·데이터 기반 실무 혁신과 엔터프라이즈 보안 강화가 도드라졌습니다. 특히 Foundry, Fabric 등 차세대 데이터/AI 플랫폼 미리 보기가 다수 추가됨으로써 기존 Azure PaaS와의 유연한 연결, 조직 전체에서의 AI 활용 효율화가 급진적으로 진행될 것으로 예상됩니다. 글로벌 신규 리전 오픈과 멀티클라우드 데이터 이동성 강화는 지역별 규제·디지털 전환의 요구를 충족시키며, 보안/컴플라이언스 기능의 확장은 서비스 신뢰성 확보에 기여하고 있습니다.

다음 달에는 신규 미리 보기 기능의 정식 지원 전환, Fabric/Foundry의 확장 및 현지화, AI 모델 및 데이터 거버넌스 혁신이 더욱 본격화될 전망이며, 플랫폼 안정성 및 자동화 도구의 추가 개선과 엔터프라이즈 통합 생태계 확장에 주목할 필요가 있습니다. 업계는 데이터와 AI 기반 실무, 보안 내재화, 자동화 효율성 등 세가지 트렌드에 집중하며, Azure는 지속적인 개방성·혁신을 통해 시장 리더십을 강화하고 있습니다.