# Azure 월간 업데이트 요약 - 2026년 05월

## 주요 트렌드 및 핵심 인사이트

2026년 5월의 Azure 업데이트는 ‘미리 보기’ 기능과 ‘정식 지원’ 기능 모두에 걸쳐 클라우드 네이티브 환경의 가속, 스토리지 서비스의 혁신, 네트워크 및 보안의 대대적 확장, 완전 자동화 관리와 협업 효율 증대라는 전반적인 흐름이 뚜렷합니다.

특히 AI 및 컨테이너 기반의 서비스와 인프라 관리 영역에서 자동화 및 보안을 혁신적으로 강화하는 기능과, 개발자∙운영자 모두를 위한 경험 최적화가 눈에 띕니다. 멀티 클라우드∙하이브리드 환경 지원은 더욱 정교해졌으며, 애플리케이션과 네트워크 설계의 유연성이 향상되고, 다양한 미리 보기 기능을 통해 대규모 확장/운영 시의 복잡성을 크게 줄이고 있습니다.

스토리지 영역에서는 Azure NetApp Files, Elastic SAN, Blob Storage 등 데이터 이동성, 확장성, 고성능 연계가 강조됐으며, 데이터 분석/AI 워크로드를 위한 연동성과 새로운 API·SDK 도입도 적극적으로 이루어졌습니다.

네트워크 부문에서는 가상 네트워크 관리·시뮬레이션 및 보안 규칙 영향 분석이 ‘운영 리스크 감소’와 ‘자동화된 정책 관리’라는 방향성을 보입니다. VPN, Front Door, Event Grid, Site-to-Site 인증 등 신뢰성과 보안, 실시간성, 통신 유연성이 빠르게 업그레이드되고 있습니다.

Azure Marketplace와 협력 생태계 강화를 위한 SaaS 서비스 즉시 활성화, 다수 파트너사 오퍼 관리 편의성도 강조되었으며, 중대한 지원 종료(Retirement) 공지와 함께 지속적인 서비스 혁신으로 이전 대비 한층 도약한 서비스를 예고합니다.

실제 적용 관점에서, 한국을 비롯해 다양한 지역에 맞춘 데이터 보호, 컴플라이언스, 보안, 네트워크 이중화 증진 역시 계속 진화하고 있음을 확인할 수 있습니다. 장기적 관점에서는 엔터프라이즈 AI/데이터 혁신, 클라우드 운영 자동화, 하이브리드 업무 환경 효율화가 앞으로의 Azure의 핵심 성장축임을 알 수 있습니다.

---

## 서비스 및 인프라

실제 클라우드 운영·사용성을 높이는 서비스/인프라 관련 주요 업데이트입니다.

### [Application Gateway for Containers – Istio 서비스 메시 통합](https://azure.microsoft.com/updates?id=564714)
Application Gateway for Containers와 Istio 서비스 메시의 정식 연동을 통해, 인증서 관리 자동화, 단일 진입점, 운영 복잡성 감소 등 클라우드 환경 내 마이크로서비스 보호와 신속한 서비스 연동이 강화되었습니다.

### [Azure Functions Durable Task Scheduler 소비형 SKU 출시](https://azure.microsoft.com/updates?id=560957)
Storage 관리나 용량 계획 없이도 내구성 있는 워크플로우/AI 오케스트레이션을 상황별로 사용할 수 있으며, 초당 과금 체계로 AI 에이전트, 데이터 파이프라인, 이벤트 구동형 업무에 매우 적합합니다.

### [Azure Front Door WebSocket 지원](https://azure.microsoft.com/updates?id=562548)
Front Door Standard 및 Premium에서 WebSocket이 기본 활성화되어 실시간 쌍방향 데이터 송수신이 필요한 대화형/게임/금융 등 시나리오에서 효율적이고 확장성 높은 아키텍처 구현이 가능합니다.

### [Azure Virtual Network Manager 규칙 영향 분석 GA](https://azure.microsoft.com/updates?id=562010)
보안 규칙 및 네트워크 구성 변경 시 실제 네트워크 트래픽에 미치는 영향을 사전 시뮬레이션하여 운영 안정성 및 취약점 관리 효율이 대폭 향상되었습니다.

### [Multiparty Private Offers, Microsoft Marketplace 30개국 확장](https://azure.microsoft.com/updates?id=563016)
Marketplace 파트너들이 다국적 고객/파트너와 협력적 클라우드∙AI 도입을 효율적으로 지원하도록 다자간 프라이빗 오퍼 적용 국가가 대폭 확대되었습니다.

---

## 스토리지 및 데이터 서비스

최신 스토리지, 데이터 관리 및 혁신적 활용 방안과 관련한 중요 소식입니다.

### [Azure Blob Storage SDK for Rust 출시](https://azure.microsoft.com/updates?id=562516)
보안, 신뢰성, 분산 추적 등 엔터프라이즈 품질 요구에 대응하는 Rust용 Blob Storage SDK가 정식 지원되어, 다양한 언어 기반의 통합 관리가 한층 강화되었습니다.

### [Azure NetApp Files 캐시 볼륨 정식 지원](https://azure.microsoft.com/updates?id=562259)
가장 빈번히 접근하는 데이터만 클라우드에 캐싱하여 WAN 지연 및 비용을 절감, 파일 배포 및 성능을 극대화하는 신규 캐시 볼륨 기능이 도입되었습니다.

### [Azure Elastic SAN 단일 볼륨 스냅샷 지원](https://azure.microsoft.com/updates?id=560899)
효율적이고 특정 시점 복구가 가능한 개별 SAN 볼륨 스냅샷 지원으로 백업·복원·이관 업무 신속화와 비용 효율성이 크게 높아집니다.

### [Azure Storage Mover Blob-to-Blob 마이그레이션 기능](https://azure.microsoft.com/updates?id=562753)
Azure Blob 간 직접 이동이 완전 관리형으로 제공되어 대규모 데이터 이전 및 병렬 동작, 가시적 관리가 매우 쉬워졌습니다.

### [Prefix-scoped User Delegation SAS 권한 부여](https://azure.microsoft.com/updates?id=561257)
SAS 토큰이 컨테이너·개별 Blob 외에도 가상 디렉터리 기반 범위로 확장되어, 대용량 멀티 테넌트 환경에서 접근 통제와 보안이 최적화됩니다.

---

## 네트워크 및 보안

네트워크 성능, 보안 정책, 관리 효율화와 관련된 중대 업데이트 중심입니다.

### [Site-to-Site VPN 인증서 기반 연결 지원](https://azure.microsoft.com/updates?id=562705)
기존 예비 공유키 대신 인증서 기반 신뢰 구축을 통한 암호화, 키 관리가 더 안전해져 하이브리드 네트워크 환경 보안 수준이 한층 강화되었습니다.

### [Azure Virtual Network NSG/라우팅 테이블 한도 상향](https://azure.microsoft.com/updates?id=562695)
NSG·라우팅 테이블 기본 용량이 늘어나 대규모 멀티티어 클라우드 아키텍처 설계 유연성과 확장성이 크게 개선되었습니다.

### [VPN Gateway P2S 사용자 그룹/IP Pool 관리](https://azure.microsoft.com/updates?id=564460)
원격 사용자별 별도 IP 풀 적용 및 Microsoft Entra ID 등 루트 기반 보안 관리로 사용자 세분화 및 접근 제어가 보다 정밀해졌습니다.

### [Virtual Network Flow 로그 Sentinel 연동](https://azure.microsoft.com/updates?id=564689)
네트워크 트래픽 로그가 실시간 보안 이벤트 감지 및 연관 분석 관제에 활용할 수 있어 운영 전반의 보안 가시성이 대폭 증대됩니다.

### [Network Watcher 룰 영향 분석 GA](https://azure.microsoft.com/updates?id=562690)
보안 그룹·운영 규칙 변경 영향도를 사전에 체계적으로 분석해 배포 전 위험요인 방지가 가능해졌습니다.

---

## 데이터 플랫폼 및 AI

클라우드 기반 데이터, AI, 분석 영역 혁신과 새로운 개발자 경험을 다룬 소식입니다.

### [Azure Cosmos DB LangChain/Azure CosmosDB 파이썬 패키지 지원](https://azure.microsoft.com/updates?id=562074)
AI/에이전트 기반 서비스가 Vector/Hybrid 검색, 대화 이력, 캐시, 체크포인트까지 단일 Cosmos DB 상에서 구현 가능, 확장성과 효율적 상태 관리에 특화된 개발 환경이 강화되었습니다.

### [Azure Event Grid MQTT/구독 ID 확장](https://azure.microsoft.com/updates?id=562240)
MQTT Retain, Shared Subscription, HTTP Publish 등 IoT, 실시간 메시징 통합이 더욱 강력해졌으며, 미리 보기로 Subscription Identifier 도입 등 개발자의 활용성이 극대화됐습니다.

### [Azure Monitor Application Insights 자동 계측 AKS 앱 지원](https://azure.microsoft.com/updates?id=562049)
코드 변경 없이도 자바/Node.js 워크로드를 자동 모니터링·분석, 분산 추적, 장애 진단 등 클라우드 네이티브 모니터링 경험이 대폭 개선되었습니다.

### [Azure SQL Managed Instance Business Critical 크기 자동 최적화(미리 보기)](https://azure.microsoft.com/updates?id=560283)
과다 프로비저닝 없이 인스턴스 성능을 최적화하는 자동화 기능으로 운영 비용 최적화 및 DbaaS 전략 이점이 늘어났습니다.

### [Azure Cosmos DB 쉘(미리 보기)](https://azure.microsoft.com/updates?id=561162)
AI 기반 MCP 활용의 스마트 CLI 도입으로 쿼리, 관리, 탐색 효율이 대폭 증진되었고, 시각적·코딩 동시 지원까지 혁신적인 개발자 경험을 제공합니다.

---

## 관리, 거버넌스 및 마이그레이션

관리 효율화, 가시성, 마이그레이션 체계 강화 내 업데이트입니다.

### [Azure Storage Mover 내장 일정 관리 기능](https://azure.microsoft.com/updates?id=562622)
마이그레이션 작업의 자동 스케줄링(예약, 반복)이 지원되어 반복적 동기화, 단계적 이관, 야간 스케줄 등 기업 운영 효율성이 강화되었습니다.

### [Azure NetApp Files Object REST API 정식 지원](https://azure.microsoft.com/updates?id=562254)
S3 호환 REST API 도입으로 데이터 복제/이동 없이 쉽게 Microsoft Fabric, Azure AI 등 다양한 최신 플랫폼과 연동 및 분석이 가능해집니다.

### [Azure Site Recovery, Performance Plus 지원(미리 보기)](https://azure.microsoft.com/updates?id=564644)
ASR이 프리미엄 디스크의 고성능 옵션까지 지원하여 운영 및 재해 복구 전체의 신뢰성과 일관성이 한층 높아졌습니다.

### [Azure Backup VM 일괄 복구(미리 보기)](https://azure.microsoft.com/updates?id=561373)
최대 100개 VM 동시 복구로 장애, 랜섬웨어 등 대규모 리커버리 상황 대응 속도와 관리 편의성이 대폭 향상되었습니다.

### [Azure Storage Actions 모의 실행(Mock Run) 기능](https://azure.microsoft.com/updates?id=559494)
대용량 데이터 작업을 실제 실행 없이 시뮬레이션·보고서 생성이 가능해, 사전 검증을 통한 운영 안정성 및 규정준수 체계를 강화하였습니다.

---

## 지역 (한국 등) 주요 업데이트

한국 및 특정 지역 중심의 변화·지원 강화를 정리했습니다.

### [Azure Service Bus Premium 기밀 컴퓨팅 – Korea Central 지원](https://azure.microsoft.com/updates?id=561942)
Azure Service Bus Premium에서 하드웨어 기반 신뢰 실행 환경(TEE) 내 메시지 처리가 한국중부 리전에 제공되어, 암호·키 관리, 데이터 사용 시 보안까지 포괄적 보안 환경을 제공합니다.

---

## Microsoft Foundry / Microsoft Fabric

### Microsoft Foundry

#### [Microsoft Foundry 내장 RBAC 역할 명칭 및 관리 강화](https://azure.microsoft.com/updates?id=562533)
Foundry 역할 네이밍 통일 및 워크로드별 역할 할당 기능이 개선되어, AI 관련 프로젝트 관리 및 배포, 권한 관리가 명확하고 유연해졌습니다.

---

## 주요 지원 종료 및 중단 (Retirement/Deprecation)

현 시점 Azure 환경에서 반드시 확인해야 할 지원 종료 내용 및 향후 조치 항목입니다.

### [Azure Document Intelligence v3.0 API, 2029년 3월 30일 종료](https://azure.microsoft.com/updates?id=561176)
해당 일자 이후 v4.0 이상으로 이전이 필요하며, 지원 종료 후 더 이상 서비스 불가함에 유의해야 합니다.

### [Azure App Service/Functions/Logic Apps – TLS 1.0, 1.1 2027년 5월 31일 지원 종료](https://azure.microsoft.com/updates?id=557852)
2027년 5월 이후 TLS 1.2 이상만 연결 가능하며, 기존 레거시 암호화 환경은 반드시 업그레이드 필요합니다.

### [Azure 예약형 VM 대상 시리즈 일부 RI 판매/갱신 종료, 2026년 7월 1일](https://azure.microsoft.com/updates?id=560948)
해당 날짜 이후 RI 만료 시, 자동 갱신 불가 및 PAYG로 자동 전환되므로 미리 신규 VM 시리즈(업그레이드) 또는 비용 전략 수립이 필수입니다.

---

## 이번 달 총평 및 다음 달 전망

2026년 5월 Azure 업데이트는 클라우드 인프라의 ‘운영 단순성, 자동화, 신뢰성’ 강화에 집중되며, 데이터·네트워크·보안·개발 현장 전반에서 생태계 확장과 기술 최적화의 실질적인 진전을 보여주었습니다. 미리 보기 기능의 빠른 현장 적용, 하이브리드/분산 환경에 최적화된 관리 효율, AI 및 서비스 혁신 가속화가 상호 맞물려 Azure 플랫폼 전체에 파급효과를 낳고 있습니다. 지원 종료(리타이어먼트)와 새로운 정책의 선제적 공지는 장기적인 서비스 체계 안정화를 위한 준비로 해석할 수 있습니다.

다음 달에도 Azure는 신규 인텔 기반 VM, 보안·지능형 네트워크, 데이터 연계 혁신 기능이 추가될 전망이며, 특히 데이터 통합/AI 플랫폼, 한국 등 주요 리전의 현지화 고객 지원, 멀티클라우드 확장 관련 소식이 이어질 것으로 기대됩니다. 규모 확장과 심플함, 보안/운영의 동시 혁신이 주된 키워드로 자리 잡을 것으로 예상됩니다.