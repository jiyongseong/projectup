# Azure 월간 업데이트 요약 - 2026년 07월

## 전반적인 트렌드와 핵심 인사이트

2026년 7월 Azure 업데이트는 인프라 확장, 보안 및 거버넌스 강화, AI 및 데이터 분석 혁신, 운영 효율화, 개발 환경의 최신화 등 여러 측면에서 균형 있게 이루어졌습니다.  
먼저, 인도 South Central, 영국 West, 칠레 Central 등 다양한 지역에서 Azure 서비스가 정식 지원되며 글로벌 리전 확장 트렌드가 지속되고 있습니다. 전 세계에 배포하는 비즈니스 요구에 맞춘 높은 데이터 레지던시, 낮은 레이턴시, 고가용성 실현 노력은 계속 강화되고 있습니다.

보안과 컴플라이언스 영역에서는 네트워크 보안 경계(NSP), Confidential Computing, Azure Enclave, Key Vault Premium 대칭키, Azure Firewall HTTP 헤더 삽입 등 데이터 및 네트워크 보호의 폭이 넓어지고 있습니다. 특히 개인정보 탐지와 보안 모니터링 툴의 정식 지원과 미리보기 출시가 활발하며, 규제 산업에 대응하는 새로운 기능들이 연속적으로 공개되는 모습입니다.

AI와 데이터 분석 부문은 Anthropic Claude Sonnet 5, Claude Opus 5, GPT-5.6 등 최신 대형 AI 모델의 Azure Databricks 통합, AI Gateway 미리 보기, Microsoft Foundry 기반 툴박스와 PII Playground 제공 등 혁신적 기능이 속속 추가되고 있습니다. Fabric과 Azure Monitor 연동으로 데이터 통합 분석의 폭이 넓어지고 있고, SFTP 및 Blob Storage SDK 개선처럼 전통적인 데이터 관리 방식에도 지속적 혁신이 적용되고 있습니다.

운영/관리 영역에서는 Azure Chaos Studio 시나리오 및 CLI 확장, Site Recovery 고IOPS 지원, 리소스 배치 자동화, 인스턴트 VM 복구 등 빠른 장애 복구 및 규모 확장, 적응형 관리 기능이 강조되고 있습니다.  
개발환경 측면에서는 PowerShell 7.6, Python 3.14 등 최신 언어 지원과 Azure Kubernetes Fleet Manager, Prepared Image Specification 등 개발 경험 개선, 프로덕션 환경의 신속한 변화 대응력을 높이는 다양한 기능이 정식 지원 또는 미리보기로 출시되었습니다.

전체적으로 Azure는 지역 기반 성장, AI/데이터 분석 혁신, 보안/운영 효율화에 중점을 두어 다양한 고객 요구와 산업별 규제를 포괄적으로 지원하는 모습을 보여주고 있습니다. 앞으로 AI 활용 확장, 데이터 통합, 네트워크/스토리지 보안 강화 트렌드가 지속될 것으로 예상되며, 미리 보기 단계의 기능들이 조만간 정식 서비스로 이어질 전망입니다.

---

## 🖥️ 컴퓨트, 컨테이너, 인터넷 오브 씽스

전통적 클라우드 컴퓨트 및 컨테이너 기반 서비스의 기능 고도화와 최신 런타임 지원이 주요 트렌드입니다. AKS Gateway API 도입, Azure Functions Python 3.14 및 PowerShell 7.6 공식 지원부터 Prepared Image Specification 미리 보기까지, 성능, 보안, 개발 경험 개선을 위한 혁신이 주목받고 있습니다.

### [Application Routing with Gateway API](https://azure.microsoft.com/updates?id=567944)  
AKS에서 Gateway API 기반 애플리케이션 라우팅이 정식 지원되어 최신 쿠버네티스 표준을 적용하면서 서비스 메쉬 없이도 경량화된 인그레스 관리가 가능해졌습니다.

### [Azure Functions support for Python 3.14](https://azure.microsoft.com/updates?id=567646)  
Azure Functions가 Python 3.14를 정식 지원, 보안성과 긴 지원 기간, 최신 개발 도구 호환성을 제공합니다.

### [Azure Automation supports PowerShell 7.6 runbooks and Runtime environment](https://azure.microsoft.com/updates?id=568102)  
PowerShell 7.6 런북 및 런타임 환경이 정식 지원되며, 구버전 스크립트 손쉽게 최신 환경으로 업그레이드할 수 있게 되어 코드 조직 및 모듈 충돌 문제도 해결됩니다.

### [Resource placement in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567931)  
Azure Kubernetes Fleet Manager의 리소스 배치 기능이 정식 지원되어 여러 AKS와 Arc 클러스터에 일관성 있게 리소스 배포가 가능합니다.

### [Prepared Image Specification (미리 보기)](https://azure.microsoft.com/updates?id=567949)  
AKS 노드 이미지를 사전 준비된 컨테이너 이미지와 커스텀 설정으로 구성해, 대규모/고성능 AI 및 GPU 워크로드에 매우 빠른 스케일아웃과 초기화 효율성을 제공합니다.

---

## 💾 스토리지, 데이터베이스, 네트워크

스토리지와 데이터베이스, 네트워크 영역에서는 성능 및 보안, 관리 편의성에 초점을 맞춘 기능이 다수 정식 지원되었습니다. Blob Storage 데이터 무결성, Azure Files 암호화 전송, NAT64, VPN Gateway IPv6 등 전반적인 인프라 품질과 호환성 개선이 돋보입니다.

### [Client-side data integrity protections in Azure Blob Storage](https://azure.microsoft.com/updates?id=566895)  
Blob Storage SDK(.NET, C++, JavaScript)에서 CRC64-NVME 기반의 클라이언트-서버간 데이터 무결성 검증이 가능해져, 애플리케이션 계층부터 물리적 스토리지까지 완전한 데이터 보호가 실현됩니다.

### [Encryption in Transit for Azure Files NFS Shares in AKS](https://azure.microsoft.com/updates?id=567787)  
AKS 내 Azure Files NFS v4.1 볼륨에 대해 TLS 기반 암호화 전송 지원이 정식화되어 높은 보안 요구 환경에서 마운트 데이터의 전송 안전성을 제공합니다.

### [IPv6 support for Azure VPN Gateway](https://azure.microsoft.com/updates?id=567847)  
Azure VPN Gateway에서 IPv6 트래픽 지원을 시작, 듀얼스택 구성을 통해 IPv4/IPv6 혼합 워크로드 및 온프레미스 네트워크와의 연동이 가능해졌습니다.

### [NAT64 on StandardV2 NAT Gateway](https://azure.microsoft.com/updates?id=568409)  
StandardV2 NAT Gateway에서 NAT64 지원으로 IPv6 워크로드가 IPv4만 지원하는 외부 리소스와 원활히 통신할 수 있습니다.

### [Support for SMB Opportunistic Locking (Oplocks) configuration (미리 보기)](https://azure.microsoft.com/updates?id=568396)  
Azure NetApp Files의 SMB 및 듀얼프로토콜 볼륨에 대해 Oplocks 설정 지원이 미리 보기로 출시되어 클라이언트 캐싱 성능 및 고가용성 관리가 향상됩니다.

---

## 🤖 AI 및 머신러닝, 데이터 분석, Azure Databricks

Azure Databricks 중심으로 다양한 최신 AI 모델 지원, 모델 서비스 통합, 데이터 분석 처리의 혁신이 집중적으로 이루어지고 있습니다. 각 모델별 활용성과 데이터 관리 효율화를 높이는 기능이 잇달아 정식 지원되어 엔터프라이즈 AI 활용도를 높이고 있습니다.

### [Claude Opus 5 on Azure Databricks](https://azure.microsoft.com/updates?id=568316)  
Anthropic Claude Opus 5 모델이 AI Model Serving으로 지원되어 고도 추론 및 복잡한 전문 업무 자동화가 가능합니다.

### [Open AI GPT-5.6 on Azure Databricks](https://azure.microsoft.com/updates?id=567431)  
Microsoft Foundry 구매 모델인 GPT-5.6을 Azure Databricks Model Serving Endpoint에서 활용, 데이터 거버넌스와 통합 관리가 가능해졌습니다.

### [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)  
영국 West 리전에서 Databricks SQL Serverless가 정식 지원되어 즉시 컴퓨트, 자동 스케일링, 인프라 관리 효율화가 실현됩니다.

### [Generally available: Anthropic Claude Sonnet 5 on Azure Databricks](https://azure.microsoft.com/updates?id=567194)  
Claude Sonnet 5 모델이 Databricks에 정식 지원, 엔터프라이즈급 코드 생성 및 AI 워크플로우 구축이 더욱 강화되었습니다.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)  
PII 탐지 Playground가 빠른 샘플 평가 및 다양한 엔티티 지원으로 정식 출시, 데이터 보호 및 컴플라이언스 팀의 실무 효율이 대폭 개선됩니다.

---

## 🔒 보안, 네트워킹, 컴플라이언스

보안 강화와 컴플라이언스 지원이 핵심 화두입니다. Confidential Computing, Azure Enclave, Key Vault Premium, DDoS Protection, Azure Firewall 등 다양한 레이어에서 업무별 맞춤 보안 정책, 네트워크 경계, 암호화 기능이 확장되고 있습니다.

### [Confidential Computing support for Azure Event Hubs Dedicated](https://azure.microsoft.com/updates?id=567212)  
이벤트 허브 전용 환경에서 Confidential Computing이 정식 지원되어 메모리 내 데이터까지 하드웨어 기반 TEE로 안전하게 보호합니다.

### [HTTP header insertion in Azure Firewall](https://azure.microsoft.com/updates?id=568115)  
Azure Firewall에서 HTTP/HTTPS 헤더 삽입 기능이 도입되어, Entra 테넌트 제한, VDI, SaaS 접근 제어 등 보안과 운영 효율을 높일 수 있습니다.

### [Azure DDoS Protection custom policy (미리 보기)](https://azure.microsoft.com/updates?id=568063)  
리소스별 DDoS 탐지 임계값을 미리 지정할 수 있는 커스텀 정책이 공개되어, 대형/이벤트 성 트래픽에 맞춰 보안 정책 세부 조정이 가능해졌습니다.

### [Azure Enclave (미리 보기)](https://azure.microsoft.com/updates?id=568377)  
정부 및 규제 산업 대상의 고립 환경을 신속하게 배포/관리할 수 있는 Azure Enclave가 미리 보기로 출시되어 네트워크 분리, 접근 정책, 모니터링을 강화합니다.

### [Symmetric keys on Azure Key Vault Premium (미리 보기)](https://azure.microsoft.com/updates?id=566746)  
Key Vault Premium에서 대칭키(AES) 관리 기능이 확장되어 고수준 CNSA 2.0 호환 암호화, 중앙화된 키관리 실현이 가능합니다.

---

## 🔧 관리, 거버넌스, 마이그레이션, 운영

운영 및 관리의 효율성, 신속한 장애 복구, 데이터 이동 및 거버넌스 강화가 두드러진 달이었습니다. Site Recovery 고IOPS, Automation 업데이트, Chaos Studio 시나리오 미리 보기, Storage Mover 클라우드 간 데이터 이동 등 엔터프라이즈 환경에 실질적 도움이 되는 기능 개선이 이어졌습니다.

### [Azure Automation supports PowerShell 7.6 runbooks and Runtime environment](https://azure.microsoft.com/updates?id=568102)  
Automation 런북 및 환경 레벨의 최신화 지원으로 코드 호환성, 관리 편의성, 보안성을 대폭 높였습니다.

### [Support 5x churn in Azure Site Recovery](https://azure.microsoft.com/updates?id=566966)  
Site Recovery가 초고IOPS(VM별 500MB/s) 지원을 시작, 대형 데이터베이스 및 빅데이터 시스템도 안정적 DR 환경을 구현할 수 있게 됐습니다.

### [Azure Chaos Studio Workspaces and Scenarios (미리 보기)](https://azure.microsoft.com/updates?id=567184)  
Chaos Studio에서 워크스페이스/시나리오 기반 실시간 장애 테스트 자동화가 가능해지고, Compliance(DORA 등) 보고서 생성까지 지원합니다.

### [Azure Storage Mover now supports migration from Google Cloud Storage (GCS) (미리 보기)](https://azure.microsoft.com/updates?id=566948)  
클라우드 간(구글→Azure) 데이터 마이그레이션 지원이 추가되어 멀티클라우드 통합 및 네트워크 분리 환경에서도 쉽고 안전한 대규모 데이터 이전이 가능해졌습니다.

### [Export historical data from Log Analytics workspace with Export jobs (미리 보기)](https://azure.microsoft.com/updates?id=566591)  
Log Analytics 공간의 지정 쿼리/기간 데이터를 외부 스토리지로 내보낼 수 있어 규제 준수, 보안 분석, BI, 머신러닝 데이터 활용성을 확대합니다.

---

## 🏗️ Microsoft Foundry 및 Microsoft Fabric

Foundry는 AI 활용과 거버넌스, 개발 생산성 강화를 위한 조직 표준화 도구와 Playground 경험을 제공하며, Fabric은 데이터 모니터링 및 통합 분석 기능을 늘려 조직별 데이터 연계 강화에 집중하고 있습니다.

### [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)  
툴박스 기능이 정식 지원되며, 프롬프트 에이전트 및 다양한 조직 내 AI 도구를 중앙화된 MCP 호환 엔드포인트로 호출, 거버넌스 일관성을 확보했습니다.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)  
PII Playground가 공식 지원, 샘플 문서로 개인 정보 탐지 평가를 신속히 수행할 수 있어 컴플라이언스 업무를 획기적으로 단축합니다.

### [Public Preview: Document PII playground sample in Microsoft Foundry NextGen](https://azure.microsoft.com/updates?id=563331)  
Foundry NextGen 포털에서 PII playground가 미리보기 제공, 소스/결과를 비교하며 API 연동 전 평가가 가능합니다.

### [Protect sensitive generative AI telemetry in Application Insights and Microsoft Foundry (미리 보기)](https://azure.microsoft.com/updates?id=567594)  
GenAIContent 테이블 및 Log Analytics 연동으로 AI 텔레메트리 보호 강화, 다양한 데이터 접근 제한 정책을 적용할 수 있습니다.

### [AI Gateway in Azure API Management (미리 보기)](https://azure.microsoft.com/updates?id=568184)  
Foundry, AWS, GCP, OpenAI 등 AI 자산을 보안 정책/관찰 가능성 일관화된 게이트웨이로 관리하며 멀티클라우드 AI 활용의 통합 경험을 제공합니다.

---

## 🌏 글로벌 리전 및 인프라 확장 (한국 리전 포함)

세계 각지에서 데이터센터 신규 개설, 서비스 리전 확대 등이 이루어지는 모습이 두드러집니다. (한국 리전 신규 뉴스는 이번 달 포함되지 않았으나, Azure의 전반적인 글로벌 확장 트렌드는 계속되고 있습니다.)

### [Microsoft Azure now available from new cloud region in India (India South Central)](https://azure.microsoft.com/updates?id=568013)  
인도 South Central 리전 신설로 AI 준비형 인프라, 데이터 레지던시, 저지연, 대용량 확장 등 지역 내 디지털 전환 수요에 적극 대응합니다.

### [Azure Database for PostgreSQL flexible server in India South Central](https://azure.microsoft.com/updates?id=568334)  
PostgreSQL 플렉서블 서버가 인도 South Central에서 정식 지원되어 신규 리전의 데이터베이스 기능 활용범위가 넓어졌습니다.

### [Azure Red Hat OpenShift in Chile Central](https://azure.microsoft.com/updates?id=566732)  
칠레 Central 리전에서 OpenShift(ARO)가 정식 지원되어 현지 데이터 주권 및 규제 산업 대응 클라우드 환경이 강화되었습니다.

### [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)  
영국 West 리전에서 Databricks SQL Serverless가 정식 지원되어 지역별 데이터 분석 인프라 효율이 높아졌습니다.

### [Azure Database for PostgreSQL Flexible Server 보안 평가 지원](https://azure.microsoft.com/updates?id=567527)  
Microsoft Defender의 CSPM 평가 기능이 정식 지원, PostgreSQL 환경의 보안 상태 평가와 컴플라이언스 확인이 더욱 쉬워졌습니다.

---

## 총평 및 다음 달 전망

2026년 7월 Azure 업데이트는 글로벌 인프라 확장, AI 및 데이터 분석 혁신, 보안과 관리 효율화의 세 축이 뚜렷하게 나타난 달입니다. AKS, Databricks, Foundry, Site Recovery, Blob Storage 등 다양한 서비스가 최신 기능을 정식 지원 또는 미리 보기로 출시하며, 개발, 운영, 보안 각 분야의 생산성 및 신뢰성을 한층 높였습니다.  

특히 대형 AI 모델의 신속한 도입, 대규모 멀티클라우드 데이터 관리, 국가별 규제 대응 및 네트워크/스토리지 보안 강화가 두드러집니다. 향후에도 리전별 서비스 확대, AI 및 정보보호 트렌드, 멀티클라우드 데이터 관리와 거버넌스 기술 발전에 주목할 필요가 있습니다.  
다음 달에는 미리 보기 기능의 정식 출시에 따른 고객 경험 변화, AI Gateway 확장, Foundry/Fabric 활용 범위 증가 등 Azure의 포괄적 혁신이 지속될 것으로 예상됩니다.