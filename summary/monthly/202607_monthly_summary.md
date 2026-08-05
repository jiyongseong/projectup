# Azure 월간 업데이트 요약 - 2026년 07월

## 전반적인 트렌드와 핵심 인사이트

2026년 7월 Azure 업데이트는 AI와 데이터 분석, 보안·거버넌스 강화, 멀티·하이브리드 클라우드 지원, 개발자 경험 개선, 서비스 지역 확장 등 다양한 혁신을 선보였습니다. 특히 Azure Databricks, Microsoft Foundry, AI 모델 서빙, Event Hubs, Kubernetes Fleet Manager 등 핵심 서비스의 기능 고도화가 두드러집니다.

AI 분야에서는 Anthropic Claude Sonnet 5, Claude Opus 5, OpenAI GPT-5.6 등 최신 모델과 모델 서빙 게이트웨이가 추가되어, 엔터프라이즈 업무 효율화와 고품질 AI 예측·대화 처리가 가능하게 됐습니다. Microsoft Foundry는 Toolboxes와 PII 탐지 기능을 제공, 조직 내 AI 통합과 데이터 보호 문제를 실질적으로 해결합니다. Azure Monitor와 Microsoft Fabric 연동을 통한 로그 및 진단 데이터 분석, Power BI·Spark를 활용한 실시간 분석이 지원되어 비즈니스·운영·애플리케이션 데이터 통합 분석이 본격화됐습니다.

보안 및 거버넌스 영역에서는 Event Hubs의 기밀 컴퓨팅, 네트워크 보안 경계(Perimeter) 도입, Azure Firewall의 HTTP 헤더 검사, Entra ID 기반 SFTP 인증, Blob Storage 클라이언트 측 무결성 검증, Azure DDoS 커스텀 정책 등 데이터 흐름 전체에 보안 강화를 적용합니다. Key Vault Premium의 대칭키 지원, Azure Enclave 등 보안 인프라 솔루션도 확대됐습니다.

멀티클라우드 및 지역 확장 역시 인상적입니다. Azure Database for PostgreSQL 및 Databricks SQL Serverless 등 주요 서비스가 인도·영국 등 신규 지역에 출시됐고, Azure Red Hat OpenShift도 칠레에 도입돼 라틴아메리카 지역 클라우드 기반 확대를 지원합니다. Storage Mover는 GCS로부터의 클라우드-클라우드 마이그레이션을 간소화하며, Azure Files NFS와 AKS의 연동 보안도 한층 강화되었습니다.

개발자 경험 개선을 위한 PowerShell 7.6 및 Python 3.14 지원, AKS Gateway API 기반 라우팅, Fleet Manager 클러스터 리소스 배치, Site Recovery의 초고속 복구, API Management의 AI Gateway 등 자동화·통합 관리 기능이 강화되었고, Chaos Studio와 CLI 통합, Application Gateway·Front Door WAF 예외 정책 등 복원력·신뢰성 확보도 발전하고 있습니다.

이달은 '보안·컴플라이언스 자동화', 'AI를 통한 데이터 분석 및 비즈니스 혁신', '멀티클라우드 및 글로벌 서비스 확장', '클라우드 네이티브 개발 환경 고도화'가 주요 테마입니다. 향후 Azure는 AI 및 자동화 기반 운영 효율화, 실시간 데이터 분석과 보안 내재화, 글로벌 서비스 디지털 트랜스포메이션 가속화에 주력할 것으로 전망됩니다.

---

## 🧬 AI & 머신러닝

이번 달 Azure는 AI 모델 업데이트와 엔터프라이즈 AI 관련 기능 강화에 집중했습니다. Claude Opus 5, Claude Sonnet 5, OpenAI GPT-5.6 등 최신 AI 모델을 Azure Databricks에 정식 지원하며, 모델 서빙과 게이트웨이 확대, Microsoft Foundry의 PII 탐지와 Toolboxes 공개로 실무 적용 범위를 넓혔습니다. 엔터프라이즈 데이터 기반의 AI 분석, 자동화 적용 역시 강화되었습니다.

### [Claude Opus 5 on Azure Databricks](https://azure.microsoft.com/updates?id=568316)
Anthropic의 최신 Claude Opus 5 모델이 Azure Databricks에서 정식 지원되어, 기업이 복잡한 추론, 장기 계획, 코딩 업무 등을 AI로 효율화할 수 있게 되었습니다.

### [Anthropic Claude Sonnet 5 on Azure Databricks](https://azure.microsoft.com/updates?id=567194)
Sonnet 5는 비용 효율성과 신속성을 갖춘 하이브리드 AI로, 대규모 코드 자동화, 다중 파일 작업, 장기 실행 AI 에이전트 개발에 적합합니다.

### [Open AI GPT-5.6 on Azure Databricks](https://azure.microsoft.com/updates?id=567431)
OpenAI GPT-5.6을 Azure Databricks에서 모델 서빙 엔드포인트로 사용할 수 있게 되어, Foundry 및 Unity AI Gateway와 연동한 안전한 AI 앱 구축이 쉬워졌습니다.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)
문서 기반 PII 엔터티 탐지가 고도화되어, 법률, 컴플라이언스, 데이터보호팀이 쉽고 빠르게 민감정보 감지와 프로젝트 범위를 정할 수 있게 되었습니다.

### [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)
Foundry의 Toolboxes 기능은 프롬프트 에이전트에서 자주 사용하는 툴을 통합·재사용할 수 있는 MCP 호환 엔드포인트로, 조직 내 AI 통합 및 거버넌스 효과를 높입니다.

---

## ☁️ 컴퓨트, 컨테이너, 개발자 경험

컴퓨트 및 컨테이너 영역은 AKS Gateway API, Fleet Manager의 리소스 배치, Python 3.14 지원, AKS Prepared Image 등 클라우드 네이티브 개발의 도약을 보여줍니다. 자동화, 런타임 관리, PowerShell 7.6 및 Azure Site Recovery의 초고속 복구, Chaos Studio CLI 통합 등 개발자·운영자 편의성도 증진되었습니다.

### [Application Routing with Gateway API on AKS](https://azure.microsoft.com/updates?id=567944)
AKS에서 Gateway API 기반으로 애플리케이션 라우팅을 정식 지원하여, nginx 기반 경로에서 표준화된 라우팅 모델로 점진적 전환이 가능합니다.

### [Azure Automation supports PowerShell 7.6 runbooks](https://azure.microsoft.com/updates?id=568102)
PowerShell 7.6 런북 및 최신 스크립트 런타임 환경을 정식 지원해, 자동화 코드의 최신화, 효율성, 보안성 모두 개선되었습니다.

### [Azure Functions support for Python 3.14](https://azure.microsoft.com/updates?id=567646)
Python 3.14를 기반으로 로컬 개발 후 Azure Functions 플랜에 배포가 가능하며, 보안·호환성 및 장기 지원이 강화되었습니다.

### [Resource placement in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567931)
Fleet Manager에서 멀티클러스터 리소스 배치 API와 Azure 포털 관리 경험이 정식 지원되어, 대규모 업데이트와 리소스 관리가 자동화됩니다.

### [Support 5x churn in Azure Site Recovery](https://azure.microsoft.com/updates?id=566966)
Azure Site Recovery가 VM별 최대 500MB/s의 초고속 입출력을 지원, 데이터베이스나 빅데이터 등 고부하 환경에서도 신뢰성 높은 재해복구가 가능합니다.

---

## 🔐 보안, 네트워킹, 컴플라이언스

보안과 네트워킹 분야는 네트워크 경계, 데이터 무결성, HTTP 헤더 처리, IPv6/NAT64, SFTP/Entra ID 통합 등 클라우드 보안의 전방위 강화를 보여줍니다. Key Vault Premium 대칭키, Enclave, DDoS 커스텀 정책 등 신뢰성에 기반한 확장적 보안도 함께 도입되었습니다.

### [Confidential Computing support for Azure Event Hubs Dedicated](https://azure.microsoft.com/updates?id=567212)
Event Hubs에서 기밀 컴퓨팅이 적용되어, 인메모리 스트리밍 데이터에 하드웨어 기반 TEE로 보안성을 극대화할 수 있습니다.

### [Client-side data integrity protections in Azure Blob Storage](https://azure.microsoft.com/updates?id=566895)
Azure Blob Storage SDK에 CRC64-NVME 무결성 검증이 추가되어, 클라이언트-스토리지 간 데이터가 바이트 단위로 완벽히 유지됨을 보장합니다.

### [HTTP header insertion in Azure Firewall](https://azure.microsoft.com/updates?id=568115)
Azure Firewall에서 HTTP/HTTPS 헤더 삽입이 가능, Entra 테넌트 제한, SaaS 접근 제어 등 다양한 시나리오의 네이티브 보안 정책 적용이 용이합니다.

### [IPv6 support for Azure VPN Gateway](https://azure.microsoft.com/updates?id=567847)
Azure VPN Gateway가 IPv6 듀얼 스택을 정식 지원, 온프레미스/브랜치 네트워크와 Azure 간 IPv4·IPv6 트래픽을 한 곳에서 처리할 수 있습니다.

### [NAT64 on StandardV2 NAT Gateway](https://azure.microsoft.com/updates?id=568409)
StandardV2 NAT Gateway의 NAT64 기능으로 IPv6 워크로드가 IPv4 전용 인터넷 대상과 통신할 수 있게 되어, 차세대 네트워크 환경을 쉽게 구축 가능합니다.

---

## 💾 스토리지 & 데이터 플랫폼

스토리지 및 데이터 서비스는 Blob Storage/SFTP/Entra ID 통합, Files NFS 전송 암호화, Storage Mover GCS 마이그레이션, PostgreSQL PowerShell 모듈 등 데이터 이동·보안·자동화 고도화를 제공하며, 로그 분석·장기 보관, NetApp Files의 Oplocks도 플렉시블하게 지원합니다.

### [Microsoft Entra ID-based access for Azure Blob Storage SFTP](https://azure.microsoft.com/updates?id=567085)
Entra ID 인증 기반 SFTP 접속이 Blob Storage에서 정식 지원되어, MFA·조건부 접근·RBAC 등 조직 정책과 일관된 보안 모델을 적용할 수 있습니다.

### [Encryption in Transit for Azure Files NFS Shares in AKS](https://azure.microsoft.com/updates?id=567787)
AKS와 Azure Files NFS v4.1 연결 시 TLS 기반 암호화 전송이 정식 지원, 데이터 이동시 보안·컴플라이언스 요건 충족이 쉬워졌습니다.

### [Azure Storage Mover supports migration from Google Cloud Storage](https://azure.microsoft.com/updates?id=566948)
GCS에서 Azure Blob Storage로 클라우드-클라우드 마이그레이션이 공개 미리 보기로 지원, S3 호환 인터페이스와 키 관리, 프라이빗 링크로 안전하게 데이터를 이동 가능합니다.

### [New Powershell module: Az.PostgreSQLFlexibleServer](https://azure.microsoft.com/updates?id=566209)
Az.PostgreSQLFlexibleServer PowerShell 모듈이 출시되어 PostgreSQL 18, 엘라스틱 클러스터 등 최신 기능을 PowerShell에서 쉽게 활용·관리할 수 있습니다.

### [Support for SMB Opportunistic Locking (Oplocks) configuration](https://azure.microsoft.com/updates?id=568396)
Azure NetApp Files의 Oplocks 설정이 SMB·듀얼 프로토콜 볼륨에서 미리 보기로 지원되어, 캐싱 및 성능 최적화가 가능합니다.

---

## 🌐 관리 및 거버넌스, DevOps, 마이그레이션

운영 관리, DevOps, 마이그레이션은 Chaos Studio, Azure Monitor, API Management AI Gateway, 로그 미러링·이관, 예약 교환 정책, 런타임·레거시 버전 지원 종료 등 서비스 신뢰성, 자동화, 클라우드 비용 정책 변화 등이 강조됩니다.

### [Azure Chaos Studio Workspaces and Scenarios](https://azure.microsoft.com/updates?id=567184)
Chaos Studio가 Workspaces/Scenarios 개념으로 복원력 테스트를 자동화·애플리케이션 중심으로 구성, 실제 장애 발생 패턴을 시뮬레이션할 수 있게 되었습니다.

### [Azure Monitor Logs mirroring into Microsoft Fabric](https://azure.microsoft.com/updates?id=568322)
Azure Monitor 로그를 마이크로소프트 Fabric OneLake로 실시간 미러링·분석할 수 있어, 운영 데이터와 비즈니스 데이터의 통합 분석이 가능해졌습니다.

### [AI Gateway in Azure API Management](https://azure.microsoft.com/updates?id=568184)
AI Gateway는 Microsoft Foundry, AWS, Google Vertex, Anthropic 모델을 통합 관리·보안·관측성 정책을 일관적으로 적용할 수 있는 AI 특화 API 매니지먼트 옵션의 미리 보기입니다.

### [Support for Python-2.7; 3.8 and PowerShell- 7.1; 7.2 will be retired](https://azure.microsoft.com/updates?id=567556)
Automation에서 파이썬 2.7, 3.8 및 PowerShell 7.1·7.2는 2026년 9월 30일부터 지원 종료되며, 보안·버그픽스가 중단되어 빠른 업그레이드가 필수입니다.

### [Reservation exchanges for Azure services supported by savings plans will no longer be available](https://azure.microsoft.com/updates?id=568514)
2027년 2월 1일부터 Savings Plan이 적용된 서비스의 예약 교환이 중단되어, Compute·Database 등 주요 서비스의 예약 정책 변화가 예정되어 있습니다.

---

## 🏭 Microsoft Foundry & Microsoft Fabric

Microsoft Foundry는 AI 에이전트 및 Toolboxes 중심의 확장적 AI 통합, 실용적인 PII 탐지·차세대 Playground, 수집/통합/재사용 가능한 API 구현 경험을 제공하며, Fabric은 로그 미러링을 통해 데이터 분석의 새로운 생태계를 제시합니다. Foundry NextGen Playground와 데이터 보호 정책도 강조됩니다.

### [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)
AI 프롬프트 에이전트/외부 Tool 재사용을 위한 MCP 호환 Toolboxes를 도입해, 조직 내 효율적 AI 도입·투명한 거버넌스·재사용성을 극대화할 수 있습니다.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)
PII 탐지 Playground가 엔터프라이즈 스케일에서 정식 지원되며, 민감정보 자동 평가와 프로젝트 범위 설정이 간편합니다.

### [Public Preview: Document PII playground sample in Microsoft Foundry NextGen](https://azure.microsoft.com/updates?id=563331)
Foundry NextGen 포털에서 문서 기반 PII 감지 샘플이 미리보기로 공개되어, 실시간 평가와 API 연동을 쉬운 방식으로 지원합니다.

### [Azure Monitor Logs mirroring into Microsoft Fabric](https://azure.microsoft.com/updates?id=568322)
Monitor 로그를 Fabric OneLake에 실시간 분석, 데이터 정규화 및 비즈니스 데이터와 융합 분석이 가능해져 Fabric 기반 클라우드 데이터 분석이 더욱 강화됩니다.

### [Protect sensitive generative AI telemetry in Application Insights and Microsoft Foundry](https://azure.microsoft.com/updates?id=567594)
AI 텔레메트리 보호용 GenAIContent 테이블 및 세분화된 접근제어로, Foundry·Application Insights에서 민감한 프롬프트/응답 등 데이터를 안전하게 관리할 수 있습니다.

---

## 📍 글로벌 및 신규 지역 출시, 한국 관련

이달은 인도, 영국, 칠레 등 신규 클라우드 지역 개설, 주요 서비스의 지역 확장과 데이터 주권 확립, 글로벌 클라우드 전략이 주목받았습니다. 아시아·남미 클라우드 커버리지 확대, 인도 South Central 신규 리전, Databricks SQL Serverless 등 지역별 맞춤형 클라우드 제공이 특징입니다.

### [Azure Database for PostgreSQL flexible server in India South Central](https://azure.microsoft.com/updates?id=568334)
인도 South Central 지역에서 PostgreSQL flexible server를 정식 지원, 데이터 주권·지역 맞춤형 서비스가 강화되었습니다.

### [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)
UK West에서 Databricks SQL Serverless 정식 지원, 인스턴트 컴퓨트·자동스케일링·거버넌스가 가능해져 지역 데이터 분석이 한층 진화됐습니다.

### [Azure Red Hat OpenShift in Chile Central](https://azure.microsoft.com/updates?id=566732)
칠레 Central에 Azure Red Hat OpenShift 클러스터 출시로, 라틴 아메리카에서 클라우드 네이티브 워크로드·AI 기반 앱 개발이 실현됩니다.

### [Microsoft Azure now available from new cloud region in India (India South Central)](https://azure.microsoft.com/updates?id=568013)
인도 Hyderabad에 신설 리전 개설, AI 준비된 인프라, 데이터 주권, 낮은 레이턴시, resilient capacity 등 지역 디지털 전환이 본격 현실화됐습니다.

---

## 총평 및 다음 달 전망

2026년 7월 Azure 업데이트는 AI·데이터 분석, 보안·거버넌스, 지역 확장, 클라우드 네이티브 개발 환경 고도화가 핵심입니다. Anthropic, OpenAI 등 최신 AI 모델과 Microsoft Foundry의 통합 프레임워크가 엔터프라이즈 혁신을 주도하고, 네트워크·스토리지 보안, 데이터 무결성, 자동화·복원력 향상으로 클라우드 신뢰성과 운영 효율성이 크게 개선되고 있습니다. 신규 리전 개설과 글로벌 서비스 확대는 국제적 데이터 주권 및 맞춤형 클라우드 제공 전략을 강화합니다.

향후 Azure는 AI와 자동화 중심의 운영 최적화, 글로벌 클라우드 인프라 확장, 클라우드 네이티브 서비스 간 유기적 통합, 실시간 데이터 보호와 복원력 확보에 집중할 것으로 예상됩니다. 개발자·운영자·보안 담당자 모두를 위한 생산성 도구와 고도화된 관측성, 정책 기반 관리가 Azure 미래의 핵심 전략이 될 것입니다.