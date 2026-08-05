# Azure 월간 업데이트 요약 - 2026년 07월

## 전반적인 트렌드와 핵심 인사이트

2026년 7월 Azure 업데이트는 AI와 자동화, 데이터 거버넌스, 보안 강화, 클라우드 네이티브 및 하이브리드 환경의 진화, 글로벌 지역 확장, 개발자 및 운영 효율성 증대가 두드러진 한 달이었습니다. 특히 Azure Databricks, AI 모델 서빙, Microsoft Foundry와 Fabric 연동 등 인공지능 및 데이터 분석 플랫폼의 기능 확장과 성능 개선이 집중적으로 이루어졌습니다. Anthropic Claude 시리즈와 OpenAI GPT-5.6 등 최신 AI 모델이 정식 지원되면서, 기업들은 고도화된 자연어 처리와 업무 자동화에 한층 가까워졌으며, 복합 데이터 워크플로우 및 장기 추세 분석에 대한 니즈도 커지고 있습니다.

보안 측면에서는 Confidential Computing, Azure Firewall의 HTTP 헤더 삽입 및 네트워크 보안 경계 기능, SFTP의 Entra ID 연동 등 데이터 전송 및 저장, 네트워크 경계의 보호 강화가 강조됐습니다. Azure Chaos Studio, DDoS Protection 등 운영 안정성 및 복원력 검증을 위한 기능도 확대되었습니다. 또한 PowerShell 7.6 및 Python 3.14 지원, 자동 스크립트 관리, VM Restore Points의 Instant Access 도입 등으로 하이브리드·멀티클라우드, 자동화 환경의 효율성과 개발 생산성이 상승하고 있습니다.

글로벌 지역 확장에 따라 인도/칠레/영국 등 신규 데이터센터 및 서비스 지역 배포로 현지화와 서비스 가용성 향상, 운용의 지리적 다양성도 주목할 만합니다. 마지막으로 Microsoft Foundry, Fabric, AKS Fleet, API Gateway 등 플랫폼 통합 및 클라우드 네이티브 관련 신기술이 정식 지원 또는 미리 보기로 출시되어, 기업의 IT 거버넌스 및 개발 효율성 증대를 지원하고 있습니다.

아래는 더욱 세부적인 카테고리별 요약과 주요 업데이트 내용입니다.

---

## 🖥️ 컴퓨트 & 컨테이너

이번 달 컴퓨트 및 컨테이너 분야는 AKS Gateway API, Azure Functions의 Python 3.14, PowerShell 7.6, Azure Kubernetes Fleet Manager 기능 등 현대적 클라우드 인프라 관리와 개발자 생산성, 자동화 편의성이 강화되었습니다.

- AKS에서 Gateway API 기반 애플리케이션 라우팅이 정식 지원되어, 서비스 메시 없이 최신 Kubernetes 표준 기반 인그레스 관리를 할 수 있게 됐습니다.
- Azure Functions는 Python 3.14 및 PowerShell 7.6 런타임을 지원(미리 보기 포함), 보안과 호환성, 장기 지원을 강화했습니다.
- 대규모 클러스터 관리에 Resource Placement와 업데이트 실패 허용 임계치(미리 보기)가 추가되어 플랫폼 및 어플리케이션 팀의 운영 효율성을 높이고, 장애 허용 정책 구현이 강화되었습니다.
- AKS Prepared Image 기능(미리 보기)은 AI·GPU 등 고성능 워크로드에서 빠른 스케일아웃 및 효율적인 노드 초기화가 가능하여 성능 향상이 기대됩니다.
- Azure Sphere OS 26.09이 평가용으로 배포되어 장기 지원 Linux 커널 업그레이드 및 신뢰성 테스트 환경이 마련되었습니다.

### [Application Routing with Gateway API](https://azure.microsoft.com/updates?id=567944)
AKS에서 Kubernetes Gateway API 기반 인그레스 관리가 정식 지원되며, 서비스 메시 없이 표준 라우팅 모델을 활용할 수 있습니다.

### [Azure Functions support for Python 3.14](https://azure.microsoft.com/updates?id=567646)
Python 3.14로 Azure Functions 개발 및 배포가 가능해졌으며, 보안성과 호환성, 장기 지원이 개선되었습니다.

### [Azure Automation supports PowerShell 7.6 runbooks](https://azure.microsoft.com/updates?id=568102)
PowerShell 7.6 런북과 최신 런타임 환경 업그레이드가 지원되어 스크립트 포터빌리티, 보안, 관리 편의성이 향상되었습니다.

### [Resource placement in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567931)
Fleet Manager에서 여러 AKS 또는 Arc 클러스터에 리소스를 일괄 배포할 수 있어 대규모 환경의 운영 효율이 크게 개선되었습니다.

### [Prepared Image Specification (Preview)](https://azure.microsoft.com/updates?id=567949)
AKS 노드를 이미지 준비 후 사전 구성하여, 신규 노드의 빠른 기동과 자동화, 효율적 확장이 가능합니다.

---

## 🔒 보안 & 네트워킹

네트워킹 및 보안 분야는 Confidential Computing, 네트워크 보안 경계, VPN Gateway IPv6, HTTP 헤더 삽입 및 NAT64 같은 주요 신기능 출시와, DDoS Protection, Azure Enclave, WAF 예외/프론트도어 엣지 액션 등 미리 보기 기능으로 인프라 전체의 보호 영역이 넓어졌습니다.

- Azure Event Hubs Dedicated의 Confidential Computing 지원으로 데이터 사용 중 보호 및 신뢰 실행 환경이 확대되었습니다.
- 네트워크 보안 경계(NSP)는 PaaS 리소스의 논리적 네트워크 분리와 경계 기반 접근 제어를 정식 지원합니다.
- VPN Gateway는 IPv6 듀얼 스택 구성, NAT Gateway의 NAT64로 IPv6에서 IPv4 목적지 통신을 지원해 지속적인 네트워크 현대화가 이루어졌습니다.
- Azure Firewall의 HTTP/HTTPS 헤더 삽입, Entra 기반 Blob Storage SFTP 인증 등으로 네트워크 보안 강화가 이뤄졌습니다.
- 미리 보기로 Azure Enclave, Front Door Edge Actions, DDoS Protection 커스텀 정책, WAF 예외 등 정교한 통제 및 고급 보안 설계가 가능해졌습니다.

### [Confidential Computing support for Azure Event Hubs Dedicated](https://azure.microsoft.com/updates?id=567212)
이벤트 스트림 데이터의 메모리 내 보안처리 지원, 규제·보안 강화 환경에 최적화된 신기능.

### [Network Security Perimeter support for Azure Event Hubs](https://azure.microsoft.com/updates?id=567203)
PaaS 리소스에 네트워크 경계 지정, 접근 제어를 통한 데이터 유출 위험 감소.

### [HTTP header insertion in Azure Firewall](https://azure.microsoft.com/updates?id=568115)
HTTP/HTTPS 요청 헤더 자체 삽입 지원, 엔터프라이즈 수준의 접근 제어와 보안 통합.

### [NAT64 on StandardV2 NAT Gateway](https://azure.microsoft.com/updates?id=568409)
IPv6 워크로드를 IPv4 목적지로 변환하여 통신 가능, 클라우드 네이티브 네트워크 현대화 증진.

### [IPv6 support for Azure VPN Gateway](https://azure.microsoft.com/updates?id=567847)
IPv6 내·외부 트래픽을 VPN 터널로 지원, 미래 네트워크 환경과 이기종 인프라 연계 강화.

---

## 🗄️ 데이터 & 스토리지

데이터베이스, 스토리지 및 복구 환경은 Azure Blob Storage의 데이터 무결성 향상, SFTP 인증 통합, Storage Mover와 NetApp Files 등 멀티클라우드·대용량 데이터 이관 및 관리, Site Recovery의 고속 데이터 복구 등이 두드러집니다.

- Azure Blob Storage의 클라이언트 사이드 CRC64-NVME 체크섬으로 엔드투엔드 데이터 무결성이 보장됩니다.
- Entra ID 기반 SFTP 접속(정식 지원)으로 인증·권한 강화 및 운영 자동화가 확대되었습니다.
- Storage Mover 미리 보기는 GCS에서 Azure Blob으로 무중단·보안 집중 데이터 이관을 지원하여 복잡한 멀티클라우드 환경의 통합에 유리합니다.
- NetApp Files의 SMB Oplocks 설정(미리 보기)으로 볼륨 설정의 유연성과 성능 조정이 가능합니다.
- Azure Site Recovery는 최대 5x(500MB/s/VM) 데이터 변경량을 지원해 고속 복원·복구를 실현합니다.

### [Client-side data integrity protections in Azure Blob Storage](https://azure.microsoft.com/updates?id=566895)
SDK 기반 CRC64-NVME 체크섬 사용으로 실질적 데이터 무결성 검증 가능.

### [Microsoft Entra ID-based access for Azure Blob Storage SFTP](https://azure.microsoft.com/updates?id=567085)
Entra ID 인증 및 RBAC/ABAC, MFA 등 일관된 보안 정책 적용.

### [Public Preview: Azure Storage Mover supports migration from GCS](https://azure.microsoft.com/updates?id=566948)
GCS 데이터 이동 완전 자동화, Private Link 통한 네트워크 분리 지원.

### [Support for SMB Opportunistic Locking (Oplocks) configuration (Preview)](https://azure.microsoft.com/updates?id=568396)
NetApp Files 볼륨 별 SMB Oplocks 설정·관리로 성능 조정 및 캐싱 최적화 가능.

### [Support 5x churn in Azure Site Recovery](https://azure.microsoft.com/updates?id=566966)
500MB/s까지 고속 데이터 변경량 처리, 빅데이터·애널리틱스 등 대규모 워크로드 복구 지원.

---

## 📊 데이터 분석 & AI/ML

이번 달 AI·분석 영역은 Azure Databricks의 최신 AI 모델 서빙, Document PII Playground, Claude Sonnet/Opus/GPT-5.6 출시, AI Gateway 미리 보기 등 Azure 생태계의 지능화와 Fabric·Foundry 플랫폼의 통합이 더욱 심화되었습니다.

- GPT-5.6, Claude Sonnet 5, Opus 5 등 최신 대형언어모델(LLM)이 Azure Databricks에서 정식 지원되어 기업의 등급 AI 애플리케이션 구축이 활성화됩니다.
- AI Gateway 미리 보기(Azure API Management)는 다양한 AI 모델·툴을 안전하게 연동·관리할 수 있게 하며 Microsoft Foundry 연동도 확대되었습니다.
- Azure AI Language의 Document PII Playground, Foundry 신기능으로 개인정보 탐지 및 검증이 실시간·쉽게 이루어집니다.
- Claude Opus 및 Sonnet 5는 코딩·장기 작업, 전문가 워크플로우에 적합한 하이브리드 추론능력을 제공, 비용·성능 최적화.
- Azure Databricks Serverless(UK West), Microsoft Build Toolbox, AI 모델 연동 등으로 분석·운영 자동화와 개발자 경험이 크게 강화되었습니다.

### [Open AI GPT-5.6 on Azure Databricks](https://azure.microsoft.com/updates?id=567431)
최신 GPT-5.6 모듈 제공, Unity AI Gateway와 데이터 거버넌스 연동.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)
샘플 기반 PII 탐지 실시간 검증, 개인정보 레드랙션 업무 자동화 지원.

### [AI Gateway in Azure API Management (Preview)](https://azure.microsoft.com/updates?id=568184)
AI 모델, 툴, MCP 서버를 통합 관리하고 보안 및 관측성 강화.

### [Claude Opus 5 on Azure Databricks](https://azure.microsoft.com/updates?id=568316)
고급 추론, 코딩, 복잡한 에이전트 워크플로우 AI 모델 적용 가능.

### [Anthropic Claude Sonnet 5 on Azure Databricks](https://azure.microsoft.com/updates?id=567194)
Agentic LLM 정식지원, 코딩, 장기 업무 및 저비용 고효율 환경 구축.

---

## ⚙️ 관리·자동화·마이그레이션

관리와 거버넌스 분야는 PowerShell/Python 런타임 지원, Runbook 관리, 최대 장애 허용, Chaos Studio, Site Recovery 등 자동화와 복원력, 마이그레이션의 신기능이 두드러졌습니다.

- PowerShell 7.6 및 Python 3.14 정식 지원, 자동 Runbook 업그레이드와 새로운 런타임 관리로 운영 자동화 효율성이 상승.
- Chaos Studio Workspaces & Scenarios(미리 보기), Azure CLI에서 직접 시나리오 생성·실행 등 대규모 복원력 테스트가 간소화.
- Log Analytics Export Job(미리 보기), Application Insights에 AI 데이터 민감 정보 테이블 분리·접근제어 등 데이터 거버넌스 강화.
- Storage Mover(GCS부터 Azure Blob, 미리 보기)로 보안 중심 클라우드 데이터 마이그레이션 자동화.
- Site Recovery는 높은 데이터 변경량 지원으로 대형 워크로드 복구 신뢰성 증대.

### [Azure Automation supports PowerShell 7.6 runbooks](https://azure.microsoft.com/updates?id=568102)
최신 런타임, 자동 스크립트 모듈 관리로 보안 및 생산성 향상.

### [Azure Chaos Studio Workspaces and Scenarios (Preview)](https://azure.microsoft.com/updates?id=567184)
앱 중심 복원력 테스트 자동화, 시나리오 기반 장애 검증 및 보고서 생성.

### [Export historical data from Log Analytics workspace with Export jobs (Preview)](https://azure.microsoft.com/updates?id=566591)
이력 데이터 쿼리·추출, 규제·보안/분석/비즈니스 연계 활용성 확대.

### [Manage Azure Chaos Studio from Azure CLI (Preview)](https://azure.microsoft.com/updates?id=567225)
Azure CLI에서 복원력 시나리오 생성·실행, 운영 자동화 및 시행 효율성 증대.

### [Public Preview: Azure Storage Mover supports migration from GCS](https://azure.microsoft.com/updates?id=566948)
GCS에서 Azure Blob Storage로 클라우드 데이터 자동화·보안 마이그레이션 지원.

---

## 🛡️ 서비스 & 인프라(운영, 지역, 기타)

글로벌 클라우드 운영, 신지역·인프라, 서비스 커버리지 및 정책 관련 이슈가 집중되어 기업의 멀티 클라우드 전략 수립에 기반 제공합니다.

- 인도 South Central 및 칠레 Central 신규 데이터센터 개설, PostgreSQL Flexible Server 인도 신규 지역 배포, 영국 Databricks Serverless 지원 등 현지화와 글로벌 확장.
- Azure Kubernetes Fleet/Fleet Manager, NAT Gateway, Azure Site Recovery, Azure Sphere 등 인프라 신기능을 통한 안정성 및 효율성 증대.
- Azure Reservation Policy 변경, Savings Plan 적용 서비스 예약 교환 종료 등 비용 및 정책 변화에 따른 장기 전략 수립 주의 필요.

### [Microsoft Azure now available from new cloud region in India (India South Central)](https://azure.microsoft.com/updates?id=568013)
현지화, 데이터 거주, AI 준비 인프라 강화 및 확장.

### [Azure Red Hat OpenShift in Chile Central](https://azure.microsoft.com/updates?id=566732)
칠레 신규 지역에서 OpenShift 완전 관리환경 제공, 현지 규제·성능 최적화.

### [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)
UK West 지역에 Serverless SQL 워크로드 배포, 자동화·탄력적 인프라 제공.

### [Reservation exchanges for services supported by savings plans ending](https://azure.microsoft.com/updates?id=568514)
Savings Plan 도입 서비스 예약 교환 2027년 2월부터 종료, 비용관리 정책 변화 주의 필요.

### [Azure Database for PostgreSQL flexible server in India South Central](https://azure.microsoft.com/updates?id=568334)
인도 South Central 지역에서 PostgreSQL Flexible Server 사용 가능, 아시아 현지화 확대.

---

## 🧰 Microsoft Foundry

Foundry 영역에서는 Toolboxes 기능 정식 지원, Document PII NextGen Playground와 NextGen 샘플 playground 미리 보기 등 조직의 지능형 Agent 및 툴 관리, 개인정보 자동화 처리 등 AI 개발, 보안 거버넌스 효율성이 크게 강화되었습니다.

- Toolboxes 정식 출시로 다양한 MCP, REST, Connector, Skill을 가버넌스 정책 기반 묶음으로 관리, 재사용이 가능.
- Document PII Playground는 개인정보 탐지 자동화 및 실시간 검증 환경 제공, 규제 준수와 신속한 업무 처리 지원.
- 엔터프라이즈 등 대규모 AI 조직이 Foundry를 통한 데이터 실무 자동화를 쉽게 도입 가능.

### [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)
공용 MCP 엔드포인트 통한 통합 툴 호출, 조직 내 정책 기반 툴 관리 및 일관된 연동 지원.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)
신규 샘플 기반 Playground, 실시간 개인정보 검증·비교 기능 제공.

### [Public Preview: Document PII playground sample in Microsoft Foundry NextGen](https://azure.microsoft.com/updates?id=563331)
실제 문서 샘플로 PII 식별 결과 실시간 테스트, API 통합 전 신속 평가 가능.

---

## 🖇 Microsoft Fabric

Microsoft Fabric 영역에서는 Azure Monitor 로그 미러링(미리 보기) 등 Azure 고급 관측성 데이터와 Fabric의 심층 분석을 결합해 조직 내 연계·분석 역량이 확장되고 있습니다.

- Azure Monitor Log Analytics의 Fabric 연동 지원으로 원격 데이터와 Fabric의 Power BI, Spark 등 분석 기술을 통합.
- 통합된 관측성 및 비즈니스 데이터 분석이 가능해져 크로스 도메인·운영 맥락에서 데이터 활용이 강화됩니다.

### [Azure Monitor Logs mirroring into Microsoft Fabric (Preview)](https://azure.microsoft.com/updates?id=568322)
Log Analytics 워크스페이스 데이터를 실시간 OneLake Delta Parquet 포맷으로 Fabric에서 분석.

---

## 총평 및 다음 달 전망

7월의 Azure 업데이트는 AI, 자동화, 데이터 거버넌스, 글로벌 확장, 보안 강화 등 주요 클라우드 트렌드가 응축된 한 달이었습니다. 최신 AI 모델의 정식 지원과 Foundry·Fabric 통합 기능은 기업의 데이터 및 지능형 애플리케이션 경쟁력 확보에 커다란 변화를 촉진했으며, 관리 및 보안 자동화 신기능 출시로 복잡한 환경에서의 운영 안정성·효율성이 대폭 강화되었습니다. 또한 신지역 개설과 멀티클라우드 지원 확장으로 현지화, 글로벌 접근성도 확대되고 있습니다.

다음 달에는 GA 및 Preview 기능들의 피드백을 반영한 안정화, 더 깊은 AI·데이터 플로우 통합, Fabric 및 Foundry 플랫폼의 가버넌스 기능 확장, 보안 및 네트워크 경계 기술의 정교화가 더욱 기대됩니다. 지속적인 런타임 지원 정책 변화와 인프라 자동화 신기능 출시, 그리고 데이터 거버넌스와 AI 텔레메트리 보호 기술이 기업의 클라우드 전략 및 운영에 중요한 시사점을 줄 것입니다.