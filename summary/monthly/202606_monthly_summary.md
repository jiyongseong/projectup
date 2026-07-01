# Azure 월간 업데이트 요약 - 2026년 06월

## 전반적인 트렌드 및 핵심 인사이트

2026년 6월 Azure 업데이트는 AI 기반 서비스와 현대 애플리케이션 아키텍처의 진화가 전면에 부각된 시기입니다. Microsoft Build, Microsoft Foundry, 그리고 Fabric 연동을 중심으로 데이터, 인프라, 개발자 경험의 혁신이 지속적으로 이루어졌습니다. 특히 AI와 머신러닝 서비스의 기능 확장, 애플리케이션 통합 및 운영 자동화, 클라우드 네이티브 컴퓨팅의 강화, 그리고 보안과 거버넌스 측면에서의 새로운 지원이 두드러집니다.

1. **AI 및 데이터 중심의 혁신**  
   Azure Foundry와 Fabric이 중심적인 역할을 하면서 AI 모델의 관리·검색·구동, 대규모 데이터 처리 능력, 보안된 데이터 협업 환경(Confidential Clean Rooms), 자동화된 평가 및 최적화 기능 등 전 방위의 AI 관련 기능이 정식 또는 미리 보기 형태로 출시되었습니다. 이에 따라 개발자, 연구자, 그리고 기업들은 더 쉽게 모델 및 에이전트 개발 루프를 갖추고, RAG 기반 실무 및 복잡한 데이터 파이프라인을 실현할 수 있게 되었습니다.

2. **관리성·운영 효율성 증대**  
   Azure API Management, Logic Apps, Functions, Container Apps, Databricks, Kubernetes Fleet Manager 등 주요 서비스에 자동화, 커스텀 연동, 관리 편의성 개선이 적용되어, 개발·운영 팀은 복잡성과 비용을 줄이면서 더욱 안정적이고 민첩하게 서비스 배포 및 운영이 가능합니다.

3. **보안·규제 대응 강화**  
   Entra ID, Purview 감시와 민감 데이터 라벨링, 안전한 네트워크 연결, 분리된 백업 및 키 관리, 컨피덴셜 컴퓨트 확장 등 클라우드 보안과 거버넌스에 특화된 기능이 다양한 서비스에 정식 지원 또는 미리 보기로 포함되어, 특히 규제가 엄격한 산업 분야의 임직원들은 데이터 주권과 컴플라이언스 이슈를 효율적으로 관리할 수 있게 되었습니다.

4. **모듈화·코드 중심 개발 환경 확대**  
   VS Code, GitHub Copilot, API Center, API Builder, Functions 확장, Logic Apps 코드우선 워크플로우 등 개발자 중심의 사용성 개선과 AI 활용의 가속화가 두드러집니다. 모든 워크플로우를 코드로 작성하고 검증, 배포할 수 있도록 지원하며, AI 코드 어시스턴트가 실제 개발 업무의 생산성을 크게 높이고 있습니다.

5. **클라우드 인프라 구조 개편 및 친환경 전환**  
   VM 최적화, 새로운 리눅스 배포판, 파일 관리 모델, 스토리지 계정 구조 개편, VM 시리즈 및 네트워크 기능의 지원 종료 일정 발표 등 인프라 레벨의 지속적인 개편도 이어졌습니다. 자원 배치, 애플리케이션 연동, 스토리지 효율성을 극대화하면서도 기존 서비스의 전환을 유도하고 있습니다.

지속적으로 Azure는 인공지능, 데이터 처리, 현대적 애플리케이션 관리에서 선도적 지위를 강화하고 있으며, 이번 달은 RAG 기반 혁신, AI 모델 관리, 개발 자동화, 신규 스토리지·네트워크 옵션 등 다양한 분야의 기술적 진보가 집약된 시기입니다.

---

## ☁️ 인공지능 및 머신러닝 (AI + Machine Learning)

본 카테고리는 Azure Foundry, Azure AI Translator, Azure AI Search, Speech, Databricks 등 AI 관련 신규 기능과 출시 내용을 다룹니다.

1. [유니파이드 텍스트 번역 API 정식 지원](https://azure.microsoft.com/updates?id=563631)  
   다중 AI 번역 엔진(LLM 포함)으로 개발자들은 하나의 API에서 요구에 맞게 번역 엔진을 선택할 수 있습니다. 기존 v3와 호환되며, 지역별 데이터가 보존됩니다.

2. [Azure AI Search에서 GenAI 프롬프트 스킬 및 채팅 완성 기능 정식 지원](https://azure.microsoft.com/updates?id=563247)  
   인덱싱 중 채팅 모델 완성 스킬 호출로 콘텐츠 분류, 요약, 엔티티 정규화 등 자동화가 가능하며 인증과 비용 관리 기능까지 갖췄습니다.

3. [Azure Databricks와 OneLake 통합 정식 지원](https://azure.microsoft.com/updates?id=565733)  
   Unity Catalog를 활용해 데이터를 OneLake에서 직접 조회 가능, 향후 Fabric과의 데이터 공유/운영이 더욱 원활해집니다.

4. [LLM Speech API 정식 지원](https://azure.microsoft.com/updates?id=564387)  
   25개 언어, 90+ 지역을 아우르는 고도화된 AI 음성 인식·번역 기능이 도입되어 글로벌 대화와 분석이 용이해졌습니다.

5. [Text Analytics for Health NextGen Playground Microsoft Foundry 정식 지원](https://azure.microsoft.com/updates?id=563671)  
   임상 텍스트 분석과 FHIR 구조화 데이터 추출을 실시간으로 Playground에서 확인할 수 있습니다.

---

## 🖥️ 클라우드 인프라 및 컴퓨팅 (Compute/Containers/VM)

VM 최적화, 컨테이너관리, Functions, Kubernetes, 리눅스 관련 기능 및 지원 종료/전환 내용을 포함합니다.

1. [Azure NC RTX PRO 6000 Blackwell Server Edition v6 VM 정식 지원](https://azure.microsoft.com/updates?id=565271)  
   Nvidia Blackwell GPU와 Intel Xeon 6 CPU 기반으로 대규모 AI/그래픽 워크로드에 최적화, 아시아 및 미국 주요 리전 적용.

2. [Azure Container Linux(AKS) 정식 지원](https://azure.microsoft.com/updates?id=564537)  
   Flatcar 기반, 보안·불변성을 강조한 컨테이너 최적 OS로 노드 관리·통합 보안 지원.

3. [Azure Functions Node.js 24 지원 정식 배포](https://azure.microsoft.com/updates?id=562647)  
   Node.js 24 기반 앱 개발 및 배포가 가능해 최신 JS 생태계를 적극적으로 활용할 수 있습니다.

4. [Azure Kubernetes Fleet Manager for Arc-enabled clusters 정식 지원](https://azure.microsoft.com/updates?id=562904)  
   CNCF 기반의 멀티클라우드·온프레미스 Kubernetes 환경을 일원화 관리 및 워크로드 배치 자동화 가능.

5. [Premium SSD v2 디스크 비존(Zonal) VM 지원 확대](https://azure.microsoft.com/updates?id=565359)  
   단독 인스턴스에서도 SSD v2 사용 가능, 성능 개선 및 가격 효율성을 더 많은 워크로드에 적용 가능.

---

## ⚡ 데이터베이스 & 스토리지 (Database/Storage)

Cosmos DB, DocumentDB, PostgreSQL, MySQL 등 주요 데이터베이스 신기능/지원, 스토리지, 백업/장애처리, 관리 편의성 개선을 다룹니다.

1. [Azure Cosmos DB 전 버전 및 삭제 변경 피드 정식 지원](https://azure.microsoft.com/updates?id=562971)  
   모든 생성·수정·삭제 작업을 순차적으로 기록, 복제/감사/동기화 워크플로우에 활용.

2. [Azure Database for MySQL Flexible Server 자가 할당량 관리 기능](https://azure.microsoft.com/updates?id=563147)  
   개발·운영자가 직접 포털에서 할당량 조회 및 증설 요청, 처리 시간 단축.

3. [Azure SQL Database 플랫폼 Entra 서버 주체(로그인) 지원](https://azure.microsoft.com/updates?id=565154)  
   Entra ID 기반 인증·접근제어와 자동화된 유저/DB 프로비저닝이 가능해 보안 및 DevOps 관리가 강화됩니다.

4. [Azure Cosmos DB 글로벌 세컨더리 인덱스 정식 지원](https://azure.microsoft.com/updates?id=562799)  
   쿼리 성능 향상과 데이터 동기/검색 효율화, 다양한 워크로드 단절 없이 최적화.

5. [Azure Database for PostgreSQL 사전 업그레이드 검증 기능 미리 보기](https://azure.microsoft.com/updates?id=563786)  
   제품 업그레이드 전 호환성 검사·보고서 제공, 실패율과 운영 리스크 감소.

---

## 🔗 통합 및 관리 (Integration/Management/API/Migration)

API관리, Logic Apps, Azure Migrate, Event Grid 등 엔터프라이즈 통합, 워크플로우 자동화, 관측성 및 평가, 마이그레이션 기능과 지원 종료 및 전환 일정 발표를 포함합니다.

1. [Azure API Center 데이터 플레인 MCP 서버 정식 지원](https://azure.microsoft.com/updates?id=562914)  
   AI 자산과 API를 일원화된 엔터프라이즈 디스커버리 엔드포인트에서 관리, 통합·생태계 확장 용이.

2. [Azure Logic Apps MCP 서버 정식 출시](https://azure.microsoft.com/updates?id=562868)  
   기존 워크플로우를 MCP 도구로 노출, AI 에이전트가 자동화된 업무를 직접 호출 가능, 비즈니스 오케스트레이션 혁신.

3. [Azure Functions, Managed Connectors 미리 보기](https://azure.microsoft.com/updates?id=562442)  
   Office365, Teams, Salesforce 등 1400+ SaaS/서비스에 직접 연동·이벤트 기반 트리거 기능 강화.

4. [Azure Migrate와 GitHub Copilot Modernization 통합 미리 보기](https://azure.microsoft.com/updates?id=566145)  
   코드 통계 평가·현황 집계, 마이그레이션/현대화 판단을 AI 분석과 연동, 계획 효율 극대화.

5. [Azure Files 관리 모델 미정식 지원(NFS SSD)](https://azure.microsoft.com/updates?id=565062)  
   파일 레벨 네이티브 관리·보안, 대용량 스케일링과 비용 추적 기능.

---

## 🧩 Microsoft Foundry

Foundry 플랫폼, 모델 및 에이전트 관리, 도구 상자, 메모리 및 평가·관측성, VS Code 확장, 모델 카탈로그 등 혁신적인 AI 개발 환경과 연동 기능 전반을 정리합니다.

1. [Microsoft Foundry for Visual Studio Code 정식 지원](https://azure.microsoft.com/updates?id=563721)  
   프로젝트, 모델, 에이전트 관리 및 배포까지 통합, 코드-포털-운영 일원화.

2. [도메인 필터 및 툴 검색 기능 미리보기](https://azure.microsoft.com/updates?id=563731)  
   1,900+모델 중 특정 분야, 도메인 별 맞춤 필터링 및 에이전트 툴박스 내 검색 자동화.

3. [Foundry Memory 미리 보기 리프레시](https://azure.microsoft.com/updates?id=563616)  
   세션 및 사용자 스코프 메모리의 합리적 관리, 서드파티와 Foundry Agent 연동 강화.

4. [MCP Server Knowledge Source 및 연결 미리 보기](https://azure.microsoft.com/updates?id=563411)  
   Foundry IQ에서 Salesforce, Atlassian, Confluence 등 외부 데이터 연동 및 액세스 제어 일원화.

5. [User Feedback Logging 및 Trace Replay 미리 보기](https://azure.microsoft.com/updates?id=563426)  
   사용자 피드백과 운영 트레이스 시각화 연동, AI 에이전트 품질 관리·최적화 효율 상승.

---

## 🧑‍🔬 Microsoft Fabric

Fabric 및 OneLake, Mirroring, Databricks 연동 등 데이터 레이크 하우스·분석 플랫폼, RAG 파이프라인, 미러링 및 Power BI Direct Lake 연동, 신규 기능·지원 종료 내용을 정리합니다.

1. [OneLake 카탈로그·Fabric Ontology Knowledge Source 미리보기](https://azure.microsoft.com/updates?id=563416)  
   Fabric에서 OneLake 카탈로그 연결로 구조적·가버넌스 데이터 접근이 단일화.

2. [Mirroring for Microsoft Fabric로 Cosmos DB Synapse Link 지원 종료 시행](https://azure.microsoft.com/updates?id=558560)  
   Synapse Link의 종합적 기능을 Mirroring으로 전환, 더욱 확장된 분석 시나리오 지원.

3. [Azure Databricks OneLake 읽기/쓰기 및 Genie MCP 연동 정식/미리보기](https://azure.microsoft.com/updates?id=565733)  
   Databricks에서 OneLake 데이터 직접 조회 및 저장, Copilot Studio와 통합.

4. [Workspace-wide Genie MCP 엔드포인트 미리 보기](https://azure.microsoft.com/updates?id=564868)  
   Teams/M365 Copilot에서 Databricks 전체 데이터에 자연어 쿼리 가능, 데이터 가버넌스 강화.

5. [Fabric IQ Ontology Knowledge Source 미리 보기](https://azure.microsoft.com/updates?id=563416)  
   Fabric의 Ontology를 Foundry IQ에서 질의 가능, 비즈니스 정의와 AI 연동 신속화.

---

## 📅 지원 종료/사용 중단(Deprecation/Retirement)

VM 시리즈, 스토리지 계정, Synapse Link, VPN 클라이언트, Blueprints 등 Azure 플랫폼의 주요 지원 종료/전환 일정과 후속 조치 안내를 포함합니다.

1. [Azure Batch용 Av2/F/G/Lsv2 VM 시리즈 지원 종료(2028.11.15)](https://azure.microsoft.com/updates?id=564774)  
   기존 풀은 마이그레이션 필요, 신규 풀 생성 및 확장 불가. 대체 VM 사이즈 제시.

2. [Azure Load Balancer Inbound NAT Pool 버전 1 지원 종료(2027.09.30)](https://azure.microsoft.com/updates?id=565482)  
   NAT Pool 유형만 영향, v2로 마이그레이션 권장.

3. [Azure Synapse Link for Cosmos DB NoSQL 지원 종료(2029.03.31)](https://azure.microsoft.com/updates?id=558560)  
   신규 계정 Link 불가, Fabric Mirroring으로 전환 안내.

4. [Azure GPv1 및 Legacy Blob 스토리지 계정 생성 중단/자동 마이그레이션 안내(2026.10.13)](https://azure.microsoft.com/updates?id=564441)  
   GPv2로 자동 전환 예정, 비용 상승 주의.

5. [Azure Blueprints 서비스 지원 종료(2027.01.31)](https://azure.microsoft.com/updates?id=564806)  
   단계별 기능 종료, Azure Deployment Stacks로 전환 권장.

---

## 💡 기타 주요 업데이트

1. **서비스 관리 및 거버넌스**  
   Azure Monitor SLI/SLO, Dynamic threshold, OTEL Collector, Log Summary Rules, Metrics Usage Insights 대시보드 등 운영 품질 평가와 비용관리가 지속적으로 강화.

2. **보안 및 네트워크**  
   Azure NAT Gateway ICMP Ping, VPN Client 제거, 파일 스토리지 Entra ID 인증(macOS 포함), Microsoft Defender for Cloud 기능 전환 등 다양한 보안 정책 및 네트워크 접근 제어 강화.

3. **운영 자동화 및 DevOps**  
   자동 OS 이미지 업그레이드(VMSS Flex, 미리보기), Functions Rolling Update/Scale Rule Override, 서버리스 인덱서 등 자동화·무중단 운용 기능 확대.

---

## 총평 및 다음 달 전망

2026년 6월 Azure 업데이트는 AI/데이터 기반 서비스, 개발과 운영의 자동화, 보안 거버넌스 심화, 인프라 구조의 전략적 전환이 동시에 이루어진 점이 특징입니다. Foundry와 Fabric으로 AI 개발 및 데이터 연결이 “코드 융합”되는 경향이 강화되고 있으며, 기존 관리/운영 플랫폼은 API 및 커스텀 통합으로 더욱 유연해졌습니다.  
지원 종료 공지들이 계속 발표되고 있어 기존 인프라의 전환을 계획해야 하는 시기로 보입니다. 다음 달에는 Foundry, Fabric 기반 AI 실무 시나리오 확대, 컴플라이언스·보안 최적화, 개발자 경험 지속 개선, 하이브리드 클라우드 및 멀티리전 분산 아키텍처 강화가 예상되며, AI와 데이터 중심의 혁신적 업데이트가 계속될 전망입니다.  
기업은 기술 트렌드에 맞는 전략적 마이그레이션과 신기능 도입, 그리고 보안·거버넌스 체계 강화에 적극적으로 나서는 것이 바람직합니다.  
Azure는 AI, 데이터, 운영 효율성에서 꾸준히 혁신을 이어가며 시장 리더십을 공고히 할 것으로 보입니다.