# Azure 월간 업데이트 요약 - 2026년 07월

## 전반적인 트렌드 및 핵심 인사이트

2026년 7월 Azure 업데이트에서는 AI, 보안, 관리 자동화, 네트워크 신규 기능과 다중 클라우드 및 데이터 레지던시 확장 등 주요 트렌드가 뚜렷하게 나타났습니다. 특히 AI 및 데이터 분석 전용 서비스를 중심으로 정식 지원과 미리 보기 기능이 대거 출시되어, 기업의 디지털 전환과 생산성 향상 노력이 구체화되고 있습니다.

AI와 머신러닝 역량 강화는 Anthropic Claude Opus 5, Claude Sonnet 5, OpenAI GPT-5.6과 같은 최신 모델 지원 확대뿐 아니라, 데이터 보호와 개인정보 탐지 기능, 툴 통합 등 실사용 중심의 AI 서비스 최적화 방향을 보여줍니다. Azure Databricks, Microsoft Foundry, Fabric 등 다양한 AI 및 데이터 플랫폼에서 고급 모델과 신규 기능이 정식 지원되어 실무현장에서 즉시 활용 가능성이 높아졌습니다.

보안과 컴플라이언스 부문의 주요 업데이트에서는 네트워크 격리, 암호화, 엔트라 ID를 통한 SFTP 접근, 클라이언트-서버 간 무결성 검증 강화, Confidential Computing 환경 및 DDoS 방어 정책 등 실제 보안 시나리오에 직접 적용할 수 있는 기능이 두드러집니다. 이와 함께 관리와 자동화 플랫폼에서는 PowerShell 7.6 런북, 고속 범용 복구(5x churn), Chaos Studio 시나리오 등 시스템 안정성과 운영 효율성을 높일 수 있는 관리 도구가 지속적으로 추가되고 있습니다.

운영 및 개발 효율성 측면에서는 Kubernetes 및 컨테이너 관리 기능, 리소스 배치, 업데이트 실패 허용치, 이미지 준비 사양 등 클러스터 관리 자동화와 애플리케이션 현대화 흐름에 맞춰 기능이 최적화되어 엔터프라이즈급 기술 수용성이 확대되고 있습니다.

클라우드 네이티브 데이터 인프라 및 지역 확장 부문에서는 인도 신규 리전 개설, 남미(칠레) OpenShift 클러스터 지원, 다중 클라우드 데이터 이전 등 데이터 레지던시 및 글로벌 커버리지 강화 의지가 읽힙니다. Azure Storage Mover를 통한 GCS 데이터 이동, NetApp Files의 SMB Oplocks 등 멀티클라우드 업무환경에 대응하는 기능도 강화되었습니다.

전반적으로 이번 달은 기존 서비스의 정식 지원 확대와 미리 보기 혁신 기능 추가, 보안·컴플라이언스 강화, AI·데이터 분석 실무 적용 확대, 그리고 지역 및 워크로드 확장이 골고루 반영된 업데이트로 평가할 수 있습니다.

---

## 1️⃣ 컴퓨트, 컨테이너, 서버리스

### [Application Routing with Gateway API](https://azure.microsoft.com/updates?id=567944)
AKS에서 Gateway API 기반의 애플리케이션 라우팅이 정식 지원되어, 인그레스 관리 표준화와 서비스 메시 필요 없이 현대적 인그레스 구조로 점진적 전환이 가능합니다.

### [Azure Functions support for Python 3.14](https://azure.microsoft.com/updates?id=567646)
Azure Functions에서 Python 3.14 지원이 정식 제공되어 강화된 보안, 호환성, 장기 지원 혜택을 누릴 수 있습니다.

### [Public Preview: Azure Functions Support for PowerShell 7.6](https://azure.microsoft.com/updates?id=567651)
PowerShell 7.6 지원이 미리 보기로 제공되어, 최신 스크립트 개발 및 배포의 범용성이 확장되었습니다.

### [Prepared Image Specification](https://azure.microsoft.com/updates?id=567949)
AKS 노드 이미지 사양을 미리 지정할 수 있는 기능이 미리 보기로 추가되어, 확장 및 대규모 배포 시 빠른 노드 초기화와 예측 가능한 성능 확보가 가능합니다.

### [Resource placement in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567931)
Fleet Manager에서 리소스 일괄 배치가 정식 지원되어, AKS와 Arc 클러스터 전체에 일관된 리소스 배포·관리가 자동화됩니다.

**카테고리 요약**  
컨테이너 및 서버리스 기능의 진화는 기본 인그레스 라우팅, 언어별 런타임 지원 확대, 리소스 배치 자동화 등 엔터프라이즈 통합·대규모 현대화 요구에 대응하고 있습니다. Kubernetes 기반 운영 효율성 개선과 앱 개발 유연성 확보가 이번 달 주요 화두입니다.

---

## 2️⃣ 데이터, AI 및 분석

### [Claude Opus 5 on Azure Databricks](https://azure.microsoft.com/updates?id=568316)
Databricks에서 Claude Opus 5 최신 AI 모델이 정식 지원되어 복잡한 추론, 소프트웨어 설계 등 전문 업무에서 활용도가 크게 높아졌습니다.

### [Open AI GPT-5.6 on Azure Databricks](https://azure.microsoft.com/updates?id=567431)
GPT-5.6 신규 지원으로, Foundry와 Databricks 연계 AI 서비스 개발·배포가 가능해져 데이터 기반 인공지능 활용이 극대화됩니다.

### [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)
SQL Serverless가 UK West 리전에서 정식 지원되어 실시간 분석, 자동 스케일링 등 인프라 관리 최소화와 빠른 데이터 처리 환경이 제공됩니다.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)
PII 탐지 테스트 환경이 정식 지원되어, 민감 정보 관리와 컴플라이언스 프로젝트의 효율적 설계와 평가를 지원합니다.

### [Generally available: Anthropic Claude Sonnet 5 on Azure Databricks](https://azure.microsoft.com/updates?id=567194)
Sonnet 5 모델이 Databricks에서 정식 지원되어 비용 효율적이면서 고도화된 코딩 및 에이전트 워크플로우 구현이 가능합니다.

**카테고리 요약**  
AI 모델 지원 확대와 데이터 분석 환경 최적화가 이번 달 데이터 & AI 업데이트의 중심입니다. PII 탐지, SQL Serverless, 최신 대형 모델 도입, 플랫폼 연계 등 실무 적용성과 확장성이 크게 향상되었습니다.

---

## 3️⃣ 스토리지, 네트워크, 보안

### [Client-side data integrity protections in Azure Blob Storage](https://azure.microsoft.com/updates?id=566895)
Blob Storage에서 CRC64-NVME 기반 데이터 무결성 검증이 SDK에서 확장되어, 클라이언트-서버 간 데이터 일관성 보장이 강화되었습니다.

### [Encryption in Transit for Azure Files NFS Shares in AKS](https://azure.microsoft.com/updates?id=567787)
AKS에서 NFS 볼륨 데이터 전송 암호화가 정식 지원되어, TLS 기반 데이터 이동 보안이 단계별로 적용됩니다.

### [HTTP header insertion in Azure Firewall](https://azure.microsoft.com/updates?id=568115)
Firewall에서 HTTP 헤더 삽입 지원으로, 백엔드 서비스 연동·보안 관리 자동화 및 다중 테넌트 정책 적용이 가능합니다.

### [IPv6 support for Azure VPN Gateway](https://azure.microsoft.com/updates?id=567847)
VPN Gateway에서 IPv6 지원이 정식 제공되어, 듀얼스택 네트워크 구현과 차세대 IP 지원이 확대되었습니다.

### [NAT64 on StandardV2 NAT Gateway](https://azure.microsoft.com/updates?id=568409)
NAT64 기능이 도입되어 IPv6 워크로드를 IPv4 인터넷에 연결할 수 있어, 네트워크 호환성과 확장성이 높아졌습니다.

**카테고리 요약**  
네트워크 및 스토리지의 기능적 확장은 데이터 보호, 트래픽 관리, 보안 강화, 차세대 프로토콜 지원, 다중 구성의 유연성까지 포함되어 있습니다. 대규모 엔터프라이즈·멀티 클라우드 환경에 최적화된 스토리지·네트워크 솔루션들이 대거 반영되었습니다.

---

## 4️⃣ 관리, 거버넌스, 마이그레이션

### [Azure Automation supports PowerShell 7.6 runbooks and Runtime environment](https://azure.microsoft.com/updates?id=568102)
Automation에서 PowerShell 7.6 런북 등 최신 런타임 환경이 정식 지원되어, 스크립트 관리 효율성과 보안이 향상되었습니다.

### [Support 5x churn in Azure Site Recovery](https://azure.microsoft.com/updates?id=566966)
Site Recovery에서 VM 당 500MB/s 고속 처리 지원으로, 대용량 IOPS 워크로드 복구가 안정적으로 가능해졌습니다.

### [Public Preview: Azure Storage Mover now supports migration from Google Cloud Storage](https://azure.microsoft.com/updates?id=566948)
Storage Mover에서 GCS 데이터 클라우드 간 이전 지원으로, 멀티 클라우드 스토리지 통합 및 이동이 안전하게 이루어집니다.

### [Azure Chaos Studio Workspaces and Scenarios](https://azure.microsoft.com/updates?id=567184)
Chaos Studio에서 Workspaces & Scenarios 기능이 미리 보기로 추가되어, 실제 장애 시나리오 및 격리 테스트 자동화가 가능합니다.

### [Export historical data from Log Analytics workspace with Export jobs](https://azure.microsoft.com/updates?id=566591)
Log Analytics Export Job 기능 미리 보기로, 로그 데이터의 규정 준수, 감사 및 외부 시스템 이동이 지원됩니다.

**카테고리 요약**  
관리 및 거버넌스 부문은 자동화 환경의 고도화, 대규모 복구/백업 성능, 클라우드 간 데이터 이전, 장애 시나리오 자동 테스트 등 시스템 신뢰성과 운영 효율성 중심으로 기능이 강화되었습니다.

---

## 5️⃣ 보안, 컴플라이언스 및 네트워크 서비스

### [Confidential Computing support for Azure Event Hubs Dedicated](https://azure.microsoft.com/updates?id=567212)
Confidential Computing이 정식 지원되어, 스트리밍 처리 중 데이터 보호 및 신뢰 실행 환경 기반 보안이 강화되었습니다.

### [Network Security Perimeter support for Azure Event Hubs](https://azure.microsoft.com/updates?id=567203)
Event Hubs에서 NSP 지원으로, PaaS 리소스 격리와 퍼블릭 네트워크 접근 통제가 강화되었습니다.

### [Azure DDoS Protection custom policy](https://azure.microsoft.com/updates?id=568063)
DDoS Protection 맞춤 정책 미리 보기로, 트래픽별 임계치 조정과 공격 방어 정책의 유연성이 대폭 증가했습니다.

### [Symmetric keys on Azure Key Vault Premium](https://azure.microsoft.com/updates?id=566746)
Key Vault Premium에서 256비트 AES 기반 대칭키 미리 보기로, 키 관리와 암호화 적용이 중앙에서 간편하게 이루어집니다.

### [Azure Enclave](https://azure.microsoft.com/updates?id=568377)
Azure Enclave 미리 보기로, 격리된 클라우드 인프라 운영 및 네트워크 분리, 보안 정책 일괄 적용을 지원합니다.

**카테고리 요약**  
보안은 데이터 보호, 네트워크 격리, 맞춤형 DDoS 방어, 키 관리, 민감 정보 탐지 등 실제 컴플라이언스 시나리오에 직접 적용 가능한 기능이 강화되었습니다. 비즈니스 및 규제 요구를 동시에 만족하는 보안 정책의 표준화 방향이 잘 나타납니다.

---

## 6️⃣ Microsoft Foundry 및 Microsoft Fabric

### [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)
Foundry에서 Toolboxes 기능이 정식 지원되어, AI 에이전트와 툴 통합·재사용이 조직 전체에서 표준화되고 효율적으로 관리됩니다.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)
PII 탐지 NextGen Playground가 Foundry에서 정식 지원되어, 개인정보 보호 및 컴플라이언스 테스트 환경 구축이 더욱 유연해졌습니다.

### [Public Preview: Document PII playground sample in Microsoft Foundry NextGen](https://azure.microsoft.com/updates?id=563331)
Foundry NextGen 포털용 PII 탐지 샘플 Playground가 미리 보기로 제공, 신속 평가 및 결과 비교가 편리합니다.

### [Protect sensitive generative AI telemetry in Application Insights and Microsoft Foundry](https://azure.microsoft.com/updates?id=567594)
Foundry 내 Application Insights에서 AI 텔레메트리 데이터 보호 기능 미리 보기로, 규제 산업에서 민감 정보 관리가 가능해집니다.

### [Azure Monitor Logs mirroring into Microsoft Fabric](https://azure.microsoft.com/updates?id=568322)
Monitor 로그를 Microsoft Fabric으로 미러링 기능 미리 보기로, 운영·비즈니스 데이터 통합 분석이 실시간으로 가능해졌습니다.

**카테고리 요약**  
Foundry 및 Fabric 관련 업데이트는 AI 에이전트 툴 통합, 개인 정보 탐지, 텔레메트리 데이터 보호, 로그 통합 분석 등 신속한 실무 적용과 조직 내 표준화가 핵심입니다. 엔터프라이즈 전체에서 연결된 데이터와 AI 자산 관리가 한층 효율화되었습니다.

---

## 7️⃣ 리전 및 지역 확장

### [Azure Red Hat OpenShift in Chile Central](https://azure.microsoft.com/updates?id=566732)
칠레 중앙 리전에 OpenShift 정식 지원으로, 남미 지역 클라우드 네이티브 워크로드와 규제 환경에 맞춘 배포가 가능해졌습니다.

### [Azure Database for PostgreSQL flexible server in India South Central](https://azure.microsoft.com/updates?id=568334)
인도 남부 중앙 리전에서 PostgreSQL 플렉서블 서버가 정식 지원되어, 인도 내 데이터 레지던시·확장성이 강화되었습니다.

### [Microsoft Azure now available from new cloud region in India (India South Central)](https://azure.microsoft.com/updates?id=568013)
인도 남부 중앙 신규 리전이 개설되어, 현지 클라우드 인프라 및 AI 중심 디지털 전환 수요에 대응합니다.

### [Azure Databricks SQL Serverless in UK West](https://azure.microsoft.com/updates?id=567444)
UK West에서 SQL Serverless 정식 지원으로, 영국 내 데이터 레지던시와 분석 클라우드 수용성이 높아집니다.

### [Azure Sphere OS version 26.09 is now available for evaluation](https://azure.microsoft.com/updates?id=568466)
Azure Sphere OS 26.09 신규 버전이 평가용으로 제공되어, 장기 지원과 보안강화를 목적에 맞게 테스트 및 도입할 수 있습니다.

**카테고리 요약**  
글로벌 리전 확장-현지화 전략이 지속되며, 신규 리전 개설, 리전별 서비스 확대, 데이터 레지던시와 규제 대응이 동시에 이뤄지고 있습니다. 멀티 클라우드 환경의 관리 및 인프라 선택 폭이 넓어졌습니다.

---

## 총평 및 다음 달 전망

2026년 7월 Azure 업데이트는 AI 모델 도입과 데이터 관리 기능을 비롯해, 보안·컴플라이언스 강화, 멀티클라우드 및 리전 확장, 관리 자동화 등 엔터프라이즈 실무에서 요구되는 핵심 요소들이 균형 있게 반영되었습니다. Foundry 및 Fabric의 조직적 AI/데이터 적용 확대, 인도/칠레 등 신규 리전 지원, Kubernetes 인프라 자동화 등 기존 기술과 혁신 기능이 결합되어 기술적 진화를 이끌고 있습니다.

다음 달에는 AI 거버넌스, 데이터 보호, 네트워크·스토리지 성능 최적화, 클라우드 간 연계 등 엔터프라이즈 현장 중심의 고도화 업데이트가 지속될 전망입니다. 특히 AI 모델 및 엔진 추가와, 데이터 분석·관리 자동화, 보안 정책 일괄관리 등 실무 적용성을 높이는 혁신 서비스가 더욱 강화될 것으로 기대됩니다.