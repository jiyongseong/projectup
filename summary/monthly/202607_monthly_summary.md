# Azure 월간 업데이트 요약 - 2026년 07월

## 전반적 트렌드와 핵심 인사이트

2026년 7월의 Azure 업데이트는 클라우드 인프라의 현대화, AI 및 데이터 분석의 확장, 보안과 거버넌스의 강화, 개발자 생산성 및 멀티클라우드 지원 등 전방위 혁신이 두드러졌습니다. 특히 **지역 확장**과 **네트워크 보안**이 지속적으로 강조되며, 인도, 칠레 등 신규 데이터센터 오픈, 다양한 네트워크 서비스의 IPv6, NAT64 등 신기능 출시가 주목받았습니다. AI 및 데이터 분석 분야에서는 Anthropic Claude 모델, OpenAI GPT-5.6 등 최신 LLM(GPT, Claude Sonnet, Opus)의 **Azure Databricks** 연동이 강화되어 엔터프라이즈 AI 도입이 대폭 확대되었습니다. 문서 기반 PII 판단, 데이터 이동, 클라이언트 데이터 무결성 검증과 같은 기능은 실무자 활용성을 높이고, Microsoft Foundry의 Toolboxes, Playground처럼 **AI 에이전트 개발 및 거버넌스** 강화가 눈에 띕니다.

업데이트에는 Python, PowerShell, .NET, C++, JavaScript 등 **다양한 오픈 소스 언어의 최신 버전 적용/지원 종료**, 그리고 Azure Functions, Automation, Kubernetes 관련 기능 확장 및 관리 자동화가 강조되며, 개발자와 관리자들의 생산성 향상을 위한 서비스 개선이 활발합니다. 또한 Azure Blob Storage, NetApp Files, Azure Files, SFTP, Site Recovery 등 **스토리지 및 데이터 이동/복구** 기술이 보안·관리 측면에서 진화되고, Azure Firewall, DDoS Protection, Key Vault 프리미엄 영역에서 **네트워크, 보안, 암호화** 기술이 고도화되고 있습니다.

미리 보기(preview) 기능으로는 AI Gateway, Chaos Studio Workspace/Scenario, Azure Enclave, Azure Monitor Fabric 미러링 등 차세대 관리 및 거버넌스 솔루션이 등장했고, 개선된 네트워크 격리, 서비스 엔드포인트, 데이터 보호 정책이 클라우드 상의 **엔터프라이즈급 신뢰성** 확보에 도움을 주고 있습니다. 마지막으로 Azure 관리 정책의 변경(Reservation 교환 정책, 런타임 지원 종료 등)은 클라우드 비용 최적화 및 보안 유지에 있어 적극적인 업그레이드와 준비가 요구됩니다.

---

## 1. 🚀 신규 서비스 및 지역 확장

2026년 7월에는 Azure 클라우드의 글로벌 확장과 신기능 출시가 두드러졌습니다. 신규 지역 데이터센터 오픈으로 인도 남부, 칠레 등 로컬 서비스 강화와, AKS, Azure Red Hat OpenShift, Databricks 등 주요 서비스의 지역 지원 확대가 클라우드 인프라의 접근성과 신뢰성을 강화하고 있습니다. 신규 기능 출시(정식 지원)에서는 Kubernetes Gateway API, Azure Automation의 PowerShell 7.6 런북, Python 3.14 지원, Sphere OS 신버전 등 최신 기술을 바로 사용할 수 있게 되었습니다.

### [Application Routing with Gateway API](https://azure.microsoft.com/updates?id=567944)
AKS에서 최신 Kubernetes Gateway API 기반의 Ingress 관리 정식 지원. 기존 ingress-nginx에서 점진적 마이그레이션 가능.

### [Azure Automation PowerShell 7.6 런북 및 런타임 환경 지원](https://azure.microsoft.com/updates?id=568102)
최신 PowerShell 7.6 기반 런북과 런타임 환경 정식 지원, Azure CLI 명령 연동, 스크립트 호환성 및 관리 효율성이 대폭 향상.

### [Azure Databricks SQL Serverless UK West 지원](https://azure.microsoft.com/updates?id=567444)
UK West 지역에서 Databricks SQL Serverless 가용, 자동 확장 및 관리 효율성 강화로 분석 워크로드 민첩성 제공.

### [Azure Functions: Python 3.14 지원](https://azure.microsoft.com/updates?id=567646)
Azure Functions에서 Python 3.14를 지원, 보안 개선 및 개발 도구와의 완벽한 호환성 확보.

### [Azure Sphere OS 26.09 평가판 출시](https://azure.microsoft.com/updates?id=568466)
장기 지원 및 보안 강화된 Sphere OS 신버전, Linux 커널 버전 업그레이드로 IoT 디바이스 통합성 및 보안성 강화.

---

## 2. 📈 AI 및 데이터 분석

데이터와 AI 분석 분야에서는 Azure Databricks에 OpenAI GPT-5.6, Claude Sonnet 5, Opus 5 등이 정식 지원되어 엔터프라이즈 고도 AI 적용이 쉽게 이뤄집니다. Azure AI Language의 문서 PII 진단, Event Hubs의 기밀 컴퓨팅 등은 데이터 보호와 AI 활용 확장에 힘을 더합니다.

### [Claude Opus 5 on Azure Databricks](https://azure.microsoft.com/updates?id=568316)
최신 AI 모델인 Claude Opus 5를 Databricks 환경에서 지원, 복잡한 추론과 전문적 개발에 적합한 AI 기반 앱 개발 가능.

### [Anthropic Claude Sonnet 5 지원](https://azure.microsoft.com/updates?id=567194)
Cost 효율성과 속도 모두를 가진 Claude Sonnet 5, 전문 업무와 코드 자동화에 맞는 하이브리드 모델을 Databricks에서 활용.

### [Open AI GPT-5.6 on Azure Databricks](https://azure.microsoft.com/updates?id=567431)
Azure Databricks에서 GPT-5.6 정식 지원, Microsoft Foundry 기반 AI 모델을 안전하게 서비스 가능.

### [Client-side data integrity protections in Azure Blob Storage](https://azure.microsoft.com/updates?id=566895)
Blob Storage 클라이언트 SDK에서 CRC64-NVME 체크섬 지원. 응용 단계부터 Azure 물리적 스토리지까지 완전 무결성 검증.

### [Confidential Computing for Azure Event Hubs Dedicated](https://azure.microsoft.com/updates?id=567212)
Event Hubs Dedicated 환경에 기밀 컴퓨팅 적용, TEE 기반 메모리 보호로 Streaming 데이터 수집 시 보안·컴플라이언스 완벽 지원.

---

## 3. 🛡️ 네트워킹 및 보안

Azure 네트워크와 보안 서비스는 IPv6, NAT64, DDoS Protection, Firewall, Key Vault 등 최신 트렌드를 반영하며, 네트워크 격리, 보안 정책, 클라우드 암호화 등의 엔터프라이즈 요구를 충족시킵니다.

### [HTTP header insertion in Azure Firewall](https://azure.microsoft.com/updates?id=568115)
Azure Firewall에서 HTTP/HTTPS 헤더 삽입 지원, 보안 제어 및 SaaS 접근 제어, 텐턴트 제한 등 네이티브 헤더 관리.

### [IPv6 지원 for Azure VPN Gateway](https://azure.microsoft.com/updates?id=567847)
Dual-stack 환경에서 IPv4와 IPv6 트래픽을 투명하게 지원, 브랜치/지사, 원격 사용자, Site-to-Site/Point-to-Site VPN 통합.

### [NAT64 on StandardV2 NAT Gateway](https://azure.microsoft.com/updates?id=568409)
NAT64 지원으로 IPv6 워크로드가 IPv4-only 인터넷 타깃과 통신 가능, DNS64-capable resolver 통한 트래픽 변환 자동화.

### [Network Security Perimeter for Azure Event Hubs](https://azure.microsoft.com/updates?id=567203)
Event Hubs에서 NSP 적용, PaaS 자원에 논리적 네트워크 격리, 공용 네트워크 접근 제어 가능. 데이터 유출 위험 최소화.

### [Symmetric keys on Azure Key Vault Premium](https://azure.microsoft.com/updates?id=566746)
Key Vault 프리미엄에서 대칭키(AES, oct-HSM) 관리 및 암호화 기능 미리 보기 지원, CNSA 2.0 기준 충족 및 포스트퀀텀 대비.

---

## 4. 💼 관리/거버넌스/마이그레이션

운영 자동화, 클라우드 거버넌스, 데이터 마이그레이션 등 관리 효율성 증대를 위한 모듈·서비스가 출시되었습니다. PowerShell·Python 런타임 지원 종료 정책, Site Recovery 성능 개선, Storage Mover의 GCS 지원, 예약 교환 정책 변경 등은 관리자의 변화 대응을 필요로 합니다.

### [Azure Automation: 런타임 지원 종료 안내](https://azure.microsoft.com/updates?id=567556)
2026년 9월 30일부터 Python 2.7, 3.8 및 PowerShell 7.1, 7.2 자동화 런타임 지원 종료 예정. 빠른 업그레이드 권고.

### [Azure Site Recovery: 5x churn 지원](https://azure.microsoft.com/updates?id=566966)
VM당 최대 500MB/s의 IOPS 복구 지원, 대용량 워크로드도 안정적으로 DR 수행 가능.

### [Azure Storage Mover: GCS → Azure Blob 통합 지원](https://azure.microsoft.com/updates?id=566948)
GCS에서 Azure Blob으로 완전 자동화된 마이그레이션 지원. 엔터프라이즈 멀티클라우드 데이터 이동과 보안성 강화.

### [Reservation exchanges 정책 변경](https://azure.microsoft.com/updates?id=568514)
2027년 2월 1일부터 Savings Plan 적용 서비스(Compute, DB 등)에서는 예약 교환이 더 이상 불가. 기존 예약은 한 차례 최종 교환 가능.

### [Export historical data from Log Analytics workspace](https://azure.microsoft.com/updates?id=566591)
Log Analytics의 Export jobs로 과거 데이터 추출 지원, 컴플라이언스·감사·보안 조사에 활용성 극대화.

---

## 5. ⚡ 컨테이너/Kubernetes/스토리지

Kubernetes, OpenShift, Fleet Manager 등 컨테이너 관리의 자동화, 지역 확장, 서비스 확장 및 스토리지의 복구, 데이터 이동, 네트워크적 보호 기능이 빠르게 발전하고 있습니다.

### [Resource placement in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567931)
Fleet Manager에서 다수의 AKS/Arc 클러스터에 대해 일관적 리소스 배포, 관리 정책 자동화, 오류 방지 정책 확장.

### [Azure Red Hat OpenShift 칠레 센트럴 가용](https://azure.microsoft.com/updates?id=566732)
남미 지역 최초 칠레 센트럴에서 OpenShift 완전관리 클러스터 지원, 지연 감소와 데이터 레지던시 준수 가능.

### [Encryption in Transit for Azure Files NFS Shares in AKS](https://azure.microsoft.com/updates?id=567787)
AKS에서 Azure Files NFS 볼륨에 대한 전송 중 데이터 암호화 지원, TLS 기반 보안성 대폭 강화.

### [Azure Kubernetes Fleet Manager: 업데이트 실패 허용 기준 미리 보기](https://azure.microsoft.com/updates?id=567939)
Fleet Manager에서 업데이트 실패 허용 임계값 설정 가능, 대규모 클러스터 롤아웃 시 유연한 관리 전략 적용.

### [Prepared Image Specification for AKS(미리 보기)](https://azure.microsoft.com/updates?id=567949)
AKS에 컨테이너 및 커스텀 이미지 사전 포함 노드를 생성하여 노드 시작시간 단축, AI·GPU 워크로드 최적화.

---

## 6. 🧰 Microsoft Foundry & AI 에이전트 생태계

Foundry에서는 Toolboxes의 정식 지원과 Playground 미리 보기, 데이터 보호·거버넌스 기능 등 조직 단위 AI 에이전트의 개발, 관리, 보안 강화를 위한 혁신이 이어졌습니다.

### [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)
AI 에이전트 개발에 필요한 MCP 서버, REST API, 스킬 등을 하나의 엔드포인트로 호출·관리, 거버넌스 표준화.

### [Document PII playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)
실시간 PII 진단 Playground 정식 지원, 팀·기관 단위 PII 프로젝트 즉시 실험 가능, 컴플라이언스 강화.

### [Protect sensitive gen AI telemetry in Application Insights/Foundry](https://azure.microsoft.com/updates?id=567594)
Application Insights의 GenAIContent 테이블 및 Foundry에 민감한 AI 텔레메트리 접근 제어 기능 내장, PII/PHI 관리에 최적화.

### [Public Preview: Document PII Playground Sample in Foundry NextGen](https://azure.microsoft.com/updates?id=563331)
Foundry NextGen 포털에서 향상된 PII 샘플 Playground 제공, 비동기 파일 파이프라인 미리 평가 가능.

### [AI Gateway in Azure API Management(미리 보기)](https://azure.microsoft.com/updates?id=568184)
Foundry, AWS, Google, OpenAI 등 다양한 AI 자산을 일관된 게이트웨이로 노출, 인증·정책·관찰성·연동성을 강화.

---

## 7. 🧩 미리 보기(Preview) 기능 및 차세대 솔루션

이번 달에는 AI Gateway, Chaos Studio Workspace/Scenario, Azure Enclave, Azure Monitor Fabric 미러링, DDoS Protection 커스텀 정책 등 미리 보기 기능이 다양하게 출시되어 차세대 클라우드 관리와 거버넌스를 준비할 수 있었습니다.

### [Azure Chaos Studio: Workspace & Scenario(미리 보기)](https://azure.microsoft.com/updates?id=567184)
실무적 장애 시나리오 및 워크플로우 자동 생성, Azure RBAC에 의한 권한 제어, DORA 등 컴플라이언스 테스트 지원.

### [Azure Enclave(미리 보기)](https://azure.microsoft.com/updates?id=568377)
보안이 중요한 정부/규제 환경에 격리된 영역(Enclave) 자동 관리/배포, 네트워크 세분화, 역할·접근 제어 강화.

### [Azure Monitor Logs mirroring to Microsoft Fabric(미리 보기)](https://azure.microsoft.com/updates?id=568322)
Azure Monitor Log 데이터 실시간 복제, OneLake 및 Eventhouse, Power BI, Spark 등 Fabric 분석과의 통합 확대.

### [Azure DDoS Protection custom policy(미리 보기)](https://azure.microsoft.com/updates?id=568063)
DDoS 방어 임계값을 자원별 직접 설정, 유연한 보호 정책 구현 및 인바운드 트래픽 세분화 관리.

### [Azure Front Door edge actions(미리 보기)](https://azure.microsoft.com/updates?id=567402)
Azure Front Door의 서버리스 Edge 액션, A/B 테스트, 헤더 조작, 인증, URL 리라이트 등 실시간 엣지 연산 기능 제공.

---

## 총평 및 다음 달 전망

2026년 7월 Azure 클라우드 업데이트는 **AI 중심 혁신**과 **엔터프라이즈 보안/관리**를 양축으로 삼아, 글로벌 확장과 개발자의 생산성 증대, 민감 정보 보호, 네트워크 격리, 데이터 신뢰성, 거버넌스 자동화 등이 폭넓게 실현된 월이었습니다. Python, PowerShell 등 주요 언어의 지원 종료 정책은 보안·업데이트에 대한 사용자 책임을 강조하며, 신규 지역과 멀티클라우드 마이그레이션 지원은 확실한 시장 확장 전략을 보여주었습니다.

특히 Microsoft Foundry, AI Gateway, Databricks와 같은 차세대 AI 및 데이터 중심 구조는 엔터프라이즈 환경에 맞춰 지속적으로 진화하고 있으며, 실무적 자동화, 스케일링, 장애 대응(Chaos Studio), 거버넌스, 컴플라이언스 강화로 클라우드 내재 역량이 한층 높아졌습니다.

다음 달에는 Fabric, Foundry, AI Gateway, Enclave 등 preview 기능의 GA(정식 지원) 전환 가능성, Azure Functions 및 AKS의 신버전 기능 확대, Kubernetes 관리 자동화, 네트워크/스토리지 보안 정책 고도화, 그리고 클라우드 비용 최적화 방안(Reservation/Savings Plan 정책 등)의 추가 안내가 기대됩니다. Azure 고객은 변화에 적극적으로 대응하며 최신 기능을 활용할 준비가 필요합니다.