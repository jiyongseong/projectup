# Azure 주간 업데이트 요약 - 2026년 11월 02일

## 🔒 네트워크 및 보안
네트워크와 보안 부문에서는 Azure Front Door 프리미엄 WAF 정책의 정식 지원과 HTTP DDoS 규칙셋 도입으로 웹 애플리케이션 방어력 및 운영 효율성이 크게 향상됐습니다. 보안 정책을 프로필, 도메인, 경로별로 적용할 수 있어 서비스별 맞춤 보호가 가능하며, DDoS 방어는 Microsoft 위협 인텔리전스 기반 자동화·적응형 방식으로 정상과 이상 트래픽을 세밀하게 구분해 확장성까지 해결했습니다. 또한 Azure Network Watcher VNet 플로우 로그 필터링 기능이 정식 지원됨에 따라 IP, 포트, 프로토콜 등 다양한 기준으로 네트워크 트래픽 로그를 세분화해서 분석 및 비용 효율성을 확보할 수 있게 됐습니다. 이번 주 업데이트들은 다계층 보안 체계와 관리 자동화를 강화하고 기업의 안정적 클라우드 운영을 적극 지원합니다.

### [Azure Front Door 프로필 및 경로 단위 WAF 정책 정식 지원 출시](https://azure.microsoft.com/updates?id=578153)
Azure Front Door Premium에서 WAF 정책을 프로필, 도메인, 경로별로 유연하게 설정할 수 있어 다양한 서비스 운영에 적합합니다.

### [Azure Front Door Premium WAF HTTP DDoS 규칙셋 정식 지원 출시](https://azure.microsoft.com/updates?id=578681)
HTTP 계층 DDoS 공격 자동 대응 규칙셋이 정식 지원되어 봇 탐지, 신뢰 트래픽 예외 등 미세 조정 없이 효과적인 보호가 가능합니다.

### [Azure Network Watcher VNet 플로우 로그 필터링 기능 정식 지원](https://azure.microsoft.com/updates?id=577782)
IP, 포트, 프로토콜 등 기준별 세분화된 로그 수집으로 네트워크 운영과 보안 분석의 효율성과 경제성이 향상됩니다.

---

## 🛠️ 관리 및 거버넌스
관리 및 거버넌스 부문에서는 인프라 코드 관리, 리소스 할당량, 백업 복원 기능 등 핵심 역량이 동시에 강화되었습니다. Azure MCP Server 3.0 정식 지원으로 AI 에이전트와 개발자 도구의 Azure 연동뿐 아니라 인프라 관리, 백업·복구, 비용 최적화, 툴 통합 등 클라우드 거버넌스 전반에 걸친 역량 향상이 이루어졌습니다. Azure Blob Storage 계정 수 상향(최대 1,000개)으로 대규모 리소스 운영이 수월해졌고, Azure Backup Cross Tenant Restore 미리 보기 기능은 VM 백업을 독립 테넌트로 복원할 수 있어 회복력과 관리 효율성을 높였으며 사이버 공격 대응력도 강화됐습니다. 이번 업데이트는 조직 전체 IT 운영의 안정성과 비용 효율, 복구 신속성을 총체적으로 개선하는 기반이 됩니다.

### [Azure MCP Server 3.0 정식 지원 출시](https://azure.microsoft.com/updates?id=578662)
인프라 코드 관리, 백업·복구, 비용 최적화, 통합 툴 등 거버넌스 역량이 개선된 MCP Server 3.0이 정식 지원됩니다.

### [Azure Blob Storage 계정 지역별 할당량 상향 정식 지원](https://azure.microsoft.com/updates?id=578358)
Storage 계정 최대 1,000개까지 할당 가능해 대규모 데이터 자원 관리가 더욱 용이해졌습니다.

### [Azure Backup Cross Tenant Restore 미리 보기 제공](https://azure.microsoft.com/updates?id=577117)
CTR 기능으로 Azure VM 백업을 별도의 테넌트로 복원할 수 있어 사이버 회복성과 복구 경로 확보가 용이합니다.

---

## 💾 스토리지 및 데이터베이스
이번 주 스토리지와 데이터베이스 카테고리에선 데이터 관리와 보호력이 한층 강화됐습니다. Azure Blob Storage 계정 한도 상향으로 대규모 워크로드 지원이 가능해졌고, Azure Confidential VM 대용량 OS 디스크 암호화가 정식 지원되면서 마이그레이션 이후 OS 전체 암호화, 키관리, 하드웨어 기반 신뢰 실행 환경이 구축됩니다. Azure SQL Database에서는 데이터베이스별 관리형 ID를 개별 지정할 수 있는 미리 보기 기능이 출시되어, Blob Storage와 Data Lake Storage 접근 권한이 세분화되고 데이터베이스 간 접근 격리와 보안성이 강화됩니다. 이러한 업데이트들은 대규모 데이터 환경에서 유연한 관리와 첨단 보안을 실현합니다.

### [Azure Blob Storage 계정 지역별 할당량 상향 정식 지원](https://azure.microsoft.com/updates?id=578358)
Storage 계정 최대 1,000개까지 할당 가능해 대규모 데이터 관리 요구에 부응합니다.

### [Azure Confidential VM 대용량 OS 디스크 암호화 정식 지원 출시](https://azure.microsoft.com/updates?id=578850)
Confidential VM 마이그레이션에서 OS 디스크 전체 암호화가 정식 지원되어 데이터 보호와 키 관리가 강화됩니다.

### [Azure SQL Database 데이터베이스 수준 관리형 ID 미리 보기 출시](https://azure.microsoft.com/updates?id=577491)
데이터베이스별 관리형 ID 지정으로 데이터 접근 보안성과 격리가 향상됩니다.

---

## ✨ Microsoft Foundry / AI 및 머신러닝
AI 및 Microsoft Foundry 영역에서는 모델별 비용 집계 및 태깅 기능이 정식 지원되어 비용 분석과 책임성, 실무 투명성이 크게 개선됐습니다. Foundry Claude 모델의 비용이 Azure 리소스별로 집계되며 태그 기능을 활용해 팀·제품·워크로드별 비용 분류가 쉽게 자동화됩니다. 기존 수작업 비용 집계와 비교 시 회계·플랫폼 팀의 관리 소요가 줄고, 사용량별 정확한 배분이 가능해집니다. 태그와 그룹 기능을 활용한 클라우드AI 비용 분석은 활용률·책임성을 높여 기업의 AI 전략 운영에 실질적인 효율을 가져다 줍니다.

### [Microsoft Foundry Claude 모델 비용 관리 기능 정식 지원 출시](https://azure.microsoft.com/updates?id=577260)
Claude 모델 비용이 Azure Cost Management와 통합되어 투명한 집계와 체계적 비용 분석이 가능합니다.

### [Azure Foundry 비용 분석과 태깅 기능 상세 가이드](https://learn.microsoft.com/azure/foundry/concepts/manage-costs)
태깅을 통한 비용 관리, 조직별 워크로드 분리·분석 방법 등 Foundry AI 자원의 효율적인 관리 가이드가 제공됩니다.

### [Azure MCP Server 3.0 발매 블로그: AI와 개발 툴 통합 사례](https://devblogs.microsoft.com/azure-sdk/azure-mcp-server-3-0-stable-release/)
AI 에이전트 및 개발 도구 통합 사례와 MCP Server 3.0 기술적 의미가 블로그에서 설명됩니다.

---

## 🛒 마켓플레이스 및 컨테이너
이번 마켓플레이스와 컨테이너 부문에서는 구매 경험과 로그 관리 환경이 대폭 개선되었습니다. Azure Marketplace의 프라이빗 오퍼 기능이 개선되어 여러 제품을 한 번에 구매할 수 있는 단일 프로세스가 도입되어 도입 및 결제 과정이 간소화되었습니다. 또한 Azure Container Apps의 Log Analytics 로그 수집 옵션이 지원 종료되면서 Azure Monitor로의 마이그레이션이 권장되어 향후 관리 편의성과 보안이 강화됩니다. 관련 문서와 가이드, 마이그레이션 절차가 충분히 제공됨에 따라 관리자는 신속하게 대응할 수 있습니다.

### [Marketplace 프라이빗 오퍼 기능 개선 정식 지원](https://azure.microsoft.com/updates?id=576547)
프라이빗 오퍼 구매 과정이 단순화되어 여러 제품을 일괄 구매할 수 있게 됐습니다.

### [Azure Container Apps 로그 수집 옵션 지원 종료 및 Azure Monitor 마이그레이션 권장](https://azure.microsoft.com/updates?id=577689)
Log Analytics 로그 수집 옵션 지원이 종료되어 Azure Monitor로 전환이 필수이며 기존 환경 점검이 필요합니다.

### [Azure Container Apps 로그 마이그레이션 가이드](https://learn.microsoft.com/azure/container-apps/migrate-logs-azure-monitor?pivots=azure-portal)
Azure Monitor 마이그레이션 방법과 기존 Log Analytics 환경 점검 및 이행 절차가 자세히 안내됩니다.