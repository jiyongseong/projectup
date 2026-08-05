# Azure 월간 업데이트 요약 - 2026년 07월

## 전반적인 트렌드와 핵심 인사이트

2026년 7월 Azure 업데이트는 인프라의 확장, 보안 강화, AI 및 데이터 분석 플랫폼의 고도화, 관리 효율성 향상, 하이브리드/멀티클라우드 지원, 그리고 클라우드 네이티브 개발 패턴의 진화에 중점을 두고 있습니다.  
특히 '정식 지원'(General Availability)으로 다양한 신기능이 복수의 리전 및 서비스에 쏟아졌으며, '미리 보기'(preview) 단계의 혁신적인 기능 또한 서비스 전반에 적용되고 있습니다.

이번 달은 인공지능(AI) 효율 향상을 위한 Azure Databricks의 GPT-5.6, Claude Opus 5, Claude Sonnet 5 도입과 Microsoft Foundry의 도구 체계 표준화, 그리고 Azure API Management 내 AI Gateway와 Fabric 연동 등, 조직별 AI 활용을 극대화하기 위한 기반이 크게 강화되었습니다.  
운영 및 관리 측면에서는 PowerShell 7.6 적용, Site Recovery 5x 향상, Chaos Studio의 시나리오 자동화 등 자동화와 신뢰성 확대에 집중하였고, 네트워킹에서는 NAT64, IPV6 및 표준 서비스 엔드포인트, DDoS 맞춤 정책이 추가되어 멀티클라우드 및 하이브리드, 대량 트래픽을 고려한 견고한 인프라 구축을 뒷받침합니다.

스토리지와 보안 역시 진화되었습니다. Blob Storage SFTP의 Entra ID 통합과 데이터 무결성 검증, 네트워크 기밀 컴퓨팅(Event Hubs), Application Gateway 및 Front Door의 WAF 예외 정책 등, 조직의 데이터 보호와 컴플라이언스 요구에 부합하는 기능이 강화됐습니다.

Azure의 지역 확장 또한 눈에 띄었습니다(인도 South Central, 칠레 Central 등), 메시지 기반 하이브리드/멀티클라우드 지원과 전통적 데이터베이스, 관리 역량까지 다양한 영역에 혁신이 적용되었습니다.  
전반적으로 이번 달은 Azure의 전 세계 확장, 신뢰성, AI 역량 강화, 보안 표준화, 그리고 운영 효율화를 목표로 한 다중적 기술 진보가 이루어졌다고 분석됩니다.

---

## ☁️ 컴퓨트 & 컨테이너

클라우드 네이티브 워크로드 지원 강화를 위해 AKS에서 Gateway API 및 Prepared Image Specification 같은 최신 Kubernetes 표준 도입이 이루어졌으며, Azure Functions가 Python 3.14와 PowerShell 7.6을 지원함에 따라 개발자들의 엔터프라이즈 확장성이 증대되었습니다.  
Fleet Manager의 리소스 배치 및 업데이트 실패 허용 등 멀티클러스터 운영 효율성이 크게 향상되었습니다.

### [Application Routing with Gateway API](https://azure.microsoft.com/updates?id=567944)
AKS에서 Kubernetes Gateway API를 통한 애플리케이션 라우팅 정식 지원. 기존 ingress-nginx 모델과 병행 사용 가능, 점진적 마이그레이션 지원.

### [Azure Functions support for Python 3.14](https://azure.microsoft.com/updates?id=567646)
Python 3.14 기반 함수 개발 및 배포 정식 지원. 보안 및 장기지원 윈도우, 최신 개발도구 호환성 제공.

### [Resource placement in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567931)
Fleet Manager의 리소스 배치 API 및 포털 UX 제공, 멀티 클러스터 자동화 적용으로 운영 부담 감소.

### [Public Preview: Azure Functions Support for PowerShell 7.6](https://azure.microsoft.com/updates?id=567651)
PowerShell 7.6 기반 함수 개발 미리 보기 제공. 최신 언어와 보안 기능 활용.

### [Public Preview: Prepared Image Specification](https://azure.microsoft.com/updates?id=567949)
AKS 노드 이미지 사전 지정 미리 보기, 컨테이너 이미지와 커스텀 설정 포함으로 서버 스케일링이 신속해짐.

---

## 🔒 보안 & 네트워킹

이번 달은 Confidential Computing, NAT64, IPv6, Network Security Perimeter 등 네트워크와 보안 측면에서 다각적인 신기능이 적용되었습니다.  
WAF의 예외 정책과 DDoS 맞춤 정책으로 세밀한 트래픽 제어 가능, Enclave 및 Key Vault 대칭키는 규제 산업과 고신뢰 환경에 적합한 솔루션을 제공합니다.

### [Confidential Computing support for Azure Event Hubs Dedicated](https://azure.microsoft.com/updates?id=567212)
기밀 컴퓨팅 기반 이벤트 허브 스트리밍 데이터 보호 정식 지원, TEE를 활용한 인메모리 데이터 보안.

### [HTTP header insertion in Azure Firewall](https://azure.microsoft.com/updates?id=568115)
HTTP/HTTPS 헤더 삽입 기능, 엔터프라이즈 접근 및 보안 정책 통합 간소화.

### [IPv6 support for Azure VPN Gateway](https://azure.microsoft.com/updates?id=567847)
IPv6 트래픽의 VPN 게이트웨이 지원, 듀얼스택 환경에서 IPsec/IKE 기반 안전 네트워크 연결.

### [NAT64 on StandardV2 NAT Gateway](https://azure.microsoft.com/updates?id=568409)
IPv6 → IPv4 트래픽 NAT 변환 지원, DNS64 연동으로 하이브리드 환경 확장 및 통합.

### [In preview: Azure DDoS Protection custom policy](https://azure.microsoft.com/updates?id=568063)
DDoS 보호 맞춤 정책 미리 보기, 프로토콜별 인바운드 임계치 개별 설정 가능.

---

## 💾 스토리지 & 데이터 관리

스토리지와 데이터 관리 영역은 Blob Storage의 클라이언트 무결성 검증, Entra ID SFTP, Azure Files NFS 암호화, Azure Storage Mover의 멀티클라우드 지원 등이 두드러집니다.  
Log Analytics의 내보내기, NetApp Files의 Oplocks 설정 등 데이터 처리 및 이관 효율성이 크게 늘어났습니다.

### [Client-side data integrity protections in Azure Blob Storage](https://azure.microsoft.com/updates?id=566895)
.NET/C++/JS SDK에서 CRC64-NVME 데이터 무결성 검사 지원, 엔드-투-엔드 데이터 보증 강화.

### [Microsoft Entra ID-based access for Azure Blob Storage SFTP](https://azure.microsoft.com/updates?id=567085)
Entra ID 인증 기반 SFTP 접속 정식 지원, Guest(B2B) 활용 가능. MFA 및 조건부 접근정책 적용.

### [Encryption in Transit for Azure Files NFS Shares in AKS](https://azure.microsoft.com/updates?id=567787)
AKS에서 NFS 인식 Azure Files의 TLS 암호화 지원, 저장소 클래스 설정으로 손쉽게 활성화 가능.

### [Public Preview: Azure Storage Mover now supports migration from Google Cloud Storage (GCS)](https://azure.microsoft.com/updates?id=566948)
GCS에서 Azure Blob Storage로의 마이그레이션 미리 보기 지원, S3 호환 인터페이스 활용.

### [In preview: Export historical data from Log Analytics workspace with Export jobs](https://azure.microsoft.com/updates?id=566591)
Log Analytics에서 쿼리 기반 데이터 내보내기 미리 보기, 컴플라이언스 및 분석 용도 지원.

---

## 📊 AI & 분석 / Azure Databricks

AI 분석 플랫폼 Azure Databricks에는 GPT-5.6, Claude Opus 5, Claude Sonnet 5 모델이 도입되어 대규모 엔터프라이즈 지능형 워크로드 구성이 용이해졌습니다.  
Eventhubs NSP 및 보안 통제, 데이터 분석(서버리스), 파운데이션 모델 연동, 로그 데이터의 Fabric 통합 등 데이터와 AI 중심 경험이 강화되었습니다.

### [Claude Opus 5 on Azure Databricks](https://azure.microsoft.com/updates?id=568316)
Anthropic Claude Opus 5 모델 서빙 지원, 복잡한 지추론‧코딩‧에이전트 워크플로우 구현.

### [Open AI GPT-5.6 on Azure Databricks](https://azure.microsoft.com/updates?id=567431)
GPT-5.6 모델 서빙 정식 지원, 관리형 워크스페이스 및 AI Gateway 연동으로 데이터 거버넌스 적용.

### [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)
SQL Serverless 워크로드 UK West 적용 정식 지원, 동적 확장 및 비용 효율화.

### [Generally available: Anthropic Claude Sonnet 5 on Azure Databricks](https://azure.microsoft.com/updates?id=567194)
Claude Sonnet 5 모델 도입, 신속성 및 비용 효율 높은 에이전트 개발환경 제공.

### [Azure Monitor Logs mirroring into Microsoft Fabric](https://azure.microsoft.com/updates?id=568322)
Log Analytics 데이터를 Fabric의 OneLake에 실시간 동기화, 운영·비즈니스 데이터 통합 분석 가능.

---

## 🛠️ Microsoft Foundry

Microsoft Foundry는 조직 단위 AI 에이전트·도구 활용 표준화에 초점을 맞추고 있습니다.  
Toolboxes(툴박스) GA, PII 탐지 플레이그라운드, Application Insights 연동 등, 개발-운영간 교차 경험과 거버넌스를 크게 강화하였습니다.

### [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)
툴박스 GA 출시, 다양한 AI/MCP/RESTAPI/커넥터 도구 묶음 배포 및 거버넌스 표준화.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)
PII 탐지 샘플 환경 정식 지원, 손쉬운 개인정보 검증 및 분석 경험 제공.

### [Public Preview: Document PII playground sample in Microsoft Foundry NextGen](https://azure.microsoft.com/updates?id=563331)
비동기 PII 파이프라인 및 샘플 경험 미리 보기 제공, 원문-마스킹 정보 실시간 비교.

### [Protect sensitive generative AI telemetry in Application Insights and Microsoft Foundry](https://azure.microsoft.com/updates?id=567594)
생성 AI 데이터(프롬프트, 응답 등) 별도 테이블에서 보안 통제 및 액세스 제어 지원.

### [AI Gateway in Azure API Management (Public Preview)](https://azure.microsoft.com/updates?id=568184)
AI Gateway 전용 티어 미리 보기, AI 자산/모델/툴의 보안 및 제어 표준화, Foundry/AWS/Google 모델 통합.

---

## 🌏 지역 및 글로벌 확장

Azure는 인도 South Central, 칠레 Central 등 신규 리전 오픈 및 데이터센터 확대에 집중하고 있습니다.  
지역별 컴플라이언스, 데이터주권, 네트워크 확장, OpenShift 등 비즈니스 연속성 기반이 함께 강화되었습니다.

### [Microsoft Azure now available from new cloud region in India (India South Central)](https://azure.microsoft.com/updates?id=568013)
인도 South Central 리전 신규 오픈, 지역 데이터주권·AI 준비형 인프라 지원.

### [Azure Database for PostgreSQL flexible server in India South Central](https://azure.microsoft.com/updates?id=568334)
PostgreSQL 유연 서버 인도 South Central 리전 적용 정식 지원, 하이브리드/멀티클라우드 워크로드 대비.

### [Azure Red Hat OpenShift in Chile Central](https://azure.microsoft.com/updates?id=566732)
칠레 Central 리전에서 ARO 지원, 지역 규제 산업·미션 크리티컬 워크로드에 Azure 기반 제공.

### [New Powershell module: Az.PostgreSQLFlexibleServer](https://azure.microsoft.com/updates?id=566209)
PostgreSQL 18, elastic cluster 등 최신 API/기능 PowerShell 모듈 제공, 관리 효율화.

### [Anthropic Claude Opus 5 및 Sonnet 5 모델, 다양한 지역 Databricks에서 사용 가능](https://azure.microsoft.com/updates?id=568316)
AI 모델 분석 플랫폼 정식 지원 확장, 클라우드 지역별 최적화 적용.

---

## ⚙️ 관리 및 거버넌스

운영 효율, 자동화, 이관, Site Recovery 신속성이 크게 향상되었습니다. PowerShell‧Python‧자동화 환경 최신화, Chaos Studio 시나리오 기반 장애 테스트 등, 지속적인 클라우드 관리 경험 고도화가 이루어졌습니다.

### [Azure Automation supports PowerShell 7.6 runbooks and Runtime environment](https://azure.microsoft.com/updates?id=568102)
PowerShell 7.6 런북 및 런타임 환경 정식 지원, 스크립트 이동 및 실행 환경 관리 용이.

### [Support 5x churn in Azure Site Recovery](https://azure.microsoft.com/updates?id=566966)
Site Recovery에서 최대 500MB/s VM IOPS 지원, 고성능 워크로드의 재해복구 신속성 확보.

### [Azure Chaos Studio Workspaces and Scenarios](https://azure.microsoft.com/updates?id=567184)
Chaos Studio의 워크스페이스/시나리오 기반 장애 테스트 미리 보기, 자동화·컴플라이언스 대응 강화.

### [Manage Azure Chaos Studio from the Azure CLI](https://azure.microsoft.com/updates?id=567225)
CLI에서 Chaos 시나리오 자동 생성·실행 지원, 운영 워크플로우 간소화.

### [Instant Access via application consistent restore points](https://azure.microsoft.com/updates?id=565758)
VM Restore Point의 실시간 접근 미리 보기, 빠른 복구 및 일관성 확보.

---

## 📣 주요 공지 및 정책 변화

장기적 운영 및 비용 효율 관점에서 예약 환전 정책, 지원 종료 예정(파이썬 2.7/3.8, PowerShell 7.1/7.2) 등이 안내되었습니다.

### [Support for Python-2.7; 3.8 and PowerShell- 7.1; 7.2 will be retired on September 30, 2026](https://azure.microsoft.com/updates?id=567556)
2026년 9월 30일 이후 해당 런타임 지원 종료, 보안 업데이트 미제공 예정. 최신 버전 업그레이드 권장.

### [Reservation exchanges for Azure services supported by savings plans will no longer be available starting Feb 1, 2027](https://azure.microsoft.com/updates?id=568514)
2027년 2월부터 예약 환전 서비스 종료, Savings Plan 대상 리소스 적용. 각 예약 건당 최종 한 번의 환전 가능.

---

## 총평 및 다음 달 전망

2026년 7월 Azure는 AI 도입 확대, 멀티리전 인프라 및 데이터 관리 표준화, 보안/네트워킹 혁신, 관리 자동화까지 균형 있게 진화하였습니다.  
특히 AI 모델 서빙, Foundry 플랫폼, Fabric과의 통합 등 데이터·분석 중심 신기능은 글로벌 대기업, 중소기업 모두에게 즉각적인 경쟁우위와 기술적 신뢰를 제공할 것입니다.  
보안·컴플라이언스 강화, 런타임 최신화 및 지역 확장 정책은 하반기에도 지속될 전망이며, 다음 달에는 Fabric 및 AI 분석 플랫폼의 확대와 Azure 서비스 통합, 하이브리드 클라우드 관리 고도화, 신규 보안 정책 추가 등 클라우드 기반 디지털 트랜스포메이션의 가속화가 예상됩니다.