# Azure 월간 업데이트 요약 - 2026년 09월

## 전반적인 트렌드 및 핵심 인사이트

2026년 9월 Azure 업데이트는 AI 및 observability, 네이티브 운영 자동화, 멀티클라우드∙하이브리드 환경 확장, 보안 강화, 개발자 경험 개선이 두드러진 한 달이었습니다. 가장 눈에 띄는 트렌드는 AI와 클라우드 네이티브 기술의 결합을 통한 지속적인 플랫폼 자동화, 그리고 컨테이너·데이터·네트워크·스토리지 각 영역에서 대규모 확장성 및 민첩한 서비스 적용이 강화된 점입니다.

Azure Copilot과 Microsoft Foundry(에이전트/네트워크/자동화)가 대거 정식 지원됨에 따라, 기업은 운영 모니터링·문제 해결·보안 정책을 인공지능 기반으로 효과적으로 관리할 수 있게 되었습니다. Azure SQL, PostgreSQL, MySQL 등 주요 데이터 플랫폼에는 AI, 벡터 인덱스, 자동 포맷팅 등 혁신적 기능이 추가되어 데이터 시나리오가 한층 더 현대화되고, Fabric 및 Agent 365 기반으로 데이터 거버넌스와 관리 단일화가 진전되었습니다.

네트워크·컴퓨팅·스토리지 영역에서는 VM 및 서비스 배포의 자동화(Automatic Zone Placement), 고성능 VM 시리즈 출시(Laosv5·Lasv5), NetApp Files의 쿨 액세스 및 대용량 볼륨 지원, 보안 인증(Entra Kerberos·User-bound SAS) 도입이 글로벌 클라우드 경쟁력을 높였습니다.

또한 Azure Arc·멀티클라우드 인터커넥트·연결형 SQL 인스턴스 등 하이브리드/멀티클라우드 기능이 다수 강화되어, 온프레미스와 Azure를 자연스럽게 연결하고 관리하는 사용자 경험이 개선되었습니다. 미리 보기 기능(preview)도 증가하여, 대기업뿐 아니라 마이크로서비스 개발 조직의 실험과 혁신 기회를 확대하고 있습니다. 서비스 지원 종료(retirement) 항목에서는 기존 IoT, HPC, 커뮤니케이션, 함수 컨테이너 등 구형 모델의 점진적 이전 계획이 안내되어, 기업의 장기적인 클라우드 전환 전략 수립을 촉진하고 있습니다.

다음 섹션에서는 주요 업데이트를 카테고리별로 깊이 있게 분석합니다.

---

## 🚀 서비스 출시 및 기능 업데이트

정식 지원이 이뤄진 서비스들은 운영 자동화, 데이터 관리, 보안, 컴퓨팅, 개발환경 등 다양한 영역에 걸쳐 있습니다.

### [Artifact Streaming on AKS](https://azure.microsoft.com/updates?id=570095)
AKS에서 Azure Container Registry를 활용한 Artifact Streaming으로 컨테이너 워크로드의 배포 속도를 대폭 향상시킵니다. 이미지 풀링 대기 없이 클러스터 확장 가능.

### [Azure Copilot Troubleshooting Agent](https://azure.microsoft.com/updates?id=570980)
운영 문제 발생 시 Copilot 기반으로 빠른 탐지~해결까지 자동화된 트러블슈팅 경험을 제공합니다.

### [Azure Ephemeral OS Disk with full caching for VM/VMSS](https://azure.microsoft.com/updates?id=570551)
에페멀 OS 디스크 풀 캐싱 지원으로 VM/VMSS의 I/O 성능 최대 10배 향상, 분산·AI·분석 등 집약적 워크로드에도 안정적 지원.

### [Azure Functions support for PowerShell 7.6](https://azure.microsoft.com/updates?id=572219)
최신 PowerShell 7.6을 Azure Functions에서 지원해 로컬 개발~클라우드 배포까지 통합된 스크립트 환경을 제공.

### [Azure Database for PostgreSQL Flexible Server cross-tenant CMK](https://azure.microsoft.com/updates?id=571783)
엔트라 테넌트 간 고객 관리 키로 데이터 암호화 가능, SaaS 및 ISV가 보안·컴플라이언스 요구를 독립적으로 충족 가능.

### [Azure Arc-enabled SQL Server in 새로운 지역(이탈리아, 독일)](https://azure.microsoft.com/updates?id=570763)
SQL Server의 Azure Arc 연결을 주요 지역(Italy North, Germany West Central)에 확대하여 하이브리드 관리의 범위 확장.

### [Azure Developer CLI (azd) Extension Framework 정식 지원](https://azure.microsoft.com/updates?id=570881)
개발자가 CLI 워크플로우를 확장·자동화하는 프레임워크로, 조직별 맞춤형 개발·배포 환경 구축 가능.

### [Azure Virtual Network Manager IPAM/High-scale mesh 정식 지원](https://azure.microsoft.com/updates?id=570557)
IP 주소 배치 및 하이 스케일 메쉬 기능이 여러 지역에서 사용 가능. 최대 3,000개 가상 네트워크 연결로 글로벌 네트워크 관리 효율화.

### [Storage optimized Lasv5 and Laosv5 Azure VM series](https://azure.microsoft.com/updates?id=572630)
최신 AMD EPYC™ 기반 대용량 스토리지 최적화 VM(Lasv5, Laosv5)의 출시로 HPC, 대규모 데이터 분석, AI 워크로드에 최적화된 성능 제공.

### [Instant Access for VM Restore Points](https://azure.microsoft.com/updates?id=572573)
VM 복구 시 즉시 스냅샷 접근·복원이 가능해 RTO(복구 시간 목표) 극대화, 자동화·운영 효율성 제고.

---

## 🔍 미리 보기(Preview) 기능

대규모 플랫폼 확장, 멀티클라우드 연결, AI/데이터 자동화 관련 실험적 기능들이 대거 발표되었습니다.

### [Agentless migration of on-premises SMB file shares to Azure Files](https://azure.microsoft.com/updates?id=570910)
온프레미스 파일 이관 시 에이전트 없이 Azure Storage Mover로 빠르게 데이터 이동 가능.

### [Automatic Zone Placement for Virtual Machine Scale Sets](https://azure.microsoft.com/updates?id=571075)
VM Scale Set 배포 시 Azure가 자동으로 최적화된 가용성 존을 선정, 운영의 복잡성 해소.

### [Azure Multicloud Interconnect](https://azure.microsoft.com/updates?id=570364)
Azure와 AWS 등 다양한 클라우드 간 프라이빗 연결을 자동 관리, 멀티클라우드 환경에 빅데이터·AI·서비스를 통합 가능.

### [Azure Red Hat OpenShift with Hosted Control Planes](https://azure.microsoft.com/updates?id=571621)
OpenShift 컨트롤 플레인을 완전 매니지드 방식으로 운영, 개발·테스트 환경의 신속한 확장/축소 지원.

### [Azure SQL Hyperscale Serverless auto-pause/auto-resume](https://azure.microsoft.com/updates?id=571857)
서버리스 DB에서 자동 일시정지/재시작 지원, 불필요한 비용 절감과 데이터 처리 유연성을 확보.

### [Foundry Routines/Network Egress Controls(미리 보기)](https://azure.microsoft.com/updates?id=563536)
Foundry 에이전트의 일정/이벤트 기반 트리거링과 네트워크 연결 허용 조건 정책으로 보안과 자동화 강화.

---

## 🛡️ 보안, 컴플라이언스, 관리

각종 보안 인증, 관리 자동화, 데이터 보호 기능이 개선되어 엔터프라이즈 IT 운영 위험을 최소화합니다.

### [Azure Firewall auto-learn SNAT routes](https://azure.microsoft.com/updates?id=570474)
Firewall이 자동으로 SNAT 경로 학습‧적용해 원본 IP를 보존, SNAT 관리 간소화.

### [User-bound user delegation SAS for Azure Storage](https://azure.microsoft.com/updates?id=569241)
엔트라 ID 기반 사용자 구속 SAS로 보다 안전한 블록/파일/테이블/큐 인증 제공.

### [TLS/SSL certificate 및 end-to-end TLS encryption for Azure Functions Flex Consumption](https://azure.microsoft.com/updates?id=570940)
함수 앱별 인증서 및 전체 트래픽 TLS 암호화로 웹·IoT·컨테이너 환경의 안전성 극대화.

### [Microsoft Entra Kerberos authentication for Azure NetApp Files(Preview)](https://azure.microsoft.com/updates?id=573041)
Entra ID 기반 Kerberos 인증으로 하이브리드/클라우드 SMB 접근 시 기존 AD 의존성 제거.

### [Azure Payments HSM v2(Preview)](https://azure.microsoft.com/updates?id=570509)
PCI DSS, FIPS 등 국제 기준 준수한 단일 테넌트 결제 HSM 서비스 도입, 결제 자산∙키 관리 강화.

---

## ☁️ 하이브리드, 멀티클라우드, 지역 확장

온프레미스와 클라우드, 멀티클라우드, 글로벌 확장에 최적화된 다양한 지원이 새로이 이루어졌습니다.

### [Azure Arc-enabled SQL Server 신규 지원 지역(이탈리아, 독일)](https://azure.microsoft.com/updates?id=570763)
SQL Server를 Azure Arc에 연결하는 하이브리드 관리 지역 확대.

### [Playwright Workspaces in Australia East, Japan East, Switzerland North](https://azure.microsoft.com/updates?id=570919)
클라우드 기반 테스트 환경의 글로벌 확장으로 개발·QA 워크플로우 활성화.

### [Luxembourg - Azure Extended Zones](https://azure.microsoft.com/updates?id=572968)
저지연 및 데이터 지역성을 강조한 Azure Extended Zone이 룩셈부르크에 출시.

### [Cloud-to-cloud 연결(Azure Multicloud Interconnect) 미리 보기](https://azure.microsoft.com/updates?id=570364)
AWS와 Azure, 향후 더 많은 클라우드 간 자동화된 고성능 프라이빗 연결 지원.

### [Performance monitoring for Azure Arc-enabled SQL Server/Managed Instance(Preview)](https://azure.microsoft.com/updates?id=571904)
Azure Arc를 통한 SQL Server 모니터링 자동화가 Fabric 연동 대시보드로 경험 통일.

---

## ⚡️ 개발자 및 SDK/도구 혁신

개발자 생산성, 워크플로우 표준화, AI 기반 개발 환경 등에 집중된 업데이트.

### [Azure Developer CLI (azd) Extension Framework 정식 지원](https://azure.microsoft.com/updates?id=570881)
CLI 기능 확장 및 맞춤형 개발 자동화, 플러그인 Ecosystem 성장 촉발.

### [SQL Formatter for Visual Studio Code](https://azure.microsoft.com/updates?id=571872)
VS Code에서 직접 SQL 코드 포맷팅 및 검증, 쿼리 표준화·가독성 제고.

### [Azure SQL Dev Hub(Preview)](https://azure.microsoft.com/updates?id=572998)
Azure SQL 개발·운영·AI 적용에 특화된 허브 기능으로 개발 초입~배포까지 원스톱 지원.

### [Introducing a Guided Copilot Experience for Building Azure Apps in VS Code(Preview)](https://azure.microsoft.com/updates?id=572214)
VS Code에서 GitHub Copilot을 통한 체계적인 앱 구축 워크플로우 제공.

### [SQL Migration Agent Skills for assessment, migration, and validation](https://azure.microsoft.com/updates?id=571899)
AI 기반 SQL 서버 진단, 목표 선정, 자동 마이그레이션, 사후 검증 스킬로 클라우드 데이터 이전을 자동화.

---

## 🧠 Microsoft Foundry & Microsoft Fabric 카테고리

AI·데이터 기반 자동화 에이전트, Fabric 데이터 허브, 기타 AI+클라우드 결합 플랫폼 등장.

### [Enable/disable controls for Microsoft Foundry agents in Agent 365](https://azure.microsoft.com/updates?id=571826)
Foundry 에이전트의 조직 내 사용 제어를 Admin Center에서 관리, 거버넌스 및 보안 강화.

### [Publishing Foundry agents to Microsoft 365 Copilot and Teams](https://azure.microsoft.com/updates?id=571816)
Foundry 에이전트를 M365 Copilot, Teams에 직접 배포·운영, Entra·Agent 365 통합 관리 가능.

### [Foundry Routines 및 네트워크 이그레스 정책(Preview)](https://azure.microsoft.com/updates?id=563536)
스케줄, 이벤트 기반 에이전트 트리거링, 네트워크 egress 조건 세분화로 자동화 및 보안 강화.

### [Database Hub in Microsoft Fabric(Preview)](https://azure.microsoft.com/updates?id=571846)
SQL/포스트그레/코스모스DB/파브릭 DB를 AI 기반 통합 허브에서 관리, 데이터 현대화 추진.

### [Performance monitoring 연동(Microsoft Fabric)](https://azure.microsoft.com/updates?id=571904)
Fabric 데이터 허브와 연동된 DB 모니터링으로 엔터프라이즈 데이터 거버넌스 혁신.

---

## 🔥 지원 종료(retirement) 및 마이그레이션 가이드

클라우드 플랫폼의 장기적 전략과 서비스 현대화 흐름을 반영하는 지원 종료 소식.

### [Azure Communication Services(ACS) standalone services 2028년 9월 30일 지원 종료](https://azure.microsoft.com/updates?id=557117)
이메일, SMS, 채팅, 룸 등 독립 ACS 기능이 대거 종료 예정. Microsoft Teams 연동만 가능.

### [Azure Arc-enabled System Center Virtual Machine Manager 2029년 9월 30일 지원 종료](https://azure.microsoft.com/updates?id=570283)
SCVMM 통합 기능 중단 예정, Azure Arc-enabled Servers 등 대체 경로 제안.

### [Azure IoT Central 2029년 9월 20일 지원 종료](https://azure.microsoft.com/updates?id=569914)
IoT Central 대신 IoT Hub, DPS, Microsoft Fabric 기반으로 데이터·디바이스 관리 전환 권장.

### [Azure Functions v1 hosting model on Azure Container Apps 2027년 9월 29일 지원 종료](https://azure.microsoft.com/updates?id=570800)
기존 v1 모델 앱은 v2 모델로 마이그레이션 필요, 코드 변경 없이 표준화된 경로 제공.

### [Support for PowerShell 7.4, Node.js 22, .NET 8/9 등 순차 지원 종료](https://azure.microsoft.com/updates?id=572770)
각 언어별 최신 버전(7.6/24/10)으로 업그레이드 필수. 보안 패치, 기능 개선 반영 위해 신속 전환 권장.

---

## 📝 총평 및 다음 달 전망

9월은 Azure가 AI 중심의 자동화, 데이터 관리 혁신, 멀티클라우드/하이브리드 확장, 엔터프라이즈 보안 자동화, 개발자 친화 기능 강화 등 전방위적으로 플랫폼을 진화시켰습니다. 특히 Copilot, Foundry, Fabric 허브 등 신기술은 실질적인 거버넌스·운영 효율화에서 미래형 서비스로의 전환을 주도하고 있습니다. 기존 IoT, HPC, 커뮤니케이션, 함수 컨테이너 모델의 지원 종료 소식은 조직의 클라우드 현대화 전략 수립을 시급히 요구합니다.

오는 10월은 Fabric의 실사용 사례 확장, Foundry 에이전트 생태계 성장, 멀티클라우드 지원·보안 인증 강화, 글로벌 리전/서비스 확대가 기대됩니다. 마이그레이션 및 신규 워크플로우 적용 가이드도 점점 늘어나, 점진적 혁신과 안정적 클라우드 전환을 아우르는 업데이트가 지속될 것으로 전망됩니다.