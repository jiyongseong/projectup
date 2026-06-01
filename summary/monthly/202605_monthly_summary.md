# Azure 월간 업데이트 요약 - 2026년 05월

## 전반적인 트렌드 및 핵심 인사이트

2026년 5월 Azure 업데이트에서는 **클라우드 네이티브 인프라의 효율성과 자동화**, **데이터 및 보안 중심 혁신**, **보편적 확장성**, **개방성 및 언어 다양성**이 핵심 트렌드로 두드러집니다. 정식 지원(GA) 출시가 대다수를 차지하는 한편, 미리 보기(preview)와 일부 지원 종료(retirement) 공지 역시 활발하게 이루어졌습니다.

특히 자동화와 관리 간소화, 보안 고도화에 초점을 맞춘 서비스 기능들이 대거 발표되었습니다. 예를 들어 Azure Storage, Blob, SAN 등 스토리지 영역에서는 대용량 데이터 및 고성능 워크로드 지원이 한층 강화되었으며, NetApp Files, Elastic SAN, Storage Mover 등의 신규 기능과 데이터 이동성, 효율적 관리가 강조되었습니다. 애플리케이션 게이트웨이, 네트워크 관리자, VPN, Event Grid 등 네트워킹 서비스에서도 운영자 경험을 대폭 단순화하는 업데이트와, 실시간 메시지 처리 및 다양한 MQTT 기능 확장이 눈에 띕니다.

보안 면에선 애플리케이션/네트워크 접근제어, 인증 모델 혁신, Confidential Computing 확장 등 데이터 보호와 규제 준수 컴플라이언스가 두드러집니다. VM, 컨테이너, 데이터베이스 등 각 영역별로도 최신 인텔 기반 VM(GRANITE RAPIDS) 도입, 자동 인스트루먼테이션, Rust SDK 본격화, LangChain-Cosmos DB Python 패키지 연동 등 개발 환경과 언어 지원의 폭이 넓어지고 AI 내재화가 확대되고 있습니다.

미리 보기(preview) 영역은 AKS Application Gateway, Cosmos DB Shell, NetApp Files 자동 백업, Site Recovery 고성능 디스크 등 혁신적 시도가 활발하며, 지원 종료(retirement) 부문에서는 TLS 1.0/1.1, 특정 VM RI 일부 및 Document Intelligence v3.0 등이 예고되어 선제적 대응이 필요합니다. 앞으로도 Azure는 **보안, 자동화, 데이터 거버넌스, 글로벌 확장성**이라는 네가지 축에서 안정성과 혁신을 동시에 추구하는 플랫폼 방향성을 이어갈 전망입니다.

---

## ☁️ 컴퓨트(Compute), 가상 머신 및 서버리스

2026년 5월, Azure 컴퓨트 업데이트는 새로운 인텔 프로세서 기반의 VM, 서버리스 기능의 고도화, 예약 인스턴스(RI) 지원 종료 등 인프라 변화에 초점을 맞췄습니다.

### [Azure Dl/D/E v7 Virtual Machines](https://azure.microsoft.com/updates?id=560734)
최신 Intel Xeon 6(Granite Rapids) 기반의 v7 VM 시리즈가 정식 지원됩니다. 기존 v6 대비 최대 20% 성능향상과 최대 372 vCPU, 2.8 TiB 메모리 확장, 최대 9.6M IOPS 등 대규모 워크로드에 적합합니다.

### [Azure Functions durable task scheduler Consumption SKU](https://azure.microsoft.com/updates?id=560957)
서버리스 기반 내구성 워크플로우 실행에 더해, 사용량 기반 과금모델이 제공되어, AI 오케스트레이션, 이벤트 기반 파이프라인 등에 비용효율적 구성이 가능합니다.

### [Generally Available: Azure Functions support for Java 25](https://azure.microsoft.com/updates?id=560879)
Azure Functions에서 Java 25를 로컬 개발, 리눅스/윈도우, Flex Consumption 등 다양한 환경에서 공식 지원합니다. 최신 Java 언어의 보안, 성능을 직접 활용할 수 있습니다.

### [Azure Premium SSD v2 Disk 일본 서부 3개 존 지원](https://azure.microsoft.com/updates?id=561814)
고성능, 저지연 스토리지인 Premium SSD v2가 일본 서부 전체 가용 존에서 정식 출시되었습니다. SQL, SAP, Cassandra 등 다수의 엔터프라이즈 워크로드를 지원합니다.

### [Azure Reserved Virtual Machines Instances for select VM series 지원 종료 예고](https://azure.microsoft.com/updates?id=560948)
2026년 7월 1일부터 Av2, D, F, G 등 일부 VM 시리즈의 1/3년 예약 인스턴스 구매/갱신이 불가합니다. 미리 워크로드와 RIs 상태를 점검하여 자동 갱신 중단 및 신규 VM 전환을 준비해야 합니다.

---

## 🛠️ 데이터베이스 및 스토리지 

스토리지 및 데이터 서비스는 확장성과 자동화, 멀티 워크로드 지원 중심의 혁신이 이어집니다. 다양한 벡터, 오브젝트, 자동화 기능이 업데이트되었습니다.

### [Azure Blob Storage SDK for Rust 정식 지원](https://azure.microsoft.com/updates?id=562516)
Rust 언어 SDK로 Blob/컨테이너 작업, Entra 인증, 자동 재시도, OpenTelemetry 추적 등 고성능 데이터 접근이 가능합니다.

### [Azure Storage Mover Blob-to-Blob migration](https://azure.microsoft.com/updates?id=562753)
Blob 컨테이너 간 에이전트리스, 병렬 전송 및 대규모 디렉터리 이동이 완전 관리형 환경으로 제공되어 데이터 워크로드 이동에 혁신을 제공합니다.

### [Azure NetApp Files object REST API](https://azure.microsoft.com/updates?id=562254)
NetApp Files 데이터에 S3호환 REST API를 제공, Microsoft Fabric, Azure AI 서비스와 연동이 쉬워지고, 데이터 변환/복제 없이 데이터 비즈니스 활용이 가능합니다.

### [Single Volume Snapshots on Azure Elastic SAN](https://azure.microsoft.com/updates?id=560899)
Elastic SAN 단일 볼륨 단위로 증분 스냅샷이 제공되어, 백업/복구/장기보관이 용이해졌습니다.

### [Mock runs for Azure Storage Actions](https://azure.microsoft.com/updates?id=559494)
스토리지 작업 실행 전, 대규모 시뮬레이션 및 영향 리포트 기능이 추가되어, 데이터 관리 자동화의 신뢰도를 대폭 제고합니다.

---

## 🔗 네트워킹, 보안 및 인테그레이션

보안·네트워킹에서는 운영 효율성, 자동화, 세분화된 접근제어, 실시간 메시징 고도화가 주요 흐름입니다.

### [Application Gateway for Containers – Istio 서비스 메쉬 통합](https://azure.microsoft.com/updates?id=564714)
Istio 및 AKS Istio 서비스 메쉬 통합이 정식 지원되어, 단일 인그레스 솔루션, 자동 mTLS, 인증서 수명주기 관리 등 보안 및 운영 간소화가 실현됩니다.

### [Azure Virtual Network Manager rule impact analyzer 정식 지원](https://azure.microsoft.com/updates?id=562010)
보안 규칙, NSG, 라우트 테이블 변경 전, 실시간 트래픽 영향 시뮬레이션이 가능해져 가상 네트워크 운영 안정성이 크게 높아집니다.

### [site-to-site VPN connections with certificate authentication](https://azure.microsoft.com/updates?id=562705)
VPN Gateway에서 인증서 기반 인증을 지원, X.509 기반 상호 인증 구조로 보안성이 크게 높아집니다.

### [User Groups and IP address pools for P2S connections](https://azure.microsoft.com/updates?id=564460)
P2S VPN 연결에서 그룹별로 고유 IP 풀 할당이 가능해져, 세분화된 접근 정책 수립 및 보안 규정 준수에 기여합니다.

### [Azure Front Door WebSocket 정식 지원](https://azure.microsoft.com/updates?id=562548)
실시간 양방향 통신(WebSocket)이 기본 활성화되어, 채팅, 대시보드, 게임 등 실시간 서비스에서 네트워크 효율성과 사용자 경험이 개선됩니다.

---

## 💾 관리, 모니터링 및 마이그레이션

관리자동화, 대시보드, 대용량 데이터 이동 지원 기능이 강화되었습니다.

### [Schedule one-time or recurring migrations with Azure Storage Mover](https://azure.microsoft.com/updates?id=562622)
스토리지 마이그레이션에 예약 및 반복 스케줄이 내장되어 데이터 이전 및 동기화 작업의 자동화와 일관성 확보에 유리합니다.

### [Azure Monitor Application Insights Auto-instrumentation for AKS](https://azure.microsoft.com/updates?id=562049)
AKS 앱에 대한 자동 인스트루먼테이션 도입으로 자바/Node.js 앱의 코드 수정 없이 손쉽게 모니터링이 가능해졌습니다.

### [Virtual network flow logs connector with Microsoft Sentinel](https://azure.microsoft.com/updates?id=564689)
가상 네트워크 플로우 로그를 Sentinel에 직접 연동해 통합 보안 분석, 자동 경보, 사고 대응이 더욱 진화했습니다.

### [Bulk Restore for Azure Virtual Machines using Azure Backup](https://azure.microsoft.com/updates?id=561373)
가상 머신 백업 대량 복구(최대 100개 동시)를 미리 보기로 도입, 대규모 장애/랜섬웨어 복구 시 업무 연속성을 보장합니다.

### [Azure SQL update for early-May 2026 – 비즈니스 크리티컬 Managed Instance 메모리 최적화](https://azure.microsoft.com/updates?id=560283)
비즈니스 크리티컬 MI의 메모리 크기 조정 옵션이 통해, 과도한 오버프로비저닝 없이 성능 및 비용 최적화가 가능합니다.

---

## 🗄️ 개발 및 오픈소스, 도구 

SDK, 개발 언어, CICD 영역의 기능 개선과 새로운 통합 경험이 부각되고 있습니다.

### [langchain-azure-cosmosdb python package for Azure Cosmos DB](https://azure.microsoft.com/updates?id=562074)
LangChain 에이전트 및 LLM 애플리케이션에서 Cosmos DB의 벡터/하이브리드 검색, 대화 이력, 체크포인트 관리를 원스톱으로 활용 가능합니다.

### [Azure Cosmos DB Shell (미리 보기)](https://azure.microsoft.com/updates?id=561162)
AI 기반 워크플로우를 지원하는 CLI 도구가 선보여, 쿼리, 관리, 탐색을 더욱 효율화합니다.

### [Azure Functions Flex Consumption 인증서 관리 미리 보기](https://azure.microsoft.com/updates?id=562808)
Flex Consumption 플랜 개별 함수 앱 단위의 사이트 스코프 인증서 모델 미리 보기가 도입되어, 보안 앱 배포 자동화를 지원합니다.

### [Application Gateway for Containers managed add-on + AKS Automatic 미리보기](https://azure.microsoft.com/updates?id=558403)
AKS Automatic 환경에서 애플리케이션 게이트웨이 통합이 가능한 관리형 Add-on 미리 보기가 제공됩니다.

### [Evaluate feature rollouts with Azure App Configuration Scorecards](https://azure.microsoft.com/updates?id=561049)
피처 플래그 운영 성과와 문제점을 실시간 텔레메트리 기반으로 평가할 수 있는 Scorecards 기능이 미리 보기로 제공됩니다.

---

## 🔐 보안, 규정 준수 및 통합

서비스 메시지큐, 콘피덴셜 컴퓨팅, 멀티파티 오퍼 등 데이터 주권 및 규정 준수, 통합 강화에 방점이 찍혔습니다.

### [Confidential computing for Azure Service Bus Premium (Korea Central 지원)](https://azure.microsoft.com/updates?id=561942)
Service Bus 메시지 처리를 하드웨어 기반 신뢰 실행환경(TEE)에서 실행, 데이터 사용중 보호가 추가되며, Korea Central 리전 정식 지원이 시작되었습니다.

### [Multiparty private offers in Microsoft Marketplace 유럽 30개국 확장](https://azure.microsoft.com/updates?id=563016)
마켓플레이스에서 멀티파트너 사설 오퍼가 대폭 확대되어, 파트너 간 협업 및 고객별 맞춤형 오퍼링 전략에 유연성을 높였습니다.

### [Update: 99.99% uptime for all Azure Service Bus Premium namespaces in Availability Zone regions](https://azure.microsoft.com/updates?id=561947)
AZ(가용영역) 지원 리전에서 Service Bus Premium 네임스페이스의 SLA가 99.99%로 상향, 고가용성 및 중요한 워크로드에 최적화가 이루어졌습니다.

### [Entra-only identities with Azure Files](https://azure.microsoft.com/updates?id=562359)
AD 연동 없이 Entra ID만으로 SMB 접근 지원을 정식 출시, 권한 관리 단순화, 클라우드 네이티브 인증 구성을 실현합니다.

### [Managed Identity Support for Azure Files SMB 정식지원](https://azure.microsoft.com/updates?id=562350)
Azure Files에 관리형 ID 연동을 통한 비밀번호 없는 인증 및 RBAC 기반 세분화 접근제어가 정식 도입되었습니다.

---

## 🏢 Microsoft Foundry & 🟧 Microsoft Fabric

### Microsoft Foundry
#### [Built-in RBAC role naming and enhancements](https://azure.microsoft.com/updates?id=562533)
역할명칭 일원화와 관리 기능 확장, 워크플로우별 조건부 액세스, 추적 데이터 접근, 빌트인 RBAC 정책 고도화가 반영되었습니다.

### Microsoft Fabric
(별도 신규 업데이트 미포함/ NetApp Files object REST API/Fabric 연동은 데이터 카테고리 내 표기)

---

## 🇰🇷 한국 리전 관련 주요 업데이트

### [Confidential computing for Azure Service Bus Premium – Korea Central 지원](https://azure.microsoft.com/updates?id=561942)
Azure Service Bus Premium 서비스의 Confidential Computing 기능이 코리아 센트럴 리전에서 정식 지원되어, 국내 규제준수 및 민감 데이터 워크로드에 하드웨어 수준의 실시간 데이터 보호가 적용됩니다.

---

## 총평 및 다음 달 전망

2026년 5월 Azure 업데이트는 **보안 고도화와 인프라 효율화, 자동화, AI 내재화**가 중점적으로 반영되어, 클라우드 운영의 투명성·안정성·민첩성을 전방위적으로 한 단계 끌어올렸다고 볼 수 있습니다. 관리자·개발자 모두가 체감할 사용자 경험 및 거버넌스 개선, 글로벌 서비스 확장, 다양한 언어/플랫폼 지원이 차별점입니다.

다음 달 전망으로는, Arm/AI 인프라 연계, 멀티리전 데이터 거버넌스, AKS 및 클라우드 네이티브 도구 혁신, 산업별 워크로드(금융, 헬스케어 등) 특화 업데이트가 예상됩니다. 특히 대한민국 등 규제적 정책 변화에 따른 기능 출시에 관심을 기울여야 할 것으로 보입니다. Azure의 신속한 서비스 혁신 흐름에 맞춰 아키텍처, 운영, 보안 전략을 지속 점검할 것을 권고합니다.