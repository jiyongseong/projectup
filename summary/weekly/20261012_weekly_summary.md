# Azure 주간 업데이트 요약 - 2026년 10월 12일

## 🚀 출시 및 정식 지원
지난주 Azure는 클라우드 인프라와 데이터 서비스의 혁신을 이끌 신규 서비스와 기능을 정식 지원으로 선보였습니다. 대표적으로 Anyscale on Azure 정식 지원을 통해 Ray 기반 분산 파이썬 워크로드 처리를 네이티브로 제공하며, AKS 관리 NAT Gateway는 고가용성과 IPv6 지원을 강화하여 신뢰성 있는 클러스터 운영이 가능해졌습니다. SQL Server 리눅스용 Bulk Admin 역할 신설로 보안 유연성 및 최소 권한 모델 적용이 확대되었습니다. Azure Database for PostgreSQL은 신규 리전(East US 3) 포함으로 글로벌 확장성을 높였고, Application Gateway 및 Front Door의 WAF 예외 기능은 보안 정책 커스터마이즈를 지원하여 기업별 맞춤 운영이 한층 용이해졌습니다. 이러한 업데이트는 클라우드 기반 데이터주권 확장, 네트워크 신뢰성 강화, 보안 모델 개선 등 Azure 플랫폼의 경쟁력을 전반적으로 끌어올리고 있습니다.

### [Anyscale on Azure 정식 지원 출시](https://azure.microsoft.com/updates?id=573744)
Ray 플랫폼을 Azure AKS에 네이티브로 배포, 데이터 준비부터 모델 학습·추론·강화학습까지 단일 파이썬 런타임으로 통합 관리하는 클라우드 서비스가 정식 지원되었습니다.

### [Azure Database for PostgreSQL Flexible Server 신규 리전 지원](https://azure.microsoft.com/updates?id=573691)
East US 3 리전에서 PostgreSQL Flexible Server를 배포할 수 있게 되어 글로벌 데이터베이스 운영의 선택폭과 탄력적 확장이 확대되었습니다.

### [Azure Application Gateway 및 Azure Front Door WAF 예외 기능 정식 지원](https://azure.microsoft.com/updates?id=574343)
웹 애플리케이션 방화벽의 규칙별/그룹별 예외 설정 기능이 정식 지원되어 URI, IP, 헤더 등 기준으로 세밀한 보안 정책 튜닝이 가능해졌습니다.

---

## 🧪 미리 보기 및 프리뷰
Azure의 다양한 미리 보기 서비스와 기능은 고객의 실환경 실험과 혁신 시나리오 구현을 지원하고 있습니다. AKS 베어메탈(Ubuntu) 미리 보기는 온프레미스에서도 Azure Kubernetes 경험 및 GPU 자율적 활용을 가능하게 하며, PostgreSQL 백업 v2 프리뷰는 최대 64TB, 10년 보존 등 엔터프라이즈급 장기 데이터 보호 기능을 제공합니다. Application Gateway WAF의 IPv6 지원 또한 듀얼스택 환경에서 보안 일관성을 극대화하고, HorizonDB 리전 미리보기로 글로벌 데이터 활용성을 높였습니다. Microsoft Agent 365와 Azure API Management 통합 프리뷰는 중앙 거버넌스와 런타임 정책 적용을 연동하여 AI·DevOps 관리의 효율성을 혁신합니다. 이런 프리뷰들은 대규모 데이터 처리, 보안 강화, 클라우드·온프레미스 통합 등 다각적 기술도입을 도와줍니다.

### [AKS 베어메탈(Ubuntu) 미리 보기](https://azure.microsoft.com/updates?id=573782)
AKS를 온프레미스 Ubuntu 하드웨어에 직접 배포하여 GPU, 데이터 근접성, 관리 모델을 자유롭게 운영할 수 있는 프리뷰가 공개되었습니다.

### [PostgreSQL Flexible Server & Elastic Cluster 백업 v2 미리 보기](https://azure.microsoft.com/updates?id=573425)
최대 64TB 서버, 인크리멘털 백업, 서버 수준 복원, 10년 보존 등 대규모·장기 데이터 보호를 프리뷰로 제공합니다.

### [Application Gateway WAF IPv6 지원 미리 보기](https://azure.microsoft.com/updates?id=573861)
IPv6 트래픽 검사 및 차단 기능이 공개되어 듀얼스택 네트워크 환경에서 일관된 보안 적용과 커스텀 규칙 운용이 가능합니다.

---

## 🛑 지원 종료 및 사용 중단
Azure는 주요 기능 및 서비스의 지원 종료 일정을 발표하여 고객의 마이그레이션 준비를 촉진하고 있습니다. Always Encrypted with Intel SGX enclaves는 2027년 10월 31일 지원 종료되며, VBS Enclaves 또는 Confidential VM으로 전환이 필요합니다. Azure App Service on Azure Stack Hub 역시 2029년 9월 30일 종료 예정으로 신규 설치 및 확장이 중단되고, 마이그레이션을 추천합니다. Azure Deployment Environments은 2027년 2월 22일 운영 종료되며 환경, 카탈로그, 워크플로우 전환 준비가 필수입니다. 이 외에도 AKS pod name dimension 및 Key Vault Secrets Provider Extension 지원 종료, Microsoft Dev Box 단계적 종료, Java 8/11/17 지원 종료 등이 공지되어, 기능 대체와 보안 전환이 요구됩니다.

### [Always Encrypted with Intel SGX Enclaves 지원 종료](https://azure.microsoft.com/updates?id=569236)
SGX 기반 Azure SQL Database 기능이 2027년 10월 31일자로 종료되며, VBS Enclaves 또는 Confidential VM으로 전환이 필요합니다.

### [Azure App Service on Azure Stack Hub 지원 종료](https://azure.microsoft.com/updates?id=568178)
2029년 9월 30일 지원 종료가 예정되어 신규 설치, 확장·기능 추가가 중단되며, 마이그레이션 준비가 필요합니다.

### [Azure Deployment Environments 서비스 지원 종료 안내](https://azure.microsoft.com/updates?id=567934)
2027년 2월 22일부로 서비스 운영이 종료되며, 현 환경·카탈로그·워크플로우에 대한 대체 솔루션 선정과 이전 방안 검토가 필수입니다.

---

## 📊 데이터베이스 및 스토리지
최근 Azure는 데이터베이스와 스토리지 서비스의 글로벌 확장과 보안·관리 기능 혁신을 추진하며, 기존 기술의 지원 종료 및 신규 기능 도입을 병행하고 있습니다. SQL Server on Azure VMs이 프랑스 독립 클라우드(Azure Bleu)에 지원되어 데이터 주권 준수가 강화되었고, HorizonDB 리전 확장 및 PostgreSQL Flexible Server 리전 추가로 지역별 인프라 유연성이 높아졌습니다. SQL Server 리눅스용 Bulk Admin 역할 신설은 최소 권한 보안 모델로 대량 데이터 적재 권한 분리를 지원합니다. PostgreSQL 백업 v2 미리 보기, Always Encrypted SGX 지원 종료, Key Vault 확장 지원 종료 등은 대규모 데이터 보호 및 보안 모델 현대화를 촉진하며, 기업의 시나리오별 데이터 관리 신뢰성을 보장합니다.

### [SQL Server on Azure Virtual Machines Azure Bleu 지원](https://azure.microsoft.com/updates?id=571499)
프랑스 독립 클라우드 Azure Bleu에서 SQL Server 워크로드를 배포 지원, 데이터 주권과 규제 준수를 강화합니다.

### [Azure HorizonDB 리전 확장 미리 보기](https://azure.microsoft.com/updates?id=572940)
HorizonDB의 신규 리전 지원이 확대되어 PostgreSQL 워크로드의 글로벌 확장 및 인프라 유연성이 개선됩니다.

### [SQL Server Linux용 Bulk Admin 역할 지원 출시](https://azure.microsoft.com/updates?id=573443)
리눅스 환경에서 최소 권한 보안 모델에 따른 대량 데이터 적재 권한 분리 기능이 정식 지원되어 더 안전한 서버 운영을 제공합니다.

---

## 🛠️ 개발·운영 툴 & 통합, 마켓플레이스
Azure는 개발·운영 환경의 효율성과 관리 통합을 위한 신규 서비스와 지원 종료 일정을 동시에 발표했습니다. Microsoft Agent 365와 API Management 통합 프리뷰는 중앙 거버넌스와 런타임 정책 적용을 연동하여 엔터프라이즈 AI 관리 효율성을 높이고, Multiparty Private Offers 마켓플레이스 홍콩 확장은 제3자 솔루션 조달과 고객 기반 확대를 지원합니다. Dev Box 및 AKS 메트릭 pod name dimension 지원 종료로 플랫폼 전환 준비가 필수이며, Key Vault Secrets Provider Extension 지원 종료와 Secret Store Extension로의 전환 안내로 인증·오프라인 접근 등 보안 기능이 향상됩니다. 이를 통해 하이브리드 운영, 공급망 관리, 플랫폼 이전에 선제적으로 대응할 수 있습니다.

### [Microsoft Agent 365와 Azure API Management 통합 미리 보기](https://azure.microsoft.com/updates?id=574204)
중앙 거버넌스, 런타임 정책 적용, 도구 활동 모니터링, 위협 보호 등 AI 거버넌스 통합 관리가 가능해졌습니다.

### [Multiparty Private Offers 마켓플레이스 홍콩 확장](https://azure.microsoft.com/updates?id=571831)
파트너 기반 제3자 솔루션 조달로 새로운 시장 진출, 고객 기반 확대가 지원됩니다.

### [Azure Key Vault Secrets Provider Extension 지원 종료 안내](https://azure.microsoft.com/updates?id=570313)
2027년 10월 9일 지원 종료 예정으로, Secret Store Extension로 조속한 이전이 필요하며 인증·오프라인 접근 등 기능이 강화됩니다.

---

## 📈 Microsoft Fabric 및 분석
Microsoft Fabric은 데이터 분석과 AI 플랫폼의 혁신을 지속적으로 선보이고 있습니다. OneLake Catalog의 테이블 검색 기능 강화로 글로벌 검색, OneLake Catalog UI, Search API, Fabric MCP 서버 등 다양한 경로에서 권한 기반 테이블 검색이 가능해졌습니다. 테이블별 검색과 표준화된 데이터 접근 제어가 정책 중심 데이터 운용에 적합하게 최적화되어, 사용자 접근성과 보안성이 모두 향상되었습니다. Fabric 관리자 포털에서 검색 기능 설정을 조정할 수 있어 조직별 관리 및 데이터 보호 정책 적용이 한층 유연해졌습니다. 다양한 오브젝트 검색·발견 기능은 빅데이터, IoT, AI 시나리오의 데이터 활용성과 생산성을 크게 높이고 있습니다.

### [OneLake Catalog 테이블 검색 기능 강화](https://azure.microsoft.com/updates?id=573875)
글로벌 검색, API, CLI, discovery skill 등에서 테이블 개별 검색 지원으로 데이터 활용성과 보안이 동시에 강화되었습니다. Fabric 관리자 포털에서 검색 기능 관리도 가능해졌습니다.