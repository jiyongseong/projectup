# Azure 월간 업데이트 요약 - 2026년 07월

## 전반적인 트렌드 및 핵심 인사이트

2026년 7월의 Azure 업데이트는 보안, 네트워킹, AI, 데이터 관리의 다각화된 발전을 중심으로 공공, 기업, 금융, 헬스케어 등 다양한 산업에서 요구되는 클라우드 환경의 최적화를 보여줍니다. 이번 달에는 다수의 정식 지원(General Availability)이 발표되며 Azure 플랫폼의 신뢰성과 확장성이 한 단계 더 강화됐습니다.

특히 AI 및 머신러닝 분야에서는 Azure Databricks에 Anthropic Claude Sonnet 5, Opus 5, OpenAI GPT-5.6 모델 등 첨단 AI 모델이 정식 지원되고, Microsoft Foundry 기반의 엔터프라이즈 AI 개발 도구가 대폭 확대되었습니다. Container 및 Kubernetes 서비스 부문에서는 Gateway API와 Resource Placement 기능 도입으로 멀티클러스터 및 서비스 메쉬 없이도 유연하고 보안성이 강화된 서비스 관리가 가능합니다.

보안과 네트워킹 영역에서는 Azure Firewall Manager의 HTTP 헤더 삽입, NAT64 지원, IPv6 통합, DDoS Protection 커스텀 정책 등 고도화된 서비스가 확장되었으며, Confidential Computing, Network Security Perimeter 등 데이터와 네트워크의 안전성과 준수성에서 글로벌 표준에 부합하는 혁신이 두드러집니다.

관리 및 거버넌스 분야는 Azure Automation의 PowerShell 7.6, Azure Chaos Studio의 Workspaces·Scenario 기능, Site Recovery의 처리 성능 개선 등 현업의 효율성을 높이는 실질적 기능 업그레이드가 이뤄졌습니다. 신규 지역 확장(인도 South Central 등)도 대거 이뤄져 글로벌 데이터 거점의 다양화와 지역 맞춤형 클라우드 전략이 강화되고 있습니다.

또한, 사용 중단(retirement) 및 정책 변화 공지(예약 교환 제한 등)도 포함되어 고객이 더 빠른 환경 업그레이드와 보안 유지에 대응할 수 있도록 안내하고 있습니다. 미리 보기(Preview) 기능은 실제 운영 적용 전 실험적 활용 기회를 제공하며, 곧 더 많은 서비스의 일반 지원으로 이어질 전망입니다. 이번 달 Azure는 서비스의 범위, 심도, 안정성 측면에서 균형 잡힌 성장과 미래 지향적 혁신을 함께 주도하고 있습니다.

---

## 1. ☁️ 컴퓨팅 및 컨테이너

이번 달 컴퓨팅 및 컨테이너 부문에서는 Kubernetes 서비스의 게이트웨이 API 정식 지원, Azure Functions의 Python 3.14 및 PowerShell 7.6 지원, Fleet Manager 및 AKS에서 멀티클러스터 운영 강화 등이 주요 트렌드입니다. 서버리스와 관리형 플랫폼을 통한 자동화, 보안 강화, 확장성 개선이 돋보이며 클라우드 네이티브 환경에서의 다양한 최신 언어 지원도 주목받고 있습니다.

### [Application Routing with Gateway API](https://azure.microsoft.com/updates?id=567944)
AKS상 게이트웨이 API 기반의 애플리케이션 라우팅이 정식 지원되어 기존 인그레스에서 게이트웨이 모델로 단계적 전환이 가능하며, 서비스 메쉬 없이 표준화된 라우팅이 가능해졌습니다.

### [Azure Functions support for Python 3.14](https://azure.microsoft.com/updates?id=567646)
Python 3.14 기반 함수 개발 및 배포가 활성화되어 보안, 지원 기간, 개발 도구의 최신성과 호환성을 확보할 수 있습니다.

### [Public Preview: Azure Functions Support for PowerShell 7.6](https://azure.microsoft.com/updates?id=567651)
PowerShell 7.6을 사용해 로컬 개발·배포가 가능해져, 최신 스크립트와 언어 기능을 Azure Functions에서 활용할 수 있습니다.

### [Resource placement in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567931)
Fleet Manager의 자원 배치 기능 정식 지원으로 여러 AKS 및 ARC 클러스터에 리소스를 일관적으로 배포·관리할 수 있습니다.

### [Maximum allowed failures for update runs in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567939)
업데이트 실패 허용치 지정 미리 보기 기능으로, 일부 클러스터 실패시에도 전체 롤아웃이 지속되어 대규모 클러스터 운영의 유연성이 향상됩니다.

---

## 2. 🔒 보안 및 네트워킹

보안 및 네트워킹 부문에서는 Azure Firewall에서 HTTP 헤더 삽입, VPN Gateway IPv6 확대, Event Hubs의 Confidential Computing, NAT64 지원, 네트워크 격리, DDoS Protection 커스텀 정책 및 Key Vault 프리미엄 대칭키 등 다양한 신기능이 등장했습니다. 보안 관리와 네트워크 트래픽 제어, 인프라 유연성, 준수성 강화에 초점을 맞추고 있습니다.

### [HTTP header insertion in Azure Firewall](https://azure.microsoft.com/updates?id=568115)
Azure Firewall에서 HTTP/S 헤더를 직접 삽입하는 기능이 정식 지원되어, 보안 정책, 테넌트 제한, SaaS 접근제어 등 다양한 시나리오에 활용 가능합니다.

### [IPv6 support for Azure VPN Gateway](https://azure.microsoft.com/updates?id=567847)
VPN Gateway에서 IPv6 내 트래픽 지원이 확대되어, 듀얼스택 모드에서 다양한 워크로드의 네트워크 유연성이 향상됩니다.

### [NAT64 on StandardV2 NAT Gateway](https://azure.microsoft.com/updates?id=568409)
StandardV2 NAT Gateway의 NAT64 지원으로 IPv6 워크로드가 IPv4 전용 인터넷 대상으로 자연스럽게 통신 가능해졌습니다.

### [Azure DDoS Protection custom policy](https://azure.microsoft.com/updates?id=568063)
DDoS Protection에서 커스텀 정책 설정이 가능해져, 트래픽 임계치 설정을 통한 워크로드별 맞춤형 보호가 실현됩니다.

### [Azure Enclave](https://azure.microsoft.com/updates?id=568377)
Azure Enclave 미리 보기 발표로, 네트워크 격리 및 승인된 접속만 허용되는 보안 클라우드 환경 구축이 가능해졌습니다.

---

## 3. 📊 데이터베이스 및 분석(AI 포함)

DB 및 분석 부문은 Azure Databricks와 PostgreSQL, AI 모델 기반 데이터 처리 및 보안 평가 강화, Event Hubs의 네트워크 격리, Document PII 검출 Playground 등 AI와 데이터 관리의 융합이 두드러집니다. 최신 AI 모델 지원, 서버리스 분석 옵션, 보안 평가와 개인 정보 검출까지, 미래형 데이터 거버넌스가 본격화되고 있습니다.

### [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)
UK West 지역에서 Databricks SQL Serverless 운용이 가능해져, 자동 확장 및 인프라 최소화로 비용 효율적 분석 환경이 확대됩니다.

### [Claude Opus 5 on Azure Databricks](https://azure.microsoft.com/updates?id=568316)
Anthropic Claude Opus 5 모델을 Databricks에서 AI Model Serving으로 활용할 수 있게 되어 고도화된 AI 업무 및 엔터프라이즈 데이터 활용이 가능해졌습니다.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)
PII 탐지와 샘플 평가 작업이 정식 지원되어 문서 기반 개인식별정보 검출 서비스의 실효적 적용이 빨라졌습니다.

### [Confidential Computing support for Azure Event Hubs Dedicated](https://azure.microsoft.com/updates?id=567212)
Event Hubs Dedicated에서 Confidential Computing 지원으로, 데이터 사용 시에도 하드웨어 기반 보호가 가능합니다.

### [Microsoft Defender security assessments for Azure Database for PostgreSQL Flexible Server](https://azure.microsoft.com/updates?id=567527)
PostgreSQL Flexible Server의 보안 평가 기능이 강화되어, 지속적 취약점 모니터링과 권장조치 제공에 기반한 안전한 DB 운영이 가능합니다.

---

## 4. 💾 스토리지 및 데이터 이동

스토리지 부문은 Azure Blob Storage의 클라이언트 측 데이터 무결성 검증, SFTP에 Microsoft Entra ID 연동, NFS 암호화, Storage Mover의 GCS→Azure Blob 이동, Azure Disk의 Instant Access 미리 보기 등 데이터의 안전성과 전환 용이성, 효율적 활용 측면에서 큰 발전이 있었습니다.

### [Client-side data integrity protections in Azure Blob Storage](https://azure.microsoft.com/updates?id=566895)
클라이언트 앱에서 Blob Storage에 대한 CRC64-NVME 무결성 검증이 가능해져 데이터 통합성 확인이 더욱 정밀해졌습니다.

### [Microsoft Entra ID-based access for Azure Blob Storage SFTP](https://azure.microsoft.com/updates?id=567085)
SFTP 연결에 Entra ID 및 외부 아이덴티티 기반 인증이 정식 지원, MFA·조건부 접근·RBAC 등으로 보안 및 협업이 강화되었습니다.

### [Encryption in Transit for Azure Files NFS Shares in Azure Kubernetes Service (AKS)](https://azure.microsoft.com/updates?id=567787)
AKS와 Azure Files NFS 볼륨간 데이터 전송 암호화 기능이 제공되어 보안 및 준수성 요구에 대응합니다.

### [Azure Storage Mover now supports migration from Google Cloud Storage (GCS)](https://azure.microsoft.com/updates?id=566948)
GCS에서 Azure Blob Storage로 완전 관리형/무Agent 방식의 안전한 데이터 마이그레이션이 미리 보기로 지원됩니다.

### [Instant Access via application consistent restore points](https://azure.microsoft.com/updates?id=565758)
VM Restore Points 기능의 Instant Access 미리 보기로, 디스크 복구 시 즉시 사용 가능하며 효율적 복구 운용이 가능해집니다.

---

## 5. 🧭 관리 및 거버넌스

관리 및 거버넌스 부문은 Azure Automation의 최신 런타임 지원, Chaos Studio의 Workspaces 및 시나리오 미리 보기, Site Recovery의 큰 성능 향상, Log Analytics Export 및 관리 CLI 확대, 사용 중단 런타임 안내와 예약 교환 정책 변경 등 조직의 운영 효율성과 컴플라이언스 강화가 중심입니다.

### [Azure Automation supports PowerShell 7.6 runbooks and Runtime environment](https://azure.microsoft.com/updates?id=568102)
Azure Automation에서 PowerShell 7.6 런북, 런타임 환경 정식 지원으로 최신 스크립트 관리·이식·보안이 탁월해졌습니다.

### [Azure Chaos Studio Workspaces and Scenarios](https://azure.microsoft.com/updates?id=567184)
Chaos Studio의 Workspaces·Scenario 미리 보기로 복잡한 장애 시나리오 재현 및 애플리케이션 탄력성 평가가 손쉽게 구현됩니다.

### [Export historical data from Log Analytics workspace with Export jobs](https://azure.microsoft.com/updates?id=566591)
Log Analytics Export Job 미리 보기로, 원하는 쿼리·기간 데이터만 추출 및 외부 저장소로 이동할 수 있습니다.

### [Support 5x churn in Azure Site Recovery](https://azure.microsoft.com/updates?id=566966)
Site Recovery의 5배 증가된 처리량으로 높은 IOPS 워크로드의 DR 신뢰성과 대응력이 대폭 향상됐습니다.

### [Support for Python-2.7; 3.8 and PowerShell- 7.1; 7.2 will be retired on September 30, 2026](https://azure.microsoft.com/updates?id=567556)
2026년 9월 30일부터 구런타임 지원 종료 안내, 최신 환경으로 업그레이드 필요성이 강조됩니다.

---

## 6. 🌎 리전 및 인프라(신규 지역 포함)

글로벌 리전 확장 부문에서는 인도 South Central 클라우드 신규 오픈, 해당 리전에서 Azure Database for PostgreSQL Flexible Server 지원 및 ARO(Chile Central)와 같은 지역별 관리형 서비스 확대가 두드러집니다. 각국 데이터 거주 요건, 지연 최소화, 신뢰성 확보가 더욱 강화되고 있습니다.

### [Microsoft Azure now available from new cloud region in India (India South Central)](https://azure.microsoft.com/updates?id=568013)
인도 South Central에 Azure 신규 리전이 오픈되어 현지 AI 클라우드 인프라 및 데이터 레지던시, 저지연 환경이 보장됩니다.

### [Azure Database for PostgreSQL flexible server in India South Central](https://azure.microsoft.com/updates?id=568334)
해당 리전에서 PostgreSQL 서버의 정식 지원으로, 인도 내 DB 배포 옵션이 확대됩니다.

### [Azure Red Hat OpenShift in Chile Central](https://azure.microsoft.com/updates?id=566732)
Chile Central 리전에서 ARO 정식 지원, 남미 지역의 OpenShift 엔터프라이즈 환경이 강화됩니다.

### [Network Security Perimeter support for Azure Event Hubs](https://azure.microsoft.com/updates?id=567203)
Event Hubs의 네트워크 보안 경계(Perimeter) 지원으로 리전별 네트워크 콘트롤 및 격리가 가능합니다.

### [Standard service endpoint](https://azure.microsoft.com/updates?id=561475)
IaaS-PaaS 연결의 Private Link 계열 서비스 엔드포인트 표준화 미리 보기로 대규모 인프라 네트워크 식별·확장성이 향상됩니다.

---

## 7. 🧰 Microsoft Foundry 및 Microsoft Fabric

Foundry/Fabric 부문은 툴박스, 도큐먼트 PII 플레이그라운드, AI Gateway, Fabric 연동 로그 미러링 등 조직 내 AI 및 도구 관리, 보안, 관측 데이터 활용이 혁신적으로 업그레이드됩니다. 플랫폼 일원화, 관리 효율성, 보안 정책 강화가 특징적입니다.

### [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)
Foundry Toolboxes 정식 지원으로, 통합 MCP 엔드포인트를 통한 AI 에이전트 툴 일원화·거버넌스 관리가 가능해집니다.

### [Public Preview: Document PII playground sample in Microsoft Foundry NextGen](https://azure.microsoft.com/updates?id=563331)
PII 검출 샘플 도구 미리 보기, 속도·효율적 검증 기능이 조직 구성원에게 제공됩니다.

### [AI Gateway in Azure API Management](https://azure.microsoft.com/updates?id=568184)
AI Gateway 미리 보기로 Foundry 모델 포함 다양한 AI·MCP 서버 자산을 통합 관리·보안·관찰할 수 있습니다.

### [Azure Monitor Logs mirroring into Microsoft Fabric](https://azure.microsoft.com/updates?id=568322)
Azure Monitor Logs를 Fabric으로 미러링하는 미리 보기 기능으로 실시간 비즈니스·운영 데이터 통합 분석이 가능해집니다.

### [Protect sensitive generative AI telemetry in Application Insights and Microsoft Foundry](https://azure.microsoft.com/updates?id=567594)
Foundry연계 Application Insights에서 민감 AI 텔레메트리의 테이블별 접근 제한 기능이 미리 보기로 제공합니다.

---

## 총평 및 다음 달 전망

2026년 7월의 Azure 업데이트는 서비스의 전방위적 혁신, 신뢰성과 확장성 강화, 보안·관리 효율성 향상에 초점을 맞췄습니다. AI·데이터 분석, 컨테이너, 네트워킹, 관리 자동화 등 모든 영역에서 실질적인 기능 개선이 지속되며, 리전 확장·신규 운영체제·보안 정책 등의 글로벌, 로컬 요구 대응도 적극적으로 이루어지고 있습니다.

특히 미리 보기 기능이 다수 공개되어 조기 실험과 업계 적응 경험이 넓어지고 있으며, 엔터프라이즈 확장, 플랫폼 일원화, 데이터 보안 및 거버넌스가 차기 핵심 트렌드임을 보여줍니다. 다음 달에는 미리 보기 기능의 GA 전환, 신규 AI/데이터 기능, 보안 및 네트워크 정책 강화, 더욱 세분화된 지역 특화 서비스 발표가 기대됩니다. Azure는 편의성과 혁신, 안정성의 균형으로 클라우드 시장 리더십을 굳건히 하고 있습니다.