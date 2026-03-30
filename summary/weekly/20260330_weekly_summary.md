# Azure 주간 업데이트 요약 - 2026년 03월 30일

## 🧠 Microsoft Foundry

Microsoft Foundry 카테고리는 이번 주 AI 우선처리 기술, 문서 AI 품질 개선, 엔터프라이즈 CI/CD 혁신 등이 두드러졌습니다. Foundry의 우선처리 기능 정식 지원은 실시간 Copilot 또는 AI 에이전트 배포시 일정한 서비스 품질을 보장하며, 복잡한 AI 레이턴시 문제를 근본적으로 해결합니다. Azure Content Understanding의 문서 AI 추출 품질 개선은 다양한 산업 데이터 처리의 신뢰도를 높여 대규모 기업 환경에서 자동화와 효율성을 극대화합니다. 또한 GraphQL 소스 관리 및 CI/CD API, dbt 기반 데이터 변환, SQL 프로젝트 DevOps 통합 등으로 데이터 흐름 자동화와 거버넌스, 버전 관리 등 엔터프라이즈 데이터 운영 역량이 크게 향상되었습니다. 이러한 발전은 금융, 제조, 개발, 대시보드와 같은 실제 AI 및 분석 환경에 즉각 활용될 수 있어 기업의 데이터 경쟁력을 높입니다.

### [정식 지원: Microsoft Foundry - 우선처리 기능 출시](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/announcing-priority-processing-in-microsoft-foundry-for/ba-p/4504788)
AI 워크로드의 실시간 배포에 활용되는 우선처리 기능이 일반 출시되어, Copilot 등 미션크리티컬 환경에서도 일정한 성능과 비용 효율이 보장됩니다.

### [정식 지원: Azure Content Understanding - 문서 AI 추출 품질 개선](https://techcommunity.microsoft.com/t5/microsoft-foundry-blog/closing-the-last-mile-in-document-ai-improving-extraction/ba-p/4502029)
문서 레이아웃 변동, 추출 정확성 문제를 AI 기반으로 해결하여, 의료·법률 등 산업별 데이터 처리 신뢰도가 크게 향상되었습니다.

### [정식 지원: GraphQL 소스 관리 및 CI/CD API](https://blog.fabric.microsoft.com/en-US/blog/api-for-graphql-source-control-and-ci-cd-support-generally-available/)
Fabric 환경 내 GraphQL 아티팩트의 버전 관리와 자동화 배포가 이루어져, 기업 데이터 거버넌스와 협업이 한층 강화되었습니다.


## 🎛️ Microsoft Fabric

Fabric 카테고리에서는 데이터 통합, AI 준비, 관리 자동화 등 데이터 플랫폼 전반의 혁신이 두드러졌습니다. Dataflow Gen2 변수 라이브러리 통합은 환경간 변수 자동화와 대규모 배포 일관성을 제공하며, Tonic Textual 미리보기로 비정형 데이터의 AI-ready 전환이 가능해졌습니다. JDBC 드라이버, 워크스페이스 태그 관리, Copilot 통합 등 여러 기능이 정식 지원되면서 엔터프라이즈 환경의 데이터 이동성과 분석 신뢰성이 높아졌습니다. 보안 관리, 워크스페이스 태그, IP 방화벽 같은 데이터 거버넌스 지원 강화로 기업의 데이터 인프라 조작과 보호가 한층 안전해졌으며, 실시간 대시보드 및 비정형 데이터 분석의 실무 활용 가능성이 확대되었습니다.

### [정식 지원: Dataflow Gen2 변수 라이브러리 통합](https://blog.fabric.microsoft.com/en-US/blog/dataflow-gen2-variable-library-integration-in-microsoft-fabric-generally-available/)
운영 및 배포 환경에서 반복적 변수 관리, 대규모 데이터 통합 자동화로 환경 일관성이 보장됩니다.

### [정식 지원: Fabric에서 AI 준비 데이터 변환(Tonic Textual)](https://blog.fabric.microsoft.com/en-US/blog/from-restricted-to-ai-ready-preparing-unstructured-data-directly-in-microsoft-fabric-with-tonic-textual-generally-available/)
비정형 데이터를 AI-ready 데이터로 쉽고 빠르게 변환하여, 실무 AI 프로젝트의 성공률과 실시간 데이터 활용성이 크게 증가합니다.

### [정식 지원: 워크스페이스 태그 기반 관리](https://blog.fabric.microsoft.com/en-US/blog/find-and-manage-workspaces-faster-with-workspace-tags-generally-available/)
메타데이터 기반으로 콘텐츠 검색과 운영 효율성이 향상되어, 조직 전체 관리 체계의 지능형 자동화가 강화됩니다.


## 🔒 보안 및 네트워크

보안과 네트워크 카테고리에서는 VNET 데이터 게이트웨이 인증서 및 프록시 지원, Fabric API의 테넌트 단 Private Link, Cosmos DB 미러링 프라이빗 엔드포인트 등 신규 보안 기능이 출시되었습니다. 인증서 및 프록시 기능은 네트워크 분리와 보안 설정 유연성을 제공하며, Fabric Private Link 지원은 내부망 기반 안전한 API 접근과 데이터 보호를 보장합니다. Cosmos DB 미러링에서는 네트워크 격리 및 실시간 분석이 가능해져, 규제 산업과 민감 데이터 보호를 위한 네트워크 보안이 대폭 강화되었습니다. SQL, MySQL, PostgreSQL 등 다양한 서비스에서 세분화된 접근 관리와 실시간 모니터링, 규제 대응이 이루어져 멀티클라우드 환경에서도 안전한 데이터 운영이 가능해졌습니다.

### [정식 지원: VNET 데이터 게이트웨이 인증서 및 프록시 지원](https://blog.fabric.microsoft.com/en-US/blog/certificate-and-proxy-support-for-vnet-data-gateway-generally-available/)
엔터프라이즈 및 규제 산업 환경에서 데이터 게이트웨이의 보안성과 네트워크 설정 유연성이 크게 향상되었습니다.

### [정식 지원: Fabric GraphQL 테넌트 단 Private Link 지원](https://blog.fabric.microsoft.com/en-US/blog/34710/)
데이터 API를 Private Link 기반 내부망에서만 접근 가능하도록 하여, 대규모 기업 데이터 보안 전략이 강화됩니다.

### [정식 지원: Cosmos DB Fabric 미러링 프라이빗 엔드포인트 지원](https://azure.microsoft.com/updates?id=558836)
운영 데이터의 미러링에서도 네트워크 격리와 규제 대응, 보안 환경에서 실시간 분석이 지원됩니다.


## ⚙️ 데이터베이스 및 DevOps

데이터베이스 및 DevOps 카테고리에서는 Azure SQL, PostgreSQL, Cosmos DB 등 주요 서비스의 기능 확장과 실시간 이벤트 스트리밍, 마이그레이션이 강화되었습니다. PostgreSQL 온라인 마이그레이션(최신 pgoutput 플러그인), AlloyDB/EDB 지원 등으로 대규모 데이터 현대화와 서비스 중단 없는 전환이 용이해졌습니다. Azure SQL Managed Instance의 이벤트 스트리밍 기능은 실시간 데이터 변경 통합 아키텍처 구현을 지원합니다. SQL 프로젝트 기반 DevOps, 자동화 배포, GitHub Copilot 등 업무 효율성 및 개발 생산성이 향상되었습니다. 데이터 이동성, 실시간 분석, 오류 방지 등 데이터 관리 신뢰성과 유연성이 확대되며, GitHub/VS Code 통합으로 협업과 CI/CD 환경이 더욱 강화되었습니다.

### [정식 지원: Azure SQL Late-March 2026 업데이트](https://azure.microsoft.com/updates?id=558879)
실시간 데이터 연결, 코드 분석, Fabric 연동, .dacpac/.bacpac 파일 내보내기 등 현대적 데이터베이스 관리가 지원됩니다.

### [정식 지원: PostgreSQL 온라인 마이그레이션 pgoutput 플러그인](https://azure.microsoft.com/updates?id=558846)
최신 마이그레이션 프레임워크로 서비스 중단 최소화, 오픈소스 호환성 개선 등 데이터 현대화가 촉진됩니다.

### [정식 지원: Azure SQL Managed Instance Change Event Streaming](https://azure.microsoft.com/updates?id=558884)
실시간 데이터 변경 이벤트를 Event Hub와 연동하여, 이벤트 기반 아키텍처 및 실시간 분석이 가능해졌습니다.


## 🚀 컨테이너 및 Kubernetes

이번 주 컨테이너 및 Kubernetes 카테고리에서는 Azure Container Storage의 Elastic SAN 연동, AKS 네트워크 로그 및 메트릭 필터링, GPU 사용량 통합 모니터링 등 대규모 환경에서 안정적 운영과 관리 효율성을 높이는 기능이 대거 공개되었습니다. 컨테이너 스토리지의 중앙화 및 확장성 향상, 네트워크 플로우 실시간 분석, AI 기반 네트워크 진단과 크로스 클러스터 네트워킹 등이 기업 생산성을 크게 높입니다. 멀티클라우드 및 분산 환경에 맞는 유연한 운영체계와 실시간 모니터링으로, 운영 자동화, 문제 진단, 대규모 배포 환경에서의 신뢰성과 보안성이 강화되었습니다.

### [정식 지원: Azure Container Storage v2.1.0 (Elastic SAN 연동)](https://azure.microsoft.com/updates?id=557912)
Kubernetes 클러스터의 스토리지 확장성과 중앙화 관리를 통해 다양한 워크로드 지원과 운영 부담 완화가 이루어집니다.

### [정식 지원: AKS 컨테이너 네트워크 로그](https://azure.microsoft.com/updates?id=557892)
네트워크 플로우 실시간 모니터링, 트래픽 패턴 분석, 문제 해결이 간편해져 운영 효율성이 증가합니다.

### [정식 지원: AKS 컨테이너 네트워크 메트릭 필터링](https://azure.microsoft.com/updates?id=557902)
관측 지점별 메트릭 관리로 운영 노이즈 제거, 실시간 상태 파악, 대시보드 구성의 효율성이 대폭 향상됩니다.