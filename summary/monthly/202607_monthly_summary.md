# Azure 월간 업데이트 요약 - 2026년 07월

## 전반적 트렌드 및 핵심 인사이트

2026년 7월 Azure 업데이트는 클라우드 인프라 표준화와 컴플라이언스, AI와 데이터 분석 강화, 서비스 간 통합 및 관리 자동화, 네트워크·보안 영역의 혁신 등 여러 측면에서 의미 있는 진전을 보여줍니다. 특히 Kubernetes 관련 기능과 AKS(애저 쿠버네티스 서비스) 관리 툴이 더욱 친환경적이고 표준화된 API로 전환되고, Databricks-Foundry 연계, AI 모델 서빙 신제품 등 데이터 및 AI 플랫폼의 확장성이 돋보입니다. 클라우드 네이티브 서비스의 지역적 확장과 보안 프레임워크의 진화(예: Confidential Computing, 네트워크 보안 경계, Entra ID SFTP 연계)는 글로벌 기업뿐 아니라 규제가 엄격한 산업군(금융, 공공, 의료)에서도 Azure 도입을 가속화할 계기를 마련합니다.

운영 자동화와 DevOps 영역에서는 PowerShell, Python 등 런타임 지원이 최신 버전으로 확대되며, 은퇴 정책 안내와 함께 모듈 관리 편의성이 강조되었습니다. 네트워크 인프라 혁신, 인공지능 API 게이트웨이, DDoS 개인화 정책, Front Door 엣지 액션 등 네트워크/보안 레이어에서의 다양성도 두드러지는 시점입니다. 데이터 및 스토리지 자산의 관리 강화와 로그/이력 데이터의 Fabric 연계(통합 분석과 AI 기반 의사결정 지원), 클라우드 간 스토리지 마이그레이션의 자동화 강화 등 멀티 클라우드 시대 대응이 본격화되고 있습니다.

Microsoft Foundry와 Microsoft Fabric의 기능 및 API 개방성, 전사적 AI & 데이터 거버넌스, 실시간 분석 플랫폼 연결성 등 대기업·엔터프라이즈 시장을 노린 마이크로소프트의 전략도 더욱 구체화되었으며, 그와 동시에 서비스 지역 다양화(인도, 칠레 등 신규 리전), 컴플라이언스 기능 확대, 머신러닝 자동화 및 도구의 표준화 노력도 뚜렷하게 나타납니다. 이번 달 업데이트는 클라우드 인프라와 애플리케이션 관리의 표준화 및 거버넌스 강화, AI·데이터 플랫폼의 신뢰성과 확장성, 네트워크와 보안의 세분화와 자동화가 조화를 이루며, 전통적인 기업 IT와 현대적 AI 컴퓨팅이 융합되는 흐름을 보여줍니다.

---

## 1. 컴퓨트, 컨테이너, 운영 자동화

컴퓨트와 컨테이너 파트는 AKS의 표준화된 ingress 라우팅(Gateway API 도입), Python 3.14, PowerShell 7.6 등의 최신 언어 런타임 지원 확대가 핵심입니다. Kubernetes Fleet Manager의 리소스 배치 및 update failure threshold 정책 도입, AKS Prepared Image Specification 미리 보기 등 대규모 환경의 관리 효율과 안정성을 강화하는 방향으로 발전했습니다. 운영 자동화에서는 최신 PowerShell 및 Azure CLI 연계를 통한 스크립트 실행 환경의 개편이 두드러집니다.

- [Application Routing with Gateway API](https://azure.microsoft.com/updates?id=567944)  
  AKS에서 Gateway API 기반의 ingress 관리가 정식 지원되어 서비스 Mesh 없이 현대적인 라우팅 모델을 도입할 수 있습니다.

- [Azure Automation supports PowerShell 7.6 runbooks and Runtime environment](https://azure.microsoft.com/updates?id=568102)  
  PowerShell 7.6 런북 및 Runtime 환경이 정식 지원되어 스크립트 업그레이드와 실행 환경 경쟁력이 향상되었습니다.

- [Azure Functions support for Python 3.14](https://azure.microsoft.com/updates?id=567646)  
  Azure Functions에서 Python 3.14 지원으로 보안 강화, 지원 기간 확대 등 최신 언어 특성을 적용할 수 있습니다.

- [Resource placement in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567931)  
  Kubernetes Fleet Manager에서 리소스 배치 기능이 정식 지원되어 다중 클러스터 관리 편의성이 개선되었습니다.

- [Maximum allowed failures for update runs in Azure Kubernetes Fleet Manager (미리 보기)](https://azure.microsoft.com/updates?id=567939)  
  그룹별 업데이트 실패 임계값을 설정해 대규모 배포시 유연성을 확보할 수 있습니다.

---

## 2. 데이터 플랫폼, AI & 머신러닝, 분석

Azure Databricks에서는 Claude Opus 5, Claude Sonnet 5, OpenAI GPT-5.6 등 최신 대형 언어모델이 차례로 도입되어 AI 모델 서빙 역량이 대폭 강화되었습니다. SQL 서버리스 방식 확장, 이벤트 허브의 Confidential Computing 및 NSP(Network Security Perimeter) 지원 등 데이터 보호와 네트워크 격리 기술이 결합되며, AI 분석을 위한 PII 탐지 샘플 Playground도 Foundry 및 Language 서비스에서 전사적 활용이 가능해졌습니다.

- [Claude Opus 5 on Azure Databricks](https://azure.microsoft.com/updates?id=568316)  
  고도화된 클로드 모델을 Azure Databricks의 AI 서빙 연계로 엔터프라이즈 데이터 기반 AI 앱 구현을 지원합니다.

- [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)  
  분석 워크로드의 서버리스화로 데이터 활용의 즉시성, 자동 확장, 인프라 관리 최소화를 실현했습니다.

- [Confidential Computing support for Azure Event Hubs Dedicated](https://azure.microsoft.com/updates?id=567212)  
  신뢰 실행 환경(TEE)을 통한 이벤트 스트리밍 데이터의 인메모리 보호가 가능해져 민감 정보 처리에 적합합니다.

- [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)  
  문서 기반 PII 탐지 Playground가 정식 지원되어 컴플라이언스·보호팀이 손쉽게 테스트 및 적용할 수 있습니다.

- [Open AI GPT-5.6 on Azure Databricks](https://azure.microsoft.com/updates?id=567431)  
  최신 대형 언어 모델을 Databricks와 Foundry 통합으로 보안·거버넌스 연계 AI 앱 개발이 한층 강화됩니다.

---

## 3. 네트워크, 보안, 스토리지

클라우드 네트워크 영역에서는 NAT64, VPN Gateway IPv6, Azure Firewall의 HTTP 헤더 인서션, DDoS 개인화 정책 등 IPv6/IPv4 듀얼 스택, 보안 제어 세분화 및 확장성이 도드라집니다. Blob Storage의 클라이언트 측 데이터 무결성, SFTP Entra ID 도입, AKS NFS 데이터 암호화 등 데이터 보안이 핵심입니다. Key Vault Premium의 대칭키(오프-HSM, AES 256) 미리 보기에서는 중앙화된 키 관리와 정책 강화가 주요 포인트입니다.

- [HTTP header insertion in Azure Firewall](https://azure.microsoft.com/updates?id=568115)  
  Azure Firewall에서 HTTP/HTTPS 헤더 삽입이 지원되어 애플리케이션 제어와 클라우드 기반 인증, 보안 정책 적용이 간소화되었습니다.

- [IPv6 support for Azure VPN Gateway](https://azure.microsoft.com/updates?id=567847)  
  듀얼 스택 지원으로 온프레미스-클라우드 간 IPv6 기반 VPN 통신이 가능해졌습니다.

- [NAT64 on StandardV2 NAT Gateway](https://azure.microsoft.com/updates?id=568409)  
  IPv6 워크로드가 NAT64를 통해 IPv4-only 대상과 통신할 수 있는 변환 서비스가 추가되었습니다.

- [Client-side data integrity protections in Azure Blob Storage](https://azure.microsoft.com/updates?id=566895)  
  CRC64-NVME 체크섬 방식으로 클라이언트부터 Blob Storage까지 엔드-투-엔드 데이터 무결성 검증이 가능해졌습니다.

- [Symmetric keys on Azure Key Vault Premium (미리 보기)](https://azure.microsoft.com/updates?id=566746)  
  AES 기반 대칭키 관리가 Key Vault Premium에서 미리 보기로 제공되어 보안 및 컴플라이언스 요건 충족이 용이해집니다.

---

## 4. 지역 및 데이터센터 확장

이번 달에는 인도 South Central과 칠레 Central 리전의 신규 오픈, PostgreSQL Flexible 서버의 인도 South Central 확장 등 글로벌 인프라의 지역 다변화가 이어졌습니다. 해당 리전에서 AI, 데이터베이스, OpenShift 등 핵심 서비스가 빠르게 확장되고 있어 현지 데이터 레지던시·지연속도·컴플라이언스 요구에 대응하는 Azure의 시장 확대 전략이 뚜렷합니다.

- [Microsoft Azure now available from new cloud region in India (India South Central)](https://azure.microsoft.com/updates?id=568013)  
  인도 내 네 번째 데이터센터 리전 오픈으로 AI 인프라, 데이터 보호, 지역컴플라이언스 요구를 충족합니다.

- [Azure Database for PostgreSQL flexible server in India South Central](https://azure.microsoft.com/updates?id=568334)  
  인도 South Central 리전에서 PostgreSQL Flexible 서버 배포가 가능해져 현지 데이터베이스 운영 탄력성이 확보됩니다.

- [Azure Red Hat OpenShift in Chile Central](https://azure.microsoft.com/updates?id=566732)  
  칠레 Central 리전에서 OpenShift 정식 지원으로 남미 지역 클라우드 네이티브 확장속도가 빨라지고 있습니다.

- [New Powershell module: Az.PostgreSQLFlexibleServer](https://azure.microsoft.com/updates?id=566209)  
  PowerShell 모듈 리팩토링 및 인도 South Central 등 확장 리전의 최신 API 연계 지원이 향상되었습니다.

- [Support 5x churn in Azure Site Recovery](https://azure.microsoft.com/updates?id=566966)  
  고속 데이터 변동량(최대 500MB/s per VM) 지원으로 재해복구 서비스의 글로벌 활용성이 더욱 강화됐습니다.

---

## 5. Microsoft Foundry

Microsoft Foundry에서는 AI 기반 툴박스(통합 툴 API 및 거버넌스), Document PII Playground 샘플, 애플리케이션 인사이트의 AI 텔레메트리 보호 등 조직 내 AI·데이터 거버넌스 강화, 도구 표준화, 다양한 데이터 보호 기능이 한층 진화했습니다. 개발 및 운영팀의 도구 공유, 정책 일관화, 데이터 안전한 활용에 큰 도움이 될 전망입니다.

- [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)  
  통합된 MCP형 툴박스 제공으로 조직 내 AI 도구 활용의 일관성과 정책 거버넨스가 크게 강화됩니다.

- [Document PII playground sample in Microsoft Foundry NextGen](https://azure.microsoft.com/updates?id=563331)  
  내장 샘플 기반 PII Playground가 제공되어 AI Language의 실시간 문서 탐지 및 평가가 한층 쉬워집니다.

- [Protect sensitive generative AI telemetry in Application Insights and Microsoft Foundry (미리 보기)](https://azure.microsoft.com/updates?id=567594)  
  AI 텔레메트리 데이터를 분리 저장 및 역할 기반 접근제어로 민감 정보 관리가 가능해졌습니다.

- [AI Gateway in Azure API Management (미리 보기)](https://azure.microsoft.com/updates?id=568184)  
  Foundry·AWS·Google 모델에 대한 게이트웨이 보호 단일화로 조직별 AI 자산 관리와 거버넌스가 한층 강화됩니다.

- [Open AI GPT-5.6 on Azure Databricks](https://azure.microsoft.com/updates?id=567431)  
  Foundry에서 구매한 GPT-5.6 모델을 Databricks Model Serving에서 안전하게 연동할 수 있습니다.

---

## 6. Microsoft Fabric 및 DevOps, 통합 관리

Fabric에서는 Azure Monitor Log Analytics 데이터의 OneLake 거버넌스·실시간 분석 연계, 로그 Export Jobs, AI 텔레메트리 분리 관리, Chaos Studio CLI 연동 등 데이터·운영·보안 전반의 자동화가 활성화되고 있습니다. DevOps, 관리 도구와 API 통합, Fabric·AI·핵심 워크로드간 데이터 운영의 실시간성 강조가 특징입니다.

- [Azure Monitor Logs mirroring into Microsoft Fabric (미리 보기)](https://azure.microsoft.com/updates?id=568322)  
  실시간 Telemetry를 Fabric OneLake에 델타 파케이 형식으로 자동 연계, 범분야 데이터 분석이 지원됩니다.

- [Export historical data from Log Analytics workspace with Export jobs (미리 보기)](https://azure.microsoft.com/updates?id=566591)  
  이력 로그 데이터를 지정 쿼리, 기간별로 추출하여 외부 시스템/장기 저장으로 활용성이 확대되었습니다.

- [Manage Azure Chaos Studio from the Azure CLI (미리 보기)](https://azure.microsoft.com/updates?id=567225)  
  Chaos Studio 시나리오를 CLI에서 빠르게 구성/검증/실행 가능하며, 운영 자동화가 강화되었습니다.

- [Prepared Image Specification (미리 보기)](https://azure.microsoft.com/updates?id=567949)  
  AKS용 맞춤 node 이미지 설계로 대규모 AI·GPU·Windows 워크로드의 빠른 확장성을 확보할 수 있습니다.

- [Instant Access via application consistent restore points (미리 보기)](https://azure.microsoft.com/updates?id=565758)  
  VM 디스크 복구 시 즉시 접근 기능으로 RTO 단축, 복구 신뢰도·유연성 확보가 가능합니다.

---

## 7. 공지, 정책 및 지원 종료

Azure의 서비스 정책 변경 및 런타임 버전 은퇴/교체, 예약 교환 정책 변경 등 장기적 IT 전략 수립에 필수적인 안내가 포함되었습니다. Python 2.7, 3.8, PowerShell 7.1/7.2 은퇴, 최신 모듈 및 스크립트 업그레이드 체계 안내 등 안전성과 컴플라이언스 관점의 플랫폼 진화 방향을 제시하고 있습니다.

- [Support for Python-2.7; 3.8 and PowerShell- 7.1; 7.2 will be retired on September 30, 2026](https://azure.microsoft.com/updates?id=567556)  
  2026년 9월 30일 이후 해당 구 버전 런타임 지원이 중단되므로 최신 버전 업그레이드가 권장됩니다.

- [Announcing: Reservation exchanges for Azure services supported by savings plans will no longer be available starting February 1, 2027](https://azure.microsoft.com/updates?id=568514)  
  2027년 2월 1일부터 Savings Plans 커버리지 리전·서비스에 예약 교환 기능이 제한됩니다.

- [Azure Automation supports PowerShell 7.6 runbooks and Runtime environment](https://azure.microsoft.com/updates?id=568102)  
  최신 PowerShell 및 Azure CLI 런북 환경의 업그레이드, 지원 및 모듈 관리 정책이 정립되었습니다.

- [New Powershell module: Az.PostgreSQLFlexibleServer](https://azure.microsoft.com/updates?id=566209)  
  PostgreSQL API 및 PowerShell 모듈의 최신화로 관리 효율과 향후 변화 대응력이 강화됩니다.

- [Azure DDoS Protection custom policy (미리 보기)](https://azure.microsoft.com/updates?id=568063)  
  DDoS 차단 정책을 서비스별/리전별로 세분화할 수 있게 안내되었습니다.

---

## 총평 및 다음달 전망

2026년 7월 Azure 업데이트는 현대적 클라우드 아키텍처의 표준화, AI·데이터 분석 플랫폼의 확장, 네트워크와 보안의 세밀화 및 컴플라이언스 강화에 초점을 두고 있습니다. 글로벌 서비스 지역 확장과 AI 모델 연계, 데이터 보호와 자동화 관리 툴의 세련된 진화가 돋보입니다. 조직 내 데이터의 실시간 분석 및 거버넌스, 네트워크·스토리지·운영 자동화 기반의 표준 모델 구축이 대기업과 다양한 산업군에 Azure 도입의 실질적 가치를 제공하고 있습니다.

다음 달에는 Foundry·Fabric 연계, 다양한 AI 모델 및 데이터 서비스 확장, 네트워크·보안 서비스의 자동화·개인화 정책 확대 등 다방면에서 Azure 클라우드 기술의 혁신이 지속될 전망입니다. 특히 AI 거버넌스 기능, 멀티 클라우드 통합 관리 경험, 컴플라이언스 기능의 확대와 신규 리전 및 워크로드 최적화 방안이 주요 화두가 될 것으로 예상됩니다.