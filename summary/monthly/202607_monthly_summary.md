# Azure 월간 업데이트 요약 - 2026년 07월

## 전반적 트렌드 및 핵심 인사이트

2026년 7월의 Azure 업데이트는 하이브리드, 멀티클라우드, AI, 자동화, 보안, 거버넌스 등 광범위한 영역에서의 혁신이 두드러지는 한 달이었습니다. 특히 최신 인공지능 모델(Microsoft Foundry 및 Azure Databricks 기반 모델 포함)의 지원 확대와 AI 기반 워크로드를 위한 인프라 최적화, 데이터 및 네트워크 보안 강화, 글로벌 리전 확장, 관리 효율성 제고, 그리고 중요한 마이그레이션·모듈 관리 기능들과 클라우드 서비스 운영 표준화에 대한 새로운 시도들이 두드러집니다.

AI 분야에서는 Azure Databricks와 Foundry를 중심으로 Claude Opus 5 및 GPT-5.6 등 첨단 AI 모델 서빙, AI 게이트웨이(미리 보기), AI 텔레메트리 보호 등 실무적·보안적 요구에 부합하는 기능이 추가되었습니다. 데이터 보안 측면에선 클라이언트 단 블롭 암호화, 파일 및 Event Hubs의 암호화, Azure Enclave 등 엄격한 보안 환경 구축을 지원하는 업데이트들이 마이크로서비스, 데이터 저장소, 네트워크 전체에 걸쳐 정식 지원이 확대되었습니다.

운영 및 거버넌스 분야에서는 Kubernetes Fleet Manager, Chaos Studio, Azure Automation, Site Recovery, Storage Migration 등 대규모, 멀티 리전 시나리오에 대응하는 자동화, 복구, 관리 기능이 크게 향상되었습니다. 다양한 SDK 및 PowerShell 모듈의 업데이트, 운영 환경의 지원 종료 정책(파이썬/파워셸 레거시 버전)으로 클라우드 솔루션의 현대화와 보안 강화가 강조되었습니다.

글로벌 리전 확장은 인도 South Central, 칠레 Central 등 신규 리전의 개설 및 Azure Database, OpenShift 등의 배치 지원이 이루어져, 데이터 주권, 레이턴시 개선, 규제 대응 등 산업별 클라우드 도입의 폭이 더욱 넓어졌습니다.

전반적으로 Azure는 인공지능, 하이브리드 클라우드, 멀티 리전, 보안 및 관리 효율성 중심으로 빠르게 진화하고 있으며, AI가 엔터프라이즈 업무 및 인프라의 핵심 요소로 자리잡고 있음을 보여줍니다. 앞으로도 서비스 간 연계, 정책 및 자동화 표준화, 보안/컴플라이언스, 멀티클라우드 데이터 이동성, AI와 네이티브 인프라 협업 등 복잡성이 높은 시나리오에 대한 해결책이 지속적으로 요구될 전망입니다.

---

## 1️⃣ 컴퓨트 & 컨테이너

이번 달 컴퓨트 및 컨테이너 영역에서는 애플리케이션 라우팅의 표준화, 함수형 컴퓨팅 언어 지원, 대규모 Kubernetes 관리 자동화가 주요 이슈입니다.

- [Application Routing with Gateway API](https://azure.microsoft.com/updates?id=567944)  
  AKS에서 Gateway API를 활용한 애플리케이션 라우팅이 정식 지원되어, 서비스 메쉬 없이 Kubernetes 표준 기반 인그레스 관리가 가능해졌습니다.
- [Azure Functions support for Python 3.14](https://azure.microsoft.com/updates?id=567646)  
  Python 3.14 지원으로 장기적인 보안, 성능 개선 및 최신 함수 개발 환경이 제공됩니다.
- [Resource placement in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567931)  
  여러 Kubernetes 클러스터에 리소스를 분산·적용할 수 있도록 간소화된 API와 UI가 제공되어 대규모 AKS 관리가 용이해졌습니다.
- [Encryption in Transit for Azure Files NFS Shares in AKS](https://azure.microsoft.com/updates?id=567787)  
  AKS에서 파일 공유 통신 암호화가 정식 지원되며, TLS 기반 전송 암호화로 보안·컴플라이언스 요구를 충족합니다.
- [Public Preview: Prepared Image Specification](https://azure.microsoft.com/updates?id=567949)  
  AKS 노드 이미지 사전 구성으로 빠른 스케일링, AI/GPU 워크로드 최적화, 운영 효율성이 미리 보기로 제공됩니다.

### 카테고리 요약
컨테이너 플랫폼의 표준화와 자동화, 운영 효율성 제고, 언어/이미지 최신화, 데이터 보안 향상에 중점을 둔 업데이트가 핵심입니다. AKS의 다양한 보안·운영 개선과 Functions/컨테이너의 언어, 이미지 지원 확대가 대규모 분산/복잡한 워크로드에도 안정적 인프라를 제공하는 방향으로 발전하고 있습니다.

---

## 2️⃣ 데이터베이스 & 분석

이번 달에는 AI와 분석 시나리오, 데이터베이스 보안 및 관리 효율성, 멀티리전 지원이 강조되었습니다.

- [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)  
  자동 스케일 및 서버리스 분석 환경이 영국 West 리전에 정식 지원되어 엔터프라이즈 빅데이터 분석이 더욱 원활해졌습니다.
- [Azure Database for PostgreSQL flexible server in India South Central](https://azure.microsoft.com/updates?id=568334)  
  인도 South Central 리전에 PostgreSQL flexible server 지원 확대로 신흥시장에 클라우드 기반 데이터베이스 도입이 쉬워졌습니다.
- [Microsoft Defender 보안 평가 for PostgreSQL Flexible Server](https://azure.microsoft.com/updates?id=567527)  
  PostgreSQL 서버의 보안 상태를 지속 자동 평가·모니터링하여 컴플라이언스 및 보안 리스크 관리가 향상되었습니다.
- [New Powershell module: Az.PostgreSQLFlexibleServer](https://azure.microsoft.com/updates?id=566209)  
  PostgreSQL 18, 탄력적 클러스터 등 최신 기능을 관리할 수 있는 PowerShell 모듈이 출시되어 관리 효율이 크게 개선되었습니다.
- [Azure Databricks Claude Opus 5 지원](https://azure.microsoft.com/updates?id=568316)  
  첨단 AI 모델(Anthropic Claude Opus 5, Sonnet 5 등)을 Databricks에서 데이터 분석과 전문 AI 활용 목적으로 정식 지원합니다.

### 카테고리 요약
서버리스/자동화 분석, 데이터베이스 클라우드 확장, AI 모델 서빙, 데이터 보안 컴플라이언스 기능들이 통합되어, 분석과 운영의 경계가 더욱 유연하게 변화하고 있습니다. PostgreSQL 등 데이터베이스 관련 모듈의 관리 자동화, 리전 확장, AI 모델의 데이터 활용성 증대로 엔터프라이즈 데이터 인프라의 혁신이 가속화되는 경향을 보입니다.

---

## 3️⃣ 스토리지 & 마이그레이션

스토리지와 데이터 마이그레이션 분야에서는 보안, 클라이언트 SDK 기능, 외부 클라우드에서 Azure로의 데이터 이동성, 운영 효율성이 주요 이슈였습니다.

- [Client-side data integrity protections in Azure Blob Storage](https://azure.microsoft.com/updates?id=566895)  
  CRC64-NVME가 SDK에 통합되어 애플리케이션 단에서 데이터 무결성 검증이 가능해졌으며, 엔드투엔드 보안이 강화됐습니다.
- [Azure Storage Mover: GCS to Azure Blob Storage migration 지원](https://azure.microsoft.com/updates?id=566948)  
  GCS 데이터의 에이전트리스 마이그레이션 및 네트워크 격리(Private Link) 활용이 가능하여 멀티클라우드 통합이 간소화되었습니다.
- [Microsoft Entra ID 기반 Blob Storage SFTP 접속 지원](https://azure.microsoft.com/updates?id=567085)  
  SFTP 사용자 관리의 자동화, Entra ID 기반 인증 및 조건부 접근 정책이 도입되어 외부 협업 및 온보딩이 단순화되었습니다.
- [Azure Disk Storage: Instant Access via application consistent restore points](https://azure.microsoft.com/updates?id=565758)  
  VM 복구 시점을 즉시 디스크로 복원하여 빠른 RTO 및 안정적인 복구가 미리 보기로 도입되었습니다.
- [Azure NetApp Files: SMB Oplocks 설정 지원](https://azure.microsoft.com/updates?id=568396)  
  SMB 볼륨의 캐싱 성능 제고, 볼륨별 Oplocks 설정 및 원격 복제 볼륨의 독립적 설정 지원이 발표되었습니다.

### 카테고리 요약
스토리지 신뢰성과 관리 편의성, 클라우드 간 마이그레이션 표준화, 접근통제 강화 및 복구 시간 단축이 중심입니다. SDK 기반 보안 검증, 네트워크 분리/암호화, 다중 볼륨 설정, 자동화된 복구 기능 등 대용량, 멀티클라우드 환경에서의 안정성과 유연성이 크게 개선되었습니다.

---

## 4️⃣ 네트워크 & 보안

네트워크와 보안은 대규모 환경에서의 규제, 응대 효율성, 세분화 정책이 강조되어, 데이터 및 애플리케이션 보호가 주요 초점이었습니다.

- [Azure Firewall: HTTP header insertion](https://azure.microsoft.com/updates?id=568115)  
  HTTP 헤더 삽입 기능으로 엔터프라이즈 액세스 정책, 인증·접근 통제, Microsoft Entra 연동 등 시나리오에 유연하게 대응합니다.
- [IPv6 support for Azure VPN Gateway](https://azure.microsoft.com/updates?id=567847)  
  듀얼 스택 VPN을 통한 IPv6 워크로드 지원으로 멀티넷 환경에서의 네트워크 확장성과 미래 준비가 강화됐습니다.
- [StandardV2 NAT Gateway: NAT64 지원](https://azure.microsoft.com/updates?id=568409)  
  IPv6/IPv4 혼합 환경 네트워크 번역을 지원하여 클라우드 네이티브 애플리케이션·레거시 인터넷 대상 간 통합이 용이해졌습니다.
- [Azure DDoS Protection custom policy 미리 보기](https://azure.microsoft.com/updates?id=568063)  
  트래픽별 맞춤 DDoS 완화 정책 설정이 가능하여 대규모 워크로드 상황에 맞는 보안 대응이 유연하게 적용됩니다.
- [Azure Front Door edge actions 미리 보기](https://azure.microsoft.com/updates?id=567402)  
  프론트 도어 엣지에서 JavaScript 함수 실행, 실시간 요청 처리 및 보안·성능 조정이 가능합니다.

### 카테고리 요약
네트워크 자원의 세분화, 보안 정책의 맞춤화, IPv6/IPv4 통합, 애플리케이션 보안 유연성과 운영 자동화가 핵심입니다. DDoS/파이어월/프론트 도어 정책 등 대규모 환경에서 실무적, 보안적 요구가 융합되고, API·SDK 지원 등 플랫폼화가 강화되었습니다.

---

## 5️⃣ 관리 & 거버넌스

운영 자동화, 거버넌스, 복구 시나리오, 지원 종료 등 관리 효율성과 현대화가 주요 이슈입니다.

- [Azure Automation PowerShell 7.6 지원 정식화](https://azure.microsoft.com/updates?id=568102)  
  최신 PowerShell 및 Azure CLI 실행 환경으로 보안·성능·이식성이 대폭 향상되었습니다.
- [Azure Site Recovery: 5x churn 지원](https://azure.microsoft.com/updates?id=566966)  
  대규모 고속 IOPS 워크로드 복구가 가능해져 미션 크리티컬 애플리케이션 요구에 부합합니다.
- [Azure Chaos Studio: Workspaces & Scenarios 미리 보기](https://azure.microsoft.com/updates?id=567184)  
  사전 구성된 장애 시나리오 테스트, 리소스 자동 탐지, 컴플라이언스 리포트 등 실무 중심의 운영 자동화가 도입됐습니다.
- [Retirement: Python 2.7, 3.8, PowerShell 7.1, 7.2 지원 종료 안내](https://azure.microsoft.com/updates?id=567556)  
  구버전 러untime 미지원에 따라 보안 유지 및 최신 기능 확보를 위해 업그레이드가 반드시 필요합니다.
- [Reservation exchanges for Azure services 종료 안내](https://azure.microsoft.com/updates?id=568514)  
  Savings plan 적용 서비스는 2027년 2월부터 예약 교환이 중단되며, 교환 정책 변경에 대한 대비가 요구됩니다.

### 카테고리 요약
운영 자동화, 장애 복구, 정책 관리, 장기 데이터 보존, 지원 종료 및 정책 변경에 대한 공식화가 핵심입니다. 최신 오케스트레이션 도구, 클라우드 복구, 런타임 관리 표준화, 운영 정책 변화에 대한 빠른 대응이 엔터프라이즈 환경의 안정성을 강화합니다.

---

## 6️⃣ AI + 머신러닝 / Microsoft Foundry

AI 관련, 특히 Microsoft Foundry를 기반으로 하는 기능 확장 및 엔터프라이즈 전체에서 AI 워크로드와 거버넌스 연동이 많이 발표되었습니다.

- [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)  
  툴박스 정식 지원으로 AI 에이전트 개발팀이 공통·재사용 가능한 도구 세트를 쉽게 관리·통제할 수 있게 되었습니다.
- [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)  
  문서 기반 PII 탐지 샘플 경험이 정식 지원되어, 컴플라이언스·보호 업무를 빠르고 쉽게 설계할 수 있습니다.
- [Open AI GPT-5.6 on Azure Databricks (Microsoft Foundry 통합)](https://azure.microsoft.com/updates?id=567431)  
  Foundry에서 구매한 최신 GPT 모델을 Databricks에서 서빙할 수 있어, AI 서비스와 데이터 분석이 통합됩니다.
- [Protect sensitive generative AI telemetry in Application Insights and Microsoft Foundry 미리 보기](https://azure.microsoft.com/updates?id=567594)  
  Foundry 및 Application Insights에서 생성형 AI 데이터에 대한 접근통제 및 민감 정보 보호 기능이 미리 보기로 도입되었습니다.
- [Public Preview: Document PII playground sample in Microsoft Foundry NextGen](https://azure.microsoft.com/updates?id=563331)  
  Foundry NextGen 포털에서 문서 PII 탐지 샘플을 빠르게 평가·비교할 수 있는 미리 보기 기능이 발표되었습니다.

### 카테고리 요약
Microsoft Foundry 및 Databricks 기반 AI 모델 서빙, 도구 관리 표준화, AI 목적의 데이터 보호 및 거버넌스 강화, 컴플라이언스·보안 중심 AI 환경조성이 주요 업데이트입니다. 조직 내 AI 활용 확대에 따라 표준화된 개발·운영 환경, 데이터 보호, 엔터프라이즈 통제 정책 등이 필수적으로 적용되고 있습니다.

---

## 7️⃣ 미리 보기 및 DevOps / Microsoft Fabric

DevOps, 서비스 연동, 신규 기능(미리 보기), Microsoft Fabric 연계 및 관리 자동화가 주요 이슈입니다.

- [AI Gateway in Azure API Management 미리 보기](https://azure.microsoft.com/updates?id=568184)  
  AI 모델(Microsoft Foundry 등)을 API 형태로 안전하게 운영할 수 있는 AI Gateway가 미리 보기로 출시되었습니다.
- [Azure Monitor Logs mirroring into Microsoft Fabric 미리 보기](https://azure.microsoft.com/updates?id=568322)  
  Fabric OneLake 미러링을 통해 Azure Log 데이터와 비즈니스 데이터를 통합 분석, AI·트렌드 분석이 가능합니다.
- [Export historical data from Log Analytics workspace with Export jobs 미리 보기](https://azure.microsoft.com/updates?id=566591)  
  로그 데이터를 원하는 기간·쿼리 기준으로 내보내기 지원, 외부 시스템·분석·컴플라이언스 목적에 활용할 수 있습니다.
- [Manage Azure Chaos Studio from the Azure CLI 미리 보기](https://azure.microsoft.com/updates?id=567225)  
  Azure CLI를 통한 Chaos Studio 시나리오 관리로 운영 자동화 및 확장성이 크게 향상되었습니다.
- [Exceptions in WAF for Application Gateway/Front Door 미리 보기](https://azure.microsoft.com/updates?id=567218)  
  WAF 예외정책 기능 도입으로 실무 환경에 맞는 정교한 보안 정책 적용이 가능해졌습니다.

### 카테고리 요약
DevOps, 모니터링, 서비스 간 연계, Fabric 기반 데이터 연동, API 관리 및 자동화 도구의 강화, 보안 정책 맞춤화 등 클라우드 네이티브 운영과 AI 연계에 기반한 데이터·API 거버넌스, 관리 자동화의 진화가 두드러집니다.

---

## 총평 및 다음 달 전망

2026년 7월은 AI와 멀티클라우드, 자동화·운영 효율성, 보안 강화를 중심으로 Azure 플랫폼의 전방위적 혁신이 확인된 시기였습니다. Microsoft Foundry와 Databricks 연계, 인도·칠레 등 신규 리전 확장, AKS/Kubernetes 중심 분산 애플리케이션 관리 표준화 등이 엔터프라이즈 클라우드 전환·운영 비용 절감·규제 대응에 큰 의미를 부여합니다. 엔터프라이즈 내 AI 활용과 데이터 보호 병행, 구버전 런타임 지원 종료을 통한 현대화 전략, 멀티클라우드 데이터 마이그레이션 및 복구 표준화, 글로벌 네트워크·보안 세분화 등이 서비스별로 가속화되고 있습니다.

다음 달에는 Microsoft Fabric 및 Foundry 연동, 보안 및 컴플라이언스 기능의 더욱 통합적인 오퍼링, 멀티클라우드 워크로드에 대한 자동화·최적화, AI 모델 관리·운영 표준화, 클라우드-온프레미스 데이터 이동·분산 환경 제어 기능 등이 더욱 강화될 것으로 기대됩니다. AI와 분산 리소스 관리, 데이터 보호, 자동화 도구의 표준화는 여전히 Azure의 지속적 혁신을 견인할 핵심 축이 될 것입니다.