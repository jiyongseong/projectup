# Azure 월간 업데이트 요약 - 2026년 09월

## 전반적인 트렌드 및 핵심 인사이트

2026년 9월의 Azure 업데이트는 새로운 서비스의 정식 지원과 기존 서비스의 기능 확장, 그리고 미리 보기 단계의 혁신적 기능과 플랫폼의 도입이 두드러졌습니다. 특히 Microsoft Foundry와 Microsoft Fabric 같은 AI 및 데이터 플랫폼 관련 생태계의 성장이 두드러졌으며, 컨테이너 기반 인프라와 DevOps 자동화, 그리고 데이터베이스의 하이브리드/멀티클라우드 지원 강화가 주요 방향으로 나타났습니다. AKS와 Azure Functions, SQL 및 PostgreSQL 인스턴스 등 주요 클라우드 컴포넌트에서는 보안, 성능, 자동화, 확장성 측면에서 실질적 개선을 이뤘습니다. Azure Copilot 및 보안 관리 툴, 자동화 디버깅 기능의 정식 지원은 운영 효율성과 서비스 안정성을 높였으며, 네트워크와 스토리지에서 대규모 환경을 위한 IP 관리, 고성능 VM, 대용량 볼륨 등 엔터프라이즈급 요구를 충족시키기 위한 서비스가 강화되었습니다.

데이터베이스 영역에서는 AI 활용을 위한 벡터 검색 및 인덱스, SQL 개발 자동화, 대규모 분산 처리와 포스트그레스 최신 버전 지원 등 기존 관계형·비관계형 데이터 환경의 현대화와 통합이 가속화되고 있습니다. 모니터링과 분석 관련 기능도 Fabric 데이터 허브와 Grafa 기반 대시보드 도입 등으로 더욱 통합되고 직관적으로 업데이트되었습니다. Azure가 글로벌 리전 확장과 함께 오퍼링을 다양화하여, 지역 특화 서비스와 데이터 레지던시, 지역별 가용성 향상에 적극 나서는 모습도 관찰할 수 있습니다.

한편 미리 보기 서비스들은 하이브리드 클라우드 연계(Multicloud Interconnect), Kubernetes Flex 노드 같은 클라우드/엣지 통합, 자동화된 데이터 마이그레이션과 신뢰성 강화를 위한 기능, 고성능 컴퓨팅(HPC) VM 등 미래 지향적 기술의 도입을 예고합니다. 이러한 변화는 Azure의 클라우드 기반 AI, 데이터 분석, 운영 효율, 보안, 자동화 영역에서 성숙도와 경쟁력을 크게 끌어올리고 있으며, 기존 온프레미스와의 통합, 엔터프라이즈 요구에 맞춘 확장성이 두드러진다는 점에서 기업과 개발자, 관리자의 기대를 더욱 수렴하는 방향으로 진화하고 있습니다.

7개의 주요 카테고리별로 정리된 세부 업데이트를 아래에서 확인할 수 있습니다.

---

## 🛠️ 컴퓨트 & 컨테이너

본 카테고리는 AKS, Virtual Machines, Functions, VM 관리 도구 등 클라우드 인프라와 컨테이너 플랫폼 중심의 업데이트를 다룹니다. 주요 트렌드는 컨테이너 기반 워크로드의 확장성, VM 성능 향상, 보안 강화, 그리고 서비스 릴타임 운영의 자동화와 효율성입니다.

### [Artifact Streaming on AKS](https://azure.microsoft.com/updates?id=570095)
Azure Kubernetes Service에서 컨테이너 이미지를 완전히 다운로드하지 않아도 워크로드를 스케일링할 수 있는 'Artifact Streaming' 기능이 정식 지원되며, 컨테이너 배포 속도가 크게 향상됩니다.

### [Confidential VMs for Azure Linux](https://azure.microsoft.com/updates?id=570100)
AKS 내 Azure Linux용 컨피덴셜 VM 기능이 정식 지원되어 민감한 컨테이너 워크로드를 별도 코드 리팩토링 없이 안전하게 마이그레이션 할 수 있습니다.

### [Windows Server 2025 on AKS](https://azure.microsoft.com/updates?id=570090)
AKS에서 Windows Server 2025에 대한 정식 지원이 출시되며, 최신 보안과 성능 개선, FIPS 기본 활성화 등 안정화된 운영 환경 제공이 가능합니다.

### [Azure Ephemeral OS Disk with full caching for VM/VMSS](https://azure.microsoft.com/updates?id=570551)
신규 VM 및 VMSS에 대해 완전 캐싱 기반 Ephemeral OS Disk가 정식 지원되어 최대 10배의 I/O 성능과 스토리지 중단 시 복원력을 제공하며, AI, 실시간 분석 등 고성능 워크로드에 적합합니다.

### [Azure Functions support for PowerShell 7.6](https://azure.microsoft.com/updates?id=572219)
Azure Functions가 PowerShell 7.6을 정식 지원하여 최신 스크립트 언어 활용과 보안 업데이트, 확장된 운영 환경을 제공합니다.

---

## 📊 데이터베이스 & 분산 데이터

이 영역은 Azure SQL, PostgreSQL, MySQL, 데이터 마이그레이션/운영 자동화 기능을 집중적으로 다루며, AI 활용과 개발 효율 증대, 운영 자동화가 핵심입니다.

### [Azure SQL Database Hyperscale Premium 확장](https://azure.microsoft.com/updates?id=571643)
Azure SQL Database Hyperscale Premium 시리즈에서 160-vCore, 192-vCore 신규 옵션이 추가되어 대규모 워크로드 처리능력이 50% 향상됩니다.

### [Vector search and vector indexes in Azure SQL](https://azure.microsoft.com/updates?id=571800)
Azure SQL Database에서 벡터 검색 및 벡터 인덱스가 정식 지원되어, AI 기반 의미 검색, RAG, 추천 시스템, 이미지 검색 등 최신 인공지능 활용이 가능해졌습니다.

### [Azure Database for PostgreSQL Flexible Server의 cross-tenant CMK 지원](https://azure.microsoft.com/updates?id=571783)
SaaS 및 ISV 환경에서 데이터 암호화를 외부 테넌트에 저장된 CMK를 통해 가능하게 하여 보안 및 컴플라이언스 요구를 강화합니다.

### [PG18 지원 for Azure Database for PostgreSQL elastic clusters](https://azure.microsoft.com/updates?id=571047)
PostgreSQL 18이 elastic clusters에서 지원되어 최신 기능과 신뢰성, 분산 처리 성능을 클라우드에서 활용할 수 있습니다.

### [SQL Formatter](https://azure.microsoft.com/updates?id=571872)
Visual Studio Code에 SQL Formatter가 도입되어 SQL 개발 효율성과 코드 표준화가 크게 개선되었습니다.

---

## 🌐 네트워킹 & 보안

네트워크 관리, Firewall, Virtual Network, 보안 기능 등 인프라 및 운영 보안 강화 관련 업데이트가 중심입니다.

### [Azure Firewall auto-learn SNAT routes](https://azure.microsoft.com/updates?id=570474)
Azure Firewall이 자동으로 SNAT 경로를 학습, No-SNAT 범위 적용으로 원본 IP 보존 및 SNAT 관리 간소화가 정식 지원됩니다.

### [Azure Virtual Network Manager IPAM 기능 추가](https://azure.microsoft.com/updates?id=570557)
IP 주소 중앙 관리와 할당, 충돌 방지, 글로벌 주소 공간 관리 등이 정식 지원되어 대규모 네트워크 관리 효율이 향상되었습니다.

### [High-scale mesh in Azure Virtual Network Manager](https://azure.microsoft.com/updates?id=571572)
최대 3000개 VNET을 단일 메시로 연결할 수 있으며, 피어링 없이 대규모 네트워크 그룹 관리가 쉽고 직관적으로 진행됩니다.

### [Azure Front Door profile 및 경로 WAF 정책 미리 보기](https://azure.microsoft.com/updates?id=569804)
Azure Front Door에서 프리뷰 단계로 다양한 범위에서 WAF 정책을 적용할 수 있게 되어 세분화된 보안 구성 및 관리가 강화되었습니다.

### [HTTP/3 over QUIC 지원 in Azure Application Gateway](https://azure.microsoft.com/updates?id=571123)
HTTP/3 및 QUIC 프로토콜 지원이 미리 보기로 제공돼, 웹 및 API 워크로드의 연결 성능과 안정성이 개선되었습니다.

---

## 💾 스토리지 & 파일 서비스

Azure NetApp Files, Blob Storage, Disk Storage 등 클라우드 스토리지 관련 주요 업데이트와 성능·보안 강화 기능이 포함됩니다.

### [Storage optimized Lasv5 및 Laosv5 Azure VM 시리즈](https://azure.microsoft.com/updates?id=572630)
Lasv5/Laosv5 VM 시리즈가 정식 지원되어 고성능 NVMe SSD, 대용량 스토리지, 향상된 CPU 성능 등 대규모 워크로드에 최적화된 인프라를 제공합니다.

### [Support for large volume breakthrough mode](https://azure.microsoft.com/updates?id=573027)
Azure NetApp Files에서 2PiB 대용량 및 초고속 성능을 제공하는 'breakthrough mode' 지원이 정식으로 제공, HPC 및 대규모 EDA 워크로드에 적합합니다.

### [Public Preview: Microsoft Entra Kerberos 인증 in Azure NetApp Files](https://azure.microsoft.com/updates?id=573041)
엔트라 ID 기반 Kerberos 인증 지원이 미리 보기로 제공돼, 하이브리드 및 클라우드 환경의 사용자 인증이 간소화되고 보안성이 강화됩니다.

### [Storage with cool access enhancement](https://azure.microsoft.com/updates?id=573032)
Azure NetApp Files에 쿨 액세스 QoS가 개선되어 스토리지 비용·성능을 자동으로 최적화하며 혼합 워크로드에 대응합니다.

### [User-bound user delegation SAS for Azure Storage](https://azure.microsoft.com/updates?id=569241)
Entra ID와 연계된 사용자 바운드 SAS 지원이 정식화되어 저장소 접근 제어와 인증, 규정 준수가 더욱 강화되었습니다.

---

## 🧑‍💻 개발자 도구 & DevOps

Azure CLI, 테스트 자동화, 모니터링, 개발자 경험 개선 등 클라우드 및 DevOps 중심 툴 업데이트가 포함됩니다.

### [Azure Developer CLI (azd) Extension Framework](https://azure.microsoft.com/updates?id=570881)
AzD 익스텐션 프레임워크의 정식 지원으로, 맞춤형 개발 자동화 툴과 워크플로우 구축이 가능하며, 개발자 환경 및 조직별 프로세스 통합이 촉진됩니다.

### [Playwright Workspaces에 추가 리전 지원](https://azure.microsoft.com/updates?id=570919)
스위스 북부, 일본 동부, 호주 동부에서 Playwright Workspaces 정식 지원으로 E2E 테스트의 글로벌 확장성이 강화되었습니다.

### [Azure Copilot Troubleshooting Agent](https://azure.microsoft.com/updates?id=570980)
AI 기반 운영 동반자인 Copilot Troubleshooting Agent가 정식 출시돼, 운영 이슈 탐지 및 해결이 자동화되고 운영 효율성이 극대화됩니다.

### [Azure Copilot Observability Agent 지원 확장](https://azure.microsoft.com/updates?id=570250)
Log Analytics의 Basic 및 Auxiliary Table Plan 지원으로, Kubernetes 등 고부하 텔레메트리 관리비용 절감 및 효율적 모니터링이 가능해졌습니다.

### [SQL Migration Agent Skills for assessment, migration, and validation](https://azure.microsoft.com/updates?id=571899)
SQL 마이그레이션 단계별 AI 기반 자동화 스킬이 정식 지원되어, 데이터베이스 마이그레이션의 평가/이동/검증 과정이 더욱 간편해집니다.

---

## 🤖 Microsoft Foundry & AI Platform

본 카테고리는 Microsoft Foundry, Fabric 등 Azure 기반 AI 및 데이터 플랫폼에서의 최신 기능, 관리 자동화, 보안 강화 등 혁신적 업데이트를 상세히 다룹니다.

### [Enable/disable controls for Microsoft Foundry agents in Agent 365](https://azure.microsoft.com/updates?id=571826)
Foundry 에이전트의 Agent 365 관리센터에서 사용 가능 여부를 조정할 수 있게 되어 컴플라이언스 및 보안 요구에 맞춘 중앙화 관리를 실현했습니다.

### [Publishing Microsoft Foundry agents to Microsoft 365 Copilot and Teams](https://azure.microsoft.com/updates?id=571816)
Foundry 에이전트를 Microsoft 365 Copilot 및 Teams로 직접 게시 가능해 사용성과 거버넌스, 조직 중앙 관리가 더욱 강화되었습니다.

### [Foundry Routines in Foundry Agent Service](https://azure.microsoft.com/updates?id=563536)
공개 미리 보기로 Foundry Agent Service에 스케줄 기반 루틴 기능이 추가되어, 자동 트리거 및 실행 모니터링이 별도 인프라 없이 가능해집니다.

### [Network egress controls for hosted agents in Microsoft Foundry](https://azure.microsoft.com/updates?id=571821)
에이전트의 네트워크 egress 제어 및 감사 모드가 미리 보기로 도입되어, AI 기반 서비스의 보안성과 거버넌스가 강화되었습니다.

### [Foundry routines 및 agent 자동화 기능 확장](https://azure.microsoft.com/updates?id=563536)
고객이 스케줄·이벤트 기반 트리거를 통해 Foundry agent 자동화 실행 및 관리를 직접 수행할 수 있습니다.

---

## 🔔 서비스 지원 종료 & 컴플라이언스

지원 종료(retirement), 사용 중단(deprecation), 데이터센터 확장 등 서비스 라이프사이클에 영향을 미치는 주요 변경 사항입니다.

### [Azure Arc-enabled SCVMM 지원 종료 안내](https://azure.microsoft.com/updates?id=570283)
Azure Arc-enabled System Center Virtual Machine Manager가 2029년 9월 지원 종료, 대체 솔루션으로의 마이그레이션 권장.

### [Azure Communication Services 단독 서비스 지원 종료](https://azure.microsoft.com/updates?id=557117)
ACS의 단독 서비스(Email, SMS, WhatsApp 등)가 2028년 9월 지원 종료 예정, Teams와 연동 외 서비스 이용 제한.

### [Azure IoT Central 지원 종료 예고](https://azure.microsoft.com/updates?id=569914)
IoT Central이 2029년 9월 지원 종료 최종 확정, IoT Hub/DPS, Fabric 기반 전환 권장.

### [Azure Functions v1 on Azure Container Apps 지원 종료](https://azure.microsoft.com/updates?id=570800)
Azure Container Apps 상의 Functions v1 호스팅 모델이 2027년 9월 29일 지원 종료, v2로 마이그레이션 안내.

### [Support for .NET 8/9, Node.js 22, PowerShell 7.4 ends](https://azure.microsoft.com/updates?id=572838)
.NET 8, .NET 9, Node.js 22, PowerShell 7.4 각 지원 종료 일정 안내 및 상위 버전 업그레이드 권장.

---

## 📍 글로벌 리전 & 서비스 확장

Azure의 지역별 신규 서비스 및 확장, Extended Zones 지원, 조직별 리전 오퍼링 강화 내용을 다룹니다.

### [Azure Arc-enabled SQL Server Available in Italy North](https://azure.microsoft.com/updates?id=570763)
Azure Arc-enabled SQL Server가 Italy North 리전에 정식 지원되어 현지 데이터 주권 및 거버넌스가 강화되었습니다.

### [Azure Arc-enabled SQL Server in Germany West Central](https://azure.microsoft.com/updates?id=570696)
Germany West Central 리전에서도 Azure Arc-enabled SQL Server 정식 지원으로, 유럽 지역 데이터베이스 현대화가 확대됩니다.

### [Luxembourg - Azure Extended Zones](https://azure.microsoft.com/updates?id=572968)
Luxembourg에서 Extended Zone이 정식 지원되며, 메트로/특정 구역에서 저지연 및 데이터 레지던시 서비스가 가능해졌습니다.

### [Azure Monitor Auxiliary Logs Plan in Azure Government/China](https://azure.microsoft.com/updates?id=569899)
미국 정부(Azure Gov), 중국리전에서 Azure Monitor Auxiliary Logs Plan의 정식 지원으로 규제 준수 및 고비용 로그를 효과적으로 관리하게 됩니다.

### [Azure Virtual Network Manager IPAM in 추가 Azure 리전](https://azure.microsoft.com/updates?id=570557)
IPAM 서비스가 미국 정부 및 중국 내 추가 리전에 지원되어 글로벌 멀티클라우드 네트워크 관리가 한층 확장되었습니다.

---

## 총평 및 다음 달 전망

9월의 Azure 업데이트는 AI, 데이터 플랫폼, 네트워크/스토리지의 엔터프라이즈 스케일 확장과 클라우드 운영 자동화, 보안 정책 강화가 두드러졌습니다. DevOps 및 개발자 효율화, 데이터베이스의 AI 활용, 글로벌 리전 확장 등 고객 중심 서비스 발전이 강조되고 있으며, 미리 보기 기능 도입을 통해 강력한 하이브리드/멀티클라우드, 엣지컴퓨팅 연계 등 미래지향적 기술 방향을 선도하고 있습니다. 다음 달에는 Fabric 기반 데이터 분석 플랫폼 통합의 가속화, Azure AI 서비스의 관리·보안 고도화, 하이브리드 플랫폼의 유연화와 운영 자동화, 신규 리전 확대 및 지역 맞춤형 인프라 강화가 더욱 주목받을 것으로 전망됩니다. Azure 생태계가 데이터, AI, 운영 효율, 글로벌 컴플라이언스 등 다각적 경쟁력을 지속적으로 강화하고 있어 기업 및 개발자, 운영 현장 모두에서 혁신의 흐름이 가속화될 것입니다.