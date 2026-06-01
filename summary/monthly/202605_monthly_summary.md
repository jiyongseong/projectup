# Azure 월간 업데이트 요약 - 2026년 05월

## 주요 트렌드 및 인사이트

2026년 5월, Microsoft Azure는 클라우드 인프라의 운영 효율성과 데이터 관리, 보안, 네트워킹, AI/머신러닝, 애플리케이션 현대화, 그리고 개발자 생산성에 중점을 둔 다양한 업데이트를 발표했습니다. Azure의 서비스 전반에 걸쳐 모듈화·자동화된 운용 방안이 확산되었으며, 최신 하드웨어 인프라와 AI 환경 지원 강화, 데이터 이동 및 통합의 단순화, 네트워크 관리는 물론, 엔터프라이즈 규모의 확장성과 컨테이너·서버리스 컴퓨팅 환경 개선, 그리고 개발자 생태계 개방 등이 두드러졌습니다.

특히 **네트워크와 보안** 환경에서 Application Gateway, VPN Gateway, Azure Virtual Network Manager와 같은 핵심 서비스의 정식 지원이 확대되어, 서비스 메쉬 통합, 자동 인증, 고도화 된 네트워크 분석 기능 및 정책 기반 가시성 강화가 이뤄졌습니다. 또한, Azure의 프라이빗 오퍼·마켓플레이스 확장 및 자동화, Azure NetApp Files·Elastic SAN 등 고성능 스토리지 서비스의 기능 진화, AKS·Application Insights·Azure Functions 중심의 클라우드 네이티브 모니터링과 관측성 개선이 강조되었습니다.

AI와 데이터 부문에서는 Cosmos DB와 NetApp Files의 AI·분석 서비스와 직접 연동 가능성이 확대되면서, 데이터 기반 솔루션의 비즈니스 가치 실현이 가속화될 것으로 전망됩니다. **한국 지역에서는 Confidential Computing for Azure Service Bus Premium 기능의 정식 지원이 발표되어, 데이터 보호 수준이 한 단계 높아졌습니다.**

업데이트들은 단순한 신기술 도입에 그치지 않고, 거버넌스 강화, 빌링 효율화, 보안 규정 준수, 운영 자동화에 대한 수요에 부합하는 형식으로 이루어진 점이 이번 달의 핵심 인사이트입니다.

---

## 1. ☁️ 인프라·컴퓨트(Compute/VM)

이번 달 인프라스트럭처·컴퓨트 부문은 최신 프로세서 기반의 VM 신제품 출시, VM 복구 자동화, 예약 인스턴스 정책 변화 등 대규모 워크로드 수용 및 TCO 최적화, 고가용성 인프라 운용 관점에서 의미 있는 진전이 있었습니다.

### [Azure Dl/D/E v7 Virtual Machines](https://azure.microsoft.com/updates?id=560734)
최신 Intel Xeon 6 기반의 v7 VM 시리즈 정식 지원. 최대 20%의 더 높은 컴퓨팅 성능, 최대 372 vCPU 및 2.8TiB 메모리, AI 추론 가속 및 차세대 스케일/스토리지/네트워킹 성능 제공.

### [Bulk Restore for Azure Virtual Machines using Azure Backup](https://azure.microsoft.com/updates?id=561373)
VM 대량 복구(최대 100개 동시) 기능 미리 보기 제공. 장애·랜섬웨어·장애 복구 시 빠르고 일관된 복원 자동화 지원.

### [Azure Reserved Virtual Machines Instances for select VM series 지원 종료](https://azure.microsoft.com/updates?id=560948)
2026년 7월 1일부터 일부 VM 시리즈(Av2, Dv2, F, Lsv2 등) 예약 인스턴스 신규·갱신 중단. 마이그레이션 가이드 제공 및 기존 리소스는 약정 종료 시점까지 유지.

### [Azure Premium SSD v2 Disk 일본 데이터센터 세 Availability Zone 지원](https://azure.microsoft.com/updates?id=561814)
일본 West 지역 내 모든 Zone에서 Premium SSD v2 제공. 고성능 블록 스토리지 및 미션 크리티컬 엔터프라이즈 워크로드 최적화.

### [Azure Functions support for Java 25 정식 지원](https://azure.microsoft.com/updates?id=560879)
Function 앱의 최신 Java 25 버전 지원 개시. Flex Consumption 등 다양한 호스팅 옵션에서 사용 가능.

---

## 2. 🔒 네트워크·보안

서비스 메쉬, 인증, 정책 자동화 등 대규모·다계층 네트워크 환경에서 운영 편의성과 보안·분석 기능이 집중적으로 강화되었습니다.

### [Application Gateway for Containers – Istio 서비스 메쉬 통합](https://azure.microsoft.com/updates?id=564714)
서비스 메쉬 보안 연결(mTLS) 및 인증서 자동 관리, Istio-기반 AKS 서비스와 즉시 통합, Ingress 경로 일원화 등 클라우드 네이티브 아키텍처 효율 증대.

### [site-to-site VPN connections with certificate authentication](https://azure.microsoft.com/updates?id=562705)
VPN Gateway에서 인증 기반 VPN 연결 지원. X.509 인증서 체인 기반 신뢰성 강화 및 IKE 협상 내 보안성 향상.

### [Azure Virtual Network Manager rule impact analyzer](https://azure.microsoft.com/updates?id=562010)
시뮬레이션 기반 보안 규칙 영향 분석, 트래픽 흐름 예측 및 장애 방지, 설계/운영 자동화 지원.

### [Azure Virtual Network updates – default limits increased](https://azure.microsoft.com/updates?id=562695)
NSG 및 라우팅 테이블 한도가 대폭 상향. 대규모 네트워크/보안 정책 구현 및 엔터프라이즈 운영 최적화.

### [User Groups and IP address pools for P2S connections](https://azure.microsoft.com/updates?id=564460)
VPN Gateway에서 사용자 그룹별 IP 풀 할당 기능 추가, 그룹 기반 세분화 및 세분화 보안 정책 구현 가능.

---

## 3. 📊 데이터·스토리지·이동 & 관리

미션 크리티컬 데이터 관리와 서비스 통합, 대규모 마이그레이션, 다양한 개발 언어 SNS/SDK 지원 등이 대거 확대되었습니다.

### [Azure Blob Storage SDK for Rust 정식 지원](https://azure.microsoft.com/updates?id=562516)
Rust 환경에서 생산성 높은 안정적 Blob 스토리지 연동 SDK 출시. 인증, 자동 재시도, 분산 추적 등 최신 기능 제공.

### [Mock runs for Azure Storage Actions](https://azure.microsoft.com/updates?id=559494)
모의 실행을 통한 대규모 작업 검증. 실제 데이터 변화 없이 시뮬레이션 리포트로 정책 효과 및 파일 처리 건전성 체크 가능.

### [Azure Storage Mover Blob-to-Blob migration](https://azure.microsoft.com/updates?id=562753)
에이전트리스 Blob 간 직접 이관 지원. 대용량/병렬 데이터 마이그레이션 자동화, 작업 관리·진행 추적 기능 통합.

### [Azure NetApp Files cache volumes 정식 지원](https://azure.microsoft.com/updates?id=562259)
가장 빈번히 접근되는 데이터만 클라우드 내 캐시로 보유, WAN 대역폭/지연비용 절감 및 분산 파일 액세스 최적화.

### [Prefix-scoped access for User Delegation SAS](https://azure.microsoft.com/updates?id=561257)
Blob SAS 권한 부여 범위를 프리픽스(가상 디렉터리) 단위로 세분화, 유연한 보안 정책 및 다중 사용자 환경 지원.

---

## 4. 🛡️ AI, 데이터베이스, 앱/서비스 통합

AI 기반 서비스 연동, NoSQL 데이터플랫폼의 에이전트 활용, 서비스 메시징 보안, API 통합 기능 강화 등 엔터프라이즈 개발 환경 최적화 방향이 두드러집니다.

### [langchain-azure-cosmosdb Python 패키지 정식 지원](https://azure.microsoft.com/updates?id=562074)
LangChain/LangGraph와 Cosmos DB의 벡터(하이브리드) 검색, 캐시, 챗 히스토리 등 긴밀한 워크플로우 통합.

### [Confidential computing for Azure Service Bus Premium (Korea Central)](https://azure.microsoft.com/updates?id=561942)
하드웨어 기반 TEE 환경에서 메시지 데이터 보호. 암호화 가공 상태 데이터까지 보안 수요 부응, 기존 앱 변경 불필요.

### [Azure Event Grid releases – MQTT 기능 향상](https://azure.microsoft.com/updates?id=562240)
MQTT retain/공유 구독/HTTP 퍼블리시, IoT 실시간 애플리케이션을 위한 확장된 연결 및 백엔드 통합.

### [Application Insights Auto-instrumentation for AKS apps](https://azure.microsoft.com/updates?id=562049)
AKS 앱에 대한 소스코드 수정 없는 자동 계측, Java/Node.js 지원·분산 추적·트랜잭션 진단 강화.

### [Multiparty private offers in Microsoft Marketplace expands](https://azure.microsoft.com/updates?id=563016)
마켓플레이스 내 다자간 프라이빗 오퍼 30개국 확장. 파트너 협업 통한 신규 시장 진출 및 고객 신뢰 기반 클라우드·AI 도입 확대.

---

## 5. 🏗️ 스토리지·파일서비스·Elastic SAN·Azure Files

트랜잭션 파일 IO·데이터 분산 캐시·파일 교차 활용 및 인증 전략 등 기존 외부 스토리지 통합부터 최신 하이엔드 SAN, 데이터 복원 등 현장 요구에 부응한 업그레이드가 강화되었습니다.

### [Azure Elastic SAN support for AVS Gen2 Private Cloud](https://azure.microsoft.com/updates?id=560909)
ExpressRoute 없이 간편 연결 및 제한 없는 스루풋 제공, AVS 고성능 워크로드 최적.

### [Azure NetApp Files object REST API 정식 지원](https://azure.microsoft.com/updates?id=562254)
S3 호환 API 기반 Fabric/AI/다양한 Azure 서비스와 심리스한 연동 및 데이터 복제 없이 신규 분석 활용 확대.

### [Single Volume Snapshots on Azure Elastic SAN](https://azure.microsoft.com/updates?id=560899)
개별 SAN 볼륨별 증분 스냅샷. 복원·이관·백업 작업 용이성 향상 및 비용·운영 효율화.

### [Managed Identity Support 및 Entra-only identities with Azure Files](https://azure.microsoft.com/updates?id=562359)
Azure Files SMB 공유 접근 시 Entra ID/Managed Identity 기반 인증. 액세스 키 없는 멀티리전 보안, RBAC 및 규제 준수 강화.

### [Support for workloads with large files in Azure NetApp Files](https://azure.microsoft.com/updates?id=561722)
64TiB 단일 파일 볼륨 지원, AVS 대용량 워크로드 및 파일 기반 빅데이터 서비스 적합성 제고.

---

## 6. 🛠️ 개발·운영·거버넌스·비용관리

재해 복구 DR 지원 개선, 모의 실행/리스크 프리뷰, 비용 정책·SLA 관리 자동화, MarketPlace 자동구독, 운영/감사 기능이 동반 강화되었습니다.

### [Azure Site Recovery, Performance Plus Managed Disks 지원 (미리 보기)](https://azure.microsoft.com/updates?id=564644)
프리미엄 SSD 및 Performance Plus 디스크 실시간 복제·DR 시나리오 지원으로, 프라이머리/세컨더리 성능 오차 최소화.

### [Mock runs for Azure Storage Actions](https://azure.microsoft.com/updates?id=559494)
대규모 Blob 일괄 관리 작업 실행 전 정책의 사전체크 가능.

### [Multiparty Marketplace Offer 및 SaaS 자동 활성화](https://azure.microsoft.com/updates?id=561771)
마켓플레이스 SaaS 구독 즉시 시작·과금, 오퍼별 파트너 정책 자동화.

### [Network Watcher rule impact analyser](https://azure.microsoft.com/updates?id=562690)
네트워크/보안 변화에 대한 사전 영향 분석, 장애 예방과 컴플라이언스 보장.

### [Update: 99.99% uptime for Azure Service Bus Premium SLA](https://azure.microsoft.com/updates?id=561947)
AZ 지원 리전 내 프리미엄 네임스페이스 SLA 상향, 복잡한 메시징 인프라의 신뢰성 대폭 강화.

---

## 7. 💡 신규 서비스 및 사용 중단(지원 종료)

기존 VM 예약 인스턴스·구 API 지원 종료 공지, 구 TLS 연결의 단계적 중단 등 장기적 로드맵에 맞춘 기술 선택·마이그레이션 전략 수립 필요성을 강조했습니다.

### [TLS 1.0/1.1 in App Service, Functions, Logic Apps 지원 종료 (2027)](https://azure.microsoft.com/updates?id=557852)
2027년 5월 이후 TLS 1.0, 1.1 접속 불가. 보안 모범 사례 준수 위해 클라이언트/앱 사전 점검 권장.

### [Azure Document Intelligence v3.0 API 지원 종료 사전 공지](https://azure.microsoft.com/updates?id=561176)
2029년 3월 30일 이후 v3.0 버전 API 지원 종료. v4.0 등 최신 버전으로 조기 마이그레이션 필요.

### [Azure Reserved VMs Instances(일부 시리즈) 지원 종료](https://azure.microsoft.com/updates?id=560948)
2026년 7월 1일부터 Av2, Bv1, D, Dv2 등 신규/갱신 불가. 후속 VM 시리즈로 전환 유도.

### [Update: Egress/Data Transfer with Azure in UK](https://azure.microsoft.com/updates?id=561392)
영국 데이터 전송 시 적용 조건 변경, 비용 및 크레딧 청구 정책 안내.

### [Microsoft Foundry 내장 RBAC 역할 네이밍 개편 및 관리 강화](https://azure.microsoft.com/updates?id=562533)
역할 명칭 맞춤, 신규 워크플로 관리·권한 할당 시나리오 대응.

---

## 한국(Korea Central, Korea South) 지역 관련

### [Confidential computing for Azure Service Bus Premium (Korea Central)](https://azure.microsoft.com/updates?id=561942)
Azure Service Bus Premium에서 하드웨어 기반 신뢰 실행환경(TEE)을 통한 메시지 처리 지원 가능. 암호화된 데이터 가공·이동 중·저장 상태 전체가 보호되므로, 국내 규제가 요구하는 데이터 주권·보안 요구사항을 완벽히 충족함. 애플리케이션 코드 수정 없이 네임스페이스 단위로 설정할 수 있어, 금융·공공 등 보안 민감 업계에 적합.

---

## 총평 및 다음 달 전망

2026년 5월의 Azure 업데이트는 엔터프라이즈 및 퍼블릭 클라우드 고객 모두의 요구, 특히 대규모 확장성·보안·자동화·운영 편의성에 대한 트렌드를 반영한 실용 중심의 방향이 인상적이었습니다. 미리 보기 기능들을 통해 대용량 데이터관리, 네트워크 관리 자동화, 서비스 통합이 더욱 간편해졌으며, 컴파일러와 코드 변경 없는 모니터링·DR 등 개발과 운영 프로세스 효율도 크게 진전되었습니다.

지원 종료 관련 사전 공지(예약 VM, TLS, 문서 AI 등)가 늘어 감에 따라, 내년을 대비한 시스템 전환과 보안 정책 검토·연동 서비스 아키텍처 조정 작업의 우선 순위가 더욱 높아질 것으로 전망됩니다.

6월에는 Ignite 등 주요 연례 행사들과 맞물려, Azure AI, 보안 자동화, 하이브리드 멀티클라우드 연동, 클라우드 네이티브 개발툴 중심으로 더욱 혁신적인 서비스와 선제적 보안·운영 지원책이 발표될 것으로 기대됩니다. 앞으로도 Azure의 방향성은 클라우드 도입의 장벽을 낮추고, 데이터 기반 비즈니스의 지능화·효율화를 다양한 운영 환경에서 실현하는 데 중점을 둘 것이 분명해 보입니다.