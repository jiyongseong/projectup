# Azure 월간 업데이트 요약 - 2026년 05월

## 2026년 5월 Azure 업데이트 트렌드 및 핵심 인사이트

2026년 5월 Azure의 주요 트렌드는 ‘클라우드 인프라 혁신 가속화’, ‘플랫폼 자동화와 개발자 생산성 향상’, ‘제로 트러스트 기반 보안 강화’로 요약됩니다. 첫째, 클라우드 인프라 측면에서 네트워크·저장소·컴퓨팅 모두 주요 기능이 대폭 강화되었습니다. Azure NetApp Files의 대용량 파일 지원, Elastic SAN의 스냅샷 및 VMware 환경의 확장, Storage Mover의 에이전트리스 Blob 마이그레이션 등이 대표적입니다. 새로운 Dl/D/E v7 VM은 인공지능 워크로드 및 고성능 처리를 위한 인프라의 변화를 보여줍니다.

둘째, 개발자 생산성과 운영 자동화 강화를 위한 기능 릴리스가 두드러집니다. Application Insights의 자동 계측, App Configuration의 기능 평가 스코어카드, Azure Container Apps Express와 같은 관리형 경험 중심의 서비스들이 자동화 및 운영 편의성을 크게 개선하며, 마켓플레이스의 SaaS 자동 활성화, 멀티파트너 오퍼 등의 수익화 모델 혁신도 주목됩니다.

셋째, 보안과 거버넌스 강화 역시 큰 흐름입니다. VPN Gateway와 Application Gateway 등 네트워크 레이어의 모듈별 강화는 물론, Service Bus Confidential Computing의 정식 지원, Azure Files의 Entra Only Identity 및 Managed Identity SMB 지원과 TLS 1.0/1.1 지원 종료 등 데이터·네트워크·접근제어 전반에서 제로 트러스트를 실제로 구현하는 움직임이 힘을 받고 있습니다.

특히 미리 보기(Preview) 기능의 확장도 활발합니다. Site Recovery의 고성능 디스크 지원, AKS 애드온 자동화, App Service 및 Functions에서 Java 25 지원, Cosmos DB 우벡터/쉘, NetApp Files 기본 백업 등은 운용 및 개발 현장에 곧 체감될 변화입니다. 더불어, 한국(코리아 중부) 리전에서 Confidential Service Bus 정식 지원이 시작되어, 국내 산업·공공 분야의 메시징 보안 수요에도 실질적 혁신이 기대됩니다.

이상의 흐름에는 AI 인프라 혁신, 하이브리드 및 멀티클라우드 확대, 그리고 금융/공공/제조 등 규제 산업 대응 역량 강화라는 글로벌 트렌드가 심층 반영되어 있습니다.

---

## 컴퓨팅 및 인프라스트럭처 🖥️

이번 달에는 고성능 컴퓨팅, VM, 컨테이너 인프라, 하이브리드 솔루션 및 자동화 관련 주요 업데이트가 다수 이루어졌습니다. 최신 세대 VM 시리즈, Function·앱서비스 보안 강화, 자동화 기능 확대가 중요한 이슈입니다.

### [Azure Dl/D/E v7 Virtual Machines](https://azure.microsoft.com/updates?id=560734)
6세대 인텔 Xeon 기반 최신 VM 시리즈가 정식 지원에 들어갔습니다. 더 많은 vCPU와 메모리, 향상된 IOPS와 네트워킹 등 고성능 워크로드에 최적화된 환경이 제공됩니다.

### [Azure Functions durable task scheduler Consumption SKU](https://azure.microsoft.com/updates?id=560957)
Azure Functions에 내장 내구성 워크플로우 스케줄러가 Pay-per-use 과금 체계로 정식 지원됩니다. 인공지능 에이전트 기반 오케스트레이션 시나리오 등 대량 이벤트 기반 처리가 용이해집니다.

### [Azure Container Apps Express (미리 보기)](https://azure.microsoft.com/updates?id=559242)
컨테이너 앱 배포를 위한 최적화된 관리형 플랫폼이 미리 보기로 공개되었습니다. 인프라 설정 및 복잡도 없이 수초 내 배포가 가능, 개발자·에이전트에 집중된 애플리케이션 환경을 제공합니다.

### [Azure Site Recovery Support for Performance Plus Managed Disks (미리 보기)](https://azure.microsoft.com/updates?id=564644)
고성능 관리 디스크(Performance Plus) 기반 VM의 Azure Site Recovery 지원이 미리 보기로 제공되어, 재해 복구 시 성능 일관성과 대용량 워크로드 복원에 유리합니다.

### [Azure Cosmos DB Shell (미리 보기)](https://azure.microsoft.com/updates?id=561162)
AI 기반 명령줄 환경을 제공하는 Cosmos DB Shell(에이전트 지원)이 미리 보기로 등장, 운영 및 데이터 분석 자동화가 강화됩니다.

---

## 네트워킹과 보안 🌐

네트워킹 구조 혁신, 보안 정책 강화, 인입·연결성 개선 등 전방위적인 네트워크 환경 발전이 이루어졌습니다. 정책 및 트래픽 분석, VPN 인증, Service Mesh 등 최신 수요에 중점을 두었습니다.

### [Application Gateway for Containers – Service Mesh integration with Istio](https://azure.microsoft.com/updates?id=564714)
Istio 서비스 메시 통합이 정식 지원되어, AKS 내·외부 서비스로 착신 시 보안 정책 및 mTLS 관리를 자동화할 수 있습니다.

### [site-to-site VPN connections with certificate authentication](https://azure.microsoft.com/updates?id=562705)
디지털 인증서(비대칭키)를 활용한 사이트 간 VPN 연결이 정식 지원, 암호화 및 인증 강화로 제로 트러스트 네트워크 모델 구축에 기여합니다.

### [Azure Virtual Network Manager rule impact analyzer](https://azure.microsoft.com/updates?id=562010)
네트워크 관리 규칙(보안 관리자 룰) 영향 시뮬레이션 기능 제공, 트래픽 흐름 예측으로 장애 예방 및 유지보수 리스크 관리 역량이 크게 향상됩니다.

### [User Groups and IP address pools for P2S connections](https://azure.microsoft.com/updates?id=564460)
VPN Gateway Point-to-Site 연결에서 사용자 그룹별로 고유한 IP 풀 할당이 가능해져, 세분화된 네트워크 접근 제어 및 규정 준수에 유리합니다.

### [Summarized advertised gateway prefixes for route advertisement (미리 보기)](https://azure.microsoft.com/updates?id=562813)
ExpressRoute 및 VPN Gateway 경로 요약 광고를 통한 온프레미스 연동 편의성과 확장성 증대, 대규모 하이브리드·멀티클라우드 아키텍처 환경에 최적화된 네트워크 설계가 가능해집니다.

---

## 저장소 및 데이터 플랫폼 💾

스토리지 영역에서는 대용량 데이터 지원과 하이브리드 연동, 구체적 마이그레이션 자동화가 핵심입니다. NetApp Files, Elastic SAN, Blob Storage, 파일 마이그레이션 등에서 굵직한 변화가 이어졌습니다.

### [Azure NetApp Files cache volumes](https://azure.microsoft.com/updates?id=562259)
클라우드 기반 캐시 볼륨 지원으로 데이터 처리 속도와 사용자 접근성이 크게 향상, WAN 및 ExpressRoute 대역폭 비용 절감 효과도 기대됩니다.

### [Azure Blob Storage SDK for Rust](https://azure.microsoft.com/updates?id=562516)
생산 환경 수준의 Rust SDK가 정식 제공, Rust 개발 생태계 내에서 안트라 인증, 자동 재시도, 분산 트레이싱 적용이 본격화됩니다.

### [Azure Elastic SAN 지원: Single Volume Snapshots, AVS 연동 등](https://azure.microsoft.com/updates?id=560909)
Elastic SAN에서 단일 볼륨 스냅샷 지원, VMware Solution(AVS) 내 Gen2 및 대형 데이터 처리 워크로드의 저장소 옵션이 획기적으로 개선되었습니다.

### [Azure Storage Mover Blob-to-Blob migration](https://azure.microsoft.com/updates?id=562753)
Blob 컨테이너 간의 대용량 데이터 마이그레이션을 에이전트 없는 완전관리형으로 지원하며, 대량 데이터 및 병렬 작업을 안전하게 처리할 수 있습니다.

### [Mock runs for Azure Storage Actions – Validate before you execute](https://azure.microsoft.com/updates?id=559494)
스토리지 작업의 실행 전 사전 검증(모크 런) 지원, 정책·비용·컴플라이언스 위험을 최소화하는 저장소 관리 자동화 강화입니다.

---

## 관리, 운영, 거버넌스 ⚙️

관제 및 정책, 자원 최적화, 마켓플레이스 개선 등 관리/운영 노하우 강화를 위한 업데이트가 집중되었습니다. 기술 지원/정책 유연성, 그리고 가시화 기능이 발전되었습니다.

### [Auto activation for SaaS subscriptions in Microsoft Marketplace](https://azure.microsoft.com/updates?id=561771)
Azure Marketplace에서 SaaS 자동활성화가 적용, 구매 즉시 사용 및 과금 시작으로 파트너·고객 모두에게 즉시적인 서비스를 제공합니다.

### [Multiparty private offers in Microsoft Marketplace expand to 30 countries in Europe](https://azure.microsoft.com/updates?id=563016)
Marketplace에서 멀티파트너(공동 제안) 확장이 대폭 확대되어, 다양한 유럽 국가에서 파트너의 클라우드·AI 솔루션 공동 확대/납품 구조가 현실화됩니다.

### [Azure App Configuration Scorecards (미리 보기)](https://azure.microsoft.com/updates?id=561049)
App Configuration에서 기능 배포 효과 측정을 위한 스코어카드 텔레메트리 뷰가 제공되어, 운영 환경에서의 기능별 KPI/효과 검증이 데이터 기반으로 가능해집니다.

### [Bulk Restore for Azure Virtual Machines using Azure Backup (미리 보기)](https://azure.microsoft.com/updates?id=561373)
VM 일괄 복원(Bulk Restore) 기능이 미리 보기로 제공, 장애/랜섬웨어 대응 등 대규모 복구 업무 효율성이 향상됩니다.

### [Update: Egress and data transfer with Azure in the United Kingdom](https://azure.microsoft.com/updates?id=561392)
영국 내 데이터 송수신/청구 정책 변경이 공지되어, 영국 리전 고객 및 CSP 파트너의 비용·규정 관리에 유의해야 함을 알리고 있습니다.

---

## AI, 데이터베이스, 개발자 도구 🤖

AI 및 데이터 플랫폼, 개발자 생산성 지원(통합·SDK·추론 등)과 최신 DB 기능이 강화되었습니다. Microsoft Foundry, Cosmos DB, Function AI, 분산 트레이싱 등 최신 트렌드가 반영되었습니다.

### [langchain-azure-cosmosdb python package for Azure Cosmos DB](https://azure.microsoft.com/updates?id=562074)
LangChain 및 LangGraph 오케스트레이션의 Cosmos DB 연동 패키지 정식 릴리스, 벡터·하이브리드 검색, 캐시·에이전트 메모리 통합 구현이 가능해졌습니다.

### [Azure Cosmos DB Shell(미리 보기)](https://azure.microsoft.com/updates?id=561162)
AI 기반 명령줄 도구 제공, 대규모 데이터를 에이전트 지원 워크플로우로 효율적으로 관리할 수 있습니다.

### [Azure Cosmos DB spherical quantization for improved vector search (미리 보기)](https://azure.microsoft.com/updates?id=561167)
고도화된 벡터 인덱싱(구형 양자화, Spherical Quantization) 기능 미리 보기 도입으로 AI 기반 검색 품질과 성능이 강화됩니다.

### [Azure SQL update for early-May 2026 (미리 보기)](https://azure.microsoft.com/updates?id=560283)
Business Critical 플랜용 Azure SQL Managed Instance의 메모리 적정화(오버프로비저닝 방지)로 가격 경쟁력 및 성능이 개선되고 있습니다.

### [Azure Front Door WebSocket](https://azure.microsoft.com/updates?id=562548)
실시간/저지연 통신 기능(웹소켓) 정식 지원으로, 대화형 앱·실시간 대시보드/게임 등 연속 데이터 워크로드에서 활용도가 높아집니다.

---

## Microsoft Foundry & Microsoft Fabric 🏭

Azure AI 기반 데이터 및 개발자 생산성을 위한 핵심 플랫폼인 Microsoft Foundry/Fabric 관련 업데이트도 포함됩니다.

### [Microsoft Foundry built-in RBAC role naming and enhancements](https://azure.microsoft.com/updates?id=562533)
Foundry 역할 명칭이 서비스 브랜드와 일치하도록 변경되었으며, 계정/프로젝트 소유자 권한 위임 및 관리 기능이 향상되었습니다. 복잡한 워크플로우에서의 역할 배분이 유연해집니다.

---

## 한국(Korea Central, Korea South) 리전 관련 🇰🇷

이번 달 한국 리전에는 데이터 보호와 기밀성 측면의 특징적 변화가 있었습니다.

### [Confidential computing for Azure Service Bus Premium – Korea Central](https://azure.microsoft.com/updates?id=561942)
Service Bus Premium의 기밀 컴퓨팅(Confidential Computing)이 한국 중부 리전에서 정식 지원됩니다. 하드웨어 기반 실행 환경에 메시지가 격리 저장되고, 기존 앱 호환/변경 없이 최고의 보안 등급을 누릴 수 있습니다.

---

## 지원 종료 및 사용 중단 ⛔️

보안 및 서비스 아키텍처 변화에 따라, VM 예약 인스턴스, TLS 1.0/1.1 등 일부 기능의 지원 종료/사용 중단이 공지되었습니다. 데이터 마이그레이션과 보안 테스트 등 사전 조치가 필요합니다.

### [TLS 1.0과 TLS 1.1 지원 종료](https://azure.microsoft.com/updates?id=557852)
2027년 5월 31일 이후 App Service, Functions, Logic Apps에서 TLS 1.0/1.1 프로토콜 연결이 완전 중단됩니다. 조직 내 모든 클라이언트 및 서비스가 TLS 1.2 이상을 지원하는지 반드시 점검/전환해야 합니다.

### [Azure Document Intelligence v3.0 API 지원 종료 (2029년 3월 30일)](https://azure.microsoft.com/updates?id=561176)
Azure Document Intelligence API v3.0이 2029년 3월 지원 종료, 반드시 v4.0 이상으로 서비스 마이그레이션이 필요합니다.

### [Azure Reserved Virtual Machines Instances(일부 VM 시리즈) 지원 종료](https://azure.microsoft.com/updates?id=560948)
Av2, D, F, L 등 구형 VM 시리즈 예약 인스턴스의 신규 구매 및 갱신이 2026년 7월 1일부터 종료됩니다. 만료 전 신규 VM 시리즈로 전환 필요.

---

## 2026년 5월 업데이트 총평 및 6월 전망

2026년 5월 Azure 업계는 대규모 인프라 혁신, 개발자 자동화, 네트워크 및 데이터 보안의 실질적 강화라는 3대 축으로 뚜렷한 발전을 이뤘습니다. 최신 VM 및 스토리지의 인텔 기반 고도화, 컨테이너 앱 자동화, 네트워킹 룰 시뮬레이션 및 보안 강화 등은 기업의 운영 안정성과 혁신 속도를 동시에 크게 높여주는 요소로 자리 잡았습니다. 한편, 한국을 포함한 리전별 특화 보안 모델의 확장은 규제 산업 및 민감 데이터 처리 서비스 영역에서 차별점을 부각시키고 있습니다.

다가오는 6월에는 Data + AI 플랫폼 고도화와 애플리케이션 관리 간소화, 그리고 하이브리드/멀티클라우드 기반 실시간 데이터 활용·거버넌스 자동화 흐름이 더욱 강화될 것으로 전망됩니다. Microsoft Fabric/Foundry 생태계 연동, AI·Agent 인프라 관리 및 규제준수 지원이 핵심 이슈가 될 개연성이 높습니다. 급변하는 클라우드 혁신 현장에서 Azure 플랫폼의 민첩한 변화를 지속 모니터링할 필요가 있습니다.