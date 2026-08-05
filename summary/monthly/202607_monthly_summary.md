# Azure 월간 업데이트 요약 - 2026년 07월

## 전반적인 트렌드 및 핵심 인사이트

2026년 7월의 Azure 업데이트는 AI 중심 혁신, 클라우드 네이티브 관리 자동화, 대규모 데이터 관리, 강화된 네트워크 보안 및 서비스 운영 효율성을 중점으로 보여줍니다. 애널리틱스와 AI 분야에서는 Azure Databricks, Microsoft Foundry, API Management 등 AI 플랫폼 및 데이터 서비스의 정식 지원이 대폭 확대되었습니다. Anthropic Claude와 OpenAI GPT 등 최고 성능의 AI 모델 지원 확대와 함께, 기밀 컴퓨팅(Confidential Computing) 및 개인정보 보호(PII) 기능이 강화되어 기업의 보안 및 컴플라이언스 요구 사항에 보다 효과적으로 대응할 수 있게 되었습니다.

컨테이너, Kubernetes 및 DevOps 분야에서는 분산 클러스터 관리와 신속한 애플리케이션 배포를 위한 기능 업데이트가 두드러졌으며, 클라우드 운영 자동화와 데이터 보호 역시 주요 개선점으로 부각됩니다. Storage와 Networking 분야에서는 Azure Blob Storage, Files, NetApp Files의 데이터 무결성, 암호화, 네트워크 격리 등 보안 확장과 IPv6, NAT64 등 현대 네트워크 프로토콜 지원이 확대되어 하이브리드 및 멀티클라우드 환경의 연결성과 안정성을 크게 높였습니다.

아울러 인도, 칠레 등 신규 리전 오픈과 글로벌 지역 확장, 관리 자동화에 대한 런타임 지원, 서비스 단종(지원 종료), 예약 교환 정책 변화 등 운영적 측면에서도 주목할 만한 변화가 있었습니다. Microsoft Foundry와 Microsoft Fabric에서 데이터 통합, 관측성 강화, AI 모델 배포 및 관리 시스템의 진화가 확인되며, 앞으로도 AI 데이터 플랫폼의 지속적 발전이 기대됩니다.

전반적으로 보안 및 컴플라이언스, 대규모 관리 효율성, AI 기반 업무 자동화, 글로벌 서비스 확장과 사용자 경험 강화를 위한 혁신이 두드러진 한 달이었으며, 각 영역별 발전 트렌드와 전략 방향성이 명확히 나타나고 있습니다.

---

## ☁️ 클라우드 컴퓨트 및 컨테이너

이번 달 컴퓨트 및 컨테이너 분야는 Kubernetes와 AKS, Azure Functions 등 클라우드 네이티브 환경의 현대화와 운영 효율성 강화로 요약됩니다. 서비스 메쉬 없이 Kubernetes Gateway API 기반의 인그레스 관리 정식 지원과 Python 3.14 및 PowerShell 7.6 등 최신 런타임 환경 도입이 주목되었으며, 리소스 분산 관리, 준비된 이미지 사양(Prepared Image Specification), 그리고 IoT와 Edge 환경의 운영 체제 평판도 상승이 확인됩니다.

### [Application Routing with Gateway API](https://azure.microsoft.com/updates?id=567944)
AKS에서 Kubernetes Gateway API 기반 애플리케이션 라우팅이 정식 지원되어, 기존 인그레스-nginx 환경에서 단계적 전환이 가능해졌습니다. 서비스 메쉬 없이 현대적 인그레스 관리 모델이 적용됩니다.

### [Azure Functions support for Python 3.14](https://azure.microsoft.com/updates?id=567646)
Python 3.14 지원이 도입되어 Azure Functions 개발자가 보안 강화, 장기 지원, 향상된 개발 도구를 활용할 수 있게 됐습니다.

### [Public Preview: Azure Functions Support for PowerShell 7.6](https://azure.microsoft.com/updates?id=567651)
PowerShell 7.6 기반 Azure Functions의 미리 보기 지원으로 최신 스크립팅 환경 및 개발 프로세스 최적화가 가능해졌습니다.

### [Resource placement in Azure Kubernetes Fleet Manager](https://azure.microsoft.com/updates?id=567931)
Fleet Manager에서 여러 AKS 및 Arc 클러스터를 대상으로 일관된 리소스 배포가 정식 지원, 운영 자동화와 클러스터 간 정책 일관성을 확보할 수 있습니다.

### [Prepared Image Specification](https://azure.microsoft.com/updates?id=567949)
AKS 노드의 사전 이미지 지정 기능이 미리 보기로 출시되어 신속한 확장성과 애플리케이션 기동 성능 향상, 대규모 운영 효율화가 기대됩니다.

---

## 📊 분석, AI 및 데이터 서비스

7월은 Azure Databricks와 AI 모델 기반 서비스 확장, 기밀 컴퓨팅과 개인정보 검출 및 보호 강화에 중점을 두었습니다. Claude, GPT, Sonnet 등 최신 AI 모델 지원 확대와 AKS 기반 클라우드 데이터 관리, Event Hubs, Databricks 등 데이터 분석 플랫폼의 보안 및 운영 효율성 강화가 두드러졌습니다.

### [Claude Opus 5 on Azure Databricks](https://azure.microsoft.com/updates?id=568316)
Anthropic Claude Opus 5 모델이 Azure Databricks AI Model Serving에 적용됐다. 고차원적 리즈닝, 에이전트 워크플로우, 코드 자동화 등 전문 업무에서 활용성을 높았습니다.

### [Open AI GPT-5.6 on Azure Databricks](https://azure.microsoft.com/updates?id=567431)
Microsoft Foundry 연동을 통한 GPT-5.6 정식 지원으로 엔터프라이즈 데이터 기반 AI 모델의 배포, 관리, 거버넌스가 강화됐습니다.

### [Generally available: Anthropic Claude Sonnet 5 on Azure Databricks](https://azure.microsoft.com/updates?id=567194)
Claude Sonnet 5가 Azure Databricks에서 정식 지원되어, 대용량 코드 자동화 및 에이전트 설계에 최적화된 모델 활용이 가능해졌습니다.

### [Confidential Computing support for Azure Event Hubs Dedicated](https://azure.microsoft.com/updates?id=567212)
Azure Event Hubs Dedicated 환경에서 기밀 컴퓨팅 지원으로 메모리 사용 데이터의 안전이 확보되어, 민감한 데이터의 스트리밍 및 분석 시 보안 수준이 크게 향상됐습니다.

### [Network Security Perimeter support for Azure Event Hubs](https://azure.microsoft.com/updates?id=567203)
이제 Event Hubs에 네트워크 보안 경계(NSP) 기능이 담겨 보안 단위별 접속 제어와 데이터 유출 방지 정책 적용이 쉬워졌습니다.

---

## ⚙️ 관리 및 거버넌스, 자동화

관리 자동화와 거버넌스 분야에서는 Azure Automation의 최신 런타임 환경 도입과 Azure Site Recovery, Chaos Studio, 예약 교환 정책 변화, 런타임 지원 종료 등 관리 효율성 및 보안 강화, 서비스 운영 정책 변화가 주요 이슈로 부각됩니다.

### [Azure Automation supports PowerShell 7.6 runbooks and Runtime environment](https://azure.microsoft.com/updates?id=568102)
PowerShell 7.6 런북과 Runtime 환경의 정식 지원은 오래된 스크립트의 손쉬운 업그레이드와 신규 언어 버전 도입, 모듈 충돌 관리 개선을 의미합니다.

### [Support 5x churn in Azure Site Recovery](https://azure.microsoft.com/updates?id=566966)
Site Recovery에서 VM당 최대 500MB/s의 타전 지원(5배 증가)이 가능해져 고성능, 고IOPS 워크로드의 안정적 재해 복구가 더욱 용이해졌습니다.

### [Azure Chaos Studio Workspaces and Scenarios](https://azure.microsoft.com/updates?id=567184)
Chaos Studio가 Workspaces 및 Scenarios 기능으로 다양한 실 운영 장애 시나리오 모의 실험과 영향 리포트를 통한 컴플라이언스 대응이 강화됩니다.

### [Manage Azure Chaos Studio from the Azure CLI](https://azure.microsoft.com/updates?id=567225)
CLI에서 Chaos Studio 시나리오 관리가 가능해져 운영 자동화 및 도구 통합이 편리해졌습니다.

### [Support for Python-2.7; 3.8 and PowerShell- 7.1; 7.2 will be retired on September 30, 2026](https://azure.microsoft.com/updates?id=567556)
Automation 서비스의 특정 런타임 버전이 2026년 9월 종료되어, 신규 버전으로의 업그레이드 필요성이 커졌습니다.

---

## 🔒 보안, 네트워킹 및 컴플라이언스

이번 달은 암호화, 네트워크 경계, 인증·접근관리, 보안 정책의 진화가 집중되었습니다. Blob Storage, VPN Gateway, NAT Gateway, Azure Firewall, DDoS Protection 등에서 최신 프로토콜, 실시간 보안 기능, 세부 정책 제어 등이 부각됩니다.

### [HTTP header insertion in Azure Firewall](https://azure.microsoft.com/updates?id=568115)
Azure Firewall에서 HTTP/HTTPS 헤더 삽입 기능이 도입, 다양한 보안 시나리오에 따른 헤더 기반 인증 및 접근 제어를 네이티브로 지원합니다.

### [IPv6 support for Azure VPN Gateway](https://azure.microsoft.com/updates?id=567847)
VPN Gateway에서 IPv6 지원이 정식 적용되어, 하이브리드 및 다중 네트워크 환경의 확장성과 연결성, 운영 안정성이 개선됐습니다.

### [NAT64 on StandardV2 NAT Gateway](https://azure.microsoft.com/updates?id=568409)
NAT Gateway의 NAT64 기능으로 IPv6 워크로드가 IPv4만 지원하는 인터넷 대상과 효과적으로 통신할 수 있게 되었습니다.

### [Azure DDoS Protection custom policy](https://azure.microsoft.com/updates?id=568063)
DDoS Protection에 맞춤 정책 도입으로, 서비스 별 규모, 프로토콜별 임계점 지정에 따라 더욱 세밀한 공격 방어와 트래픽 관리가 가능해졌습니다.

### [Azure Enclave](https://azure.microsoft.com/updates?id=568377)
Azure Enclave의 미리 보기로 민감한 업무 환경에 대해 네트워크 및 데이터 분리, 보안 강화, 관리 효율성을 동시에 확보할 수 있게 됐습니다.

---

## 🗄️ 스토리지, 데이터베이스 및 마이그레이션

이번 달 스토리지/데이터베이스 분야는 Azure Blob, Files, NetApp Files 등 데이터 무결성, 암호화, RBAC 인증, 클라우드 간 마이그레이션 효율성에 집중되었습니다. PostgreSQL, Storage Mover 등 데이터 관리, DB 운영 자동화, PowerShell 모듈 확대도 주요 이슈입니다.

### [Client-side data integrity protections in Azure Blob Storage](https://azure.microsoft.com/updates?id=566895)
Blob Storage에서 CRC64-NVME 기반 클라이언트 데이터 무결성 검증이 SDK 레벨 적용되어 데이터 일관성 보장이 강화됐습니다.

### [Encryption in Transit for Azure Files NFS Shares in Azure Kubernetes Service (AKS)](https://azure.microsoft.com/updates?id=567787)
AKS와 Azure Files NFS간 데이터 이동 암호화 정식 지원으로, TLS 기반 전송 보안 및 컴플라이언스 강화가 이루어졌습니다.

### [Public Preview: Azure Storage Mover now supports migration from Google Cloud Storage (GCS)](https://azure.microsoft.com/updates?id=566948)
Storage Mover에서 GCS 기반 S3 인터페이스 지원 및 Azure Key Vault 기반 보안 마이그레이션이 제공되어 클라우드 간 데이터 이동이 더욱 안전하고 효율적으로 가능해졌습니다.

### [Microsoft Entra ID-based access for Azure Blob Storage SFTP](https://azure.microsoft.com/updates?id=567085)
Entra ID 기반 SFTP 인증을 통해 RBAC, MFA, 조건부 접근 정책 등과 통합되어 안전한 외부 협업, 사용자 관리가 용이해졌습니다.

### [Support for SMB Opportunistic Locking (Oplocks) configuration](https://azure.microsoft.com/updates?id=568396)
NetApp Files에서 SMB Oplocks 옵션 관리가 가능해 SMB 클라이언트 캐싱 최적화와 크로스리전 볼륨별 별도 설정이 지원됩니다.

---

## 🌏 리전 및 글로벌 서비스 확장

MS Azure 서비스의 글로벌 데이터센터 확장과 OpenShift, PostgreSQL, Storage 등의 신규 리전 적용이 두드러졌으며, 인도와 칠레 등 신흥시장 접근성이 크게 개선되었습니다.

### [Microsoft Azure now available from new cloud region in India (India South Central)](https://azure.microsoft.com/updates?id=568013)
인도의 네 번째 Azure 데이터센터(India South Central) 오픈으로, 현지 AI 및 클라우드 인프라 수요 대응, 레이턴시 및 컴플라이언스 등 다양한 요구에 대응력을 강화합니다.

### [Azure Database for PostgreSQL flexible server in India South Central](https://azure.microsoft.com/updates?id=568334)
PostgreSQL Flexible Server가 인도 남부 중앙 리전에서 정식 지원됨에 따라, 지역별 데이터베이스 운영 및 서비스 분산이 용이해졌습니다.

### [Azure Red Hat OpenShift in Chile Central](https://azure.microsoft.com/updates?id=566732)
칠레 중앙 리전에서 OpenShift가 정식 지원되면서, 현지 규제 및 데이터 레지던시 요구를 만족하는 클라우드 네이티브 환경이 확대됩니다.

### [New Powershell module:  Az.PostgreSQLFlexibleServer](https://azure.microsoft.com/updates?id=566209)
Azure PostgreSQL 관리를 위한 최신 PowerShell 모듈이 추가 제공되어 데이터베이스 운영 자동화 및 신기능 연동이 쉬워졌습니다.

### [Reservation exchanges for Azure services supported by savings plans will no longer be available starting February 1, 2027](https://azure.microsoft.com/updates?id=568514)
2027년 2월부터 일부 서비스에서 예약 교환 정책 변경 적용, 사용자는 정책 변화에 대비해야 합니다.

---

## 🧪 Microsoft Foundry & Microsoft Fabric

이번 달은 Foundry와 Fabric에서 AI/ML 모델 배포, PII 탐지, 도구 통합, 데이터 미러링 등 혁신적 기능 추가가 눈에 띄었습니다. 데이터 통합, 관측성 강화, AI 자산 관리가 조직 전체에 쉽게 확장 가능한 체계를 제공하고 있습니다.

### [Toolboxes in Microsoft Foundry](https://azure.microsoft.com/updates?id=563481)
Foundry Toolboxes의 정식 지원으로 다양한 AI 도구와 엔드포인트를 단일 MCP 기반으로 통합 관리, 거버넌스 정책 일원화가 가능해졌습니다.

### [Document PII NextGen Playground in Azure AI Language](https://azure.microsoft.com/updates?id=564382)
AI Language의 문서 기반 PII 검출 Playground 정식 지원으로, 실제 데이터 테스트 없이 개인정보 보호 시나리오를 신속히 평가할 수 있습니다.

### [Public Preview: Document PII playground sample in Microsoft Foundry NextGen](https://azure.microsoft.com/updates?id=563331)
Foundry 포털에서 확장된 PII Playground 경험 미리 보기로, 샘플 문서를 통한 검출 결과 평가 및 API 통합이 간편해졌습니다.

### [Protect sensitive generative AI telemetry in Application Insights and Microsoft Foundry](https://azure.microsoft.com/updates?id=567594)
Application Insights와 Foundry에서 생성형 AI 텔레메트리 전용 접근제어와 보호 기능이 도입되어 PII·PHI 등 민감데이터 처리 안전성이 향상됐습니다.

### [Azure Monitor Logs mirroring into Microsoft Fabric](https://azure.microsoft.com/updates?id=568322)
Azure Monitor 로그를 Microsoft Fabric으로 미러링하여, 데이터 중복 없이 Fabric의 Eventhouse, Power BI, Spark 등과 통합 분석 및 AI 활용이 지원됩니다.

---

## 💬 기타 및 공지사항

서비스 출시/단종 및 정책 변화, 리전별 서비스 현황, 주목할 만한 기념 공지 등이 포함됩니다.

### [Announcing: Reservation exchanges for Azure services supported by savings plans will no longer be available starting February 1, 2027](https://azure.microsoft.com/updates?id=568514)
2027년 2월부터 Savings Plan 적용 서비스에 대한 예약 교환이 중단 예정, 기존 구매자는 한 번의 최종 교환 권리만 유지됩니다.

---

## 이번 달 총평 및 다음 달 전망

2026년 7월의 Azure 업데이트는 AI 데이터 분석 플랫폼의 발전과 보안·컴플라이언스 강화, 관리 자동화, 글로벌 리전 확장이 조화를 이루었습니다. Kubernetes 및 컨테이너 기술의 성숙은 신속한 애플리케이션 배포와 대규모 관리 체계 구성을 가속화하며, 최신 런타임과 운영 자동화, 데이터 무결성, 암호화 등 보안 지원도 한층 강화됐습니다. 리전 확장과 API, Foundry, Fabric 등 데이터 및 AI 자산 관리 혁신은 엔터프라이즈 운영을 위한 탄탄한 기반을 제공하고 있습니다.

다음 달에는 AI 워크로드를 위한 네트워크 인프라 최적화, 클라우드 보안 정책 변화, 리전별 서비스 확장, Microsoft Foundry와 Fabric에서의 신규 AI 모델 및 데이터 통합 기능 추가 등, 더욱 혁신적이고 실질적인 서비스 개선이 기대됩니다. Azure 관리 및 운영의 자동화, 보안, 글로벌 서비스 적용, AI 데이터 플랫폼 통합 등 클라우드의 핵심 트렌드는 지속적으로 심화될 전망입니다.