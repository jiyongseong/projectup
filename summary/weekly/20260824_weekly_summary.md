# Azure 주간 업데이트 요약 - 2026년 08월 24일

## 🚀 출시 및 신규 기능

지난주 Azure에서는 데이터 분석과 서비스 배포, 네트워크 관리 등 전반에 걸친 신기능이 정식 지원되었습니다. Azure Databricks Lakebase가 미국 북중부, 프랑스 중앙, 독일 서부 중앙, 동아시아 등 4개 지역에서 정식 지원되어 기업 데이터 워크로드의 지역적 다양성이 크게 확장되었습니다. Azure SQL Database의 MSSQL 확장 내 프로비저닝 기능이 정식 지원되어, 에디터에서 직접 배포 및 연결이 가능하며 ARM, Bicep, Terraform 템플릿 등 자동화된 배포 옵션이 제공됩니다. Azure Site Recovery에서는 BYON NIC 기능이 도입되어 재해복구 환경에서 네트워크 설정과 IP 예약을 유연하게 관리할 수 있습니다. 또한 Azure App Service에서도 Managed Instance가 정식 지원되어, 기존 온프레미스 및 VM 기반 .NET 애플리케이션을 코드 변경 없이 PaaS 환경으로 전환할 수 있게 되었습니다. Dragon Copilot Physician Apps 역시 Microsoft Marketplace를 통해 업무 자동화 및 임상 데이터 활용성 확대가 가능해졌습니다.

### [Azure Databricks Lakebase, 4개 지역 정식 지원](https://azure.microsoft.com/updates?id=569684)
Lakebase가 새로운 4개 Azure 지역(미국 북중부, 프랑스 중앙, 독일 서부 중앙, 동아시아)에서 정식 지원되어 글로벌 데이터 분석 확장성이 강화됩니다.

### [Azure SQL Database MSSQL 확장 내 프로비저닝 정식 지원](https://azure.microsoft.com/updates?id=569160)
에디터 내에서 Azure SQL Database를 즉시 생성·연결하고, ARM/Bicep/Terraform 템플릿을 통한 반복 배포가 가능해졌습니다.

### [Azure Site Recovery에서 BYON NIC 기능 출시](https://azure.microsoft.com/updates?id=569515)
재해복구 시 기존 NIC를 활용해 네트워크 구성과 IP 예약을 유지하며 안정적이고 통제된 복구 운영이 지원됩니다.


## 💡 서비스 관리 및 운영 혁신

운영 관리 영역에서는 Azure Copilot이 업무 목적별 에이전트 직접 접근 기능을 선보였으며, Troubleshooting, Deployment, Optimization, Resiliency 등 주요 Copilot 에이전트를 채팅 환경에서 바로 호출할 수 있게 되었습니다. Azure Virtual Machines에서는 vCore 커스터마이징이 정식 지원되어 SMT/HT 비활성화, 컨스트레인드 코어 구성 등 고성능 워크로드 맞춤 운영과 소프트웨어 라이선스 비용 최적화가 가능해졌습니다. ExpressRoute 및 VPN Gateway에 게이트웨이 요약 Prefix 광고 기능이 도입되어, 대규모 네트워크 환경에서도 라우트 수 제한 관리가 유연하게 이루어집니다.

### [Azure Copilot, 에이전트 직접 접근 기능 발표](https://azure.microsoft.com/updates?id=569685)
Azure Copilot 사용자는 Troubleshooting, Deployment, Optimization, Resiliency 에이전트를 채팅에서 즉시 호출할 수 있습니다.

### [Azure Virtual Machines vCore 커스터마이징 정식 지원](https://azure.microsoft.com/updates?id=569051)
SMT/HT 비활성화, 컨스트레인드 코어 기능으로 적정 vCPU 구성 및 고성능 워크로드 맞춤 운영이 가능해졌습니다.

### [라우트 광고용 Gateway Prefix 요약 기능 정식 지원](https://azure.microsoft.com/updates?id=569743)
IPv4, IPv6 모두 ExpressRoute와 VPN Gateway에서 요약 Prefix 광고 지원으로 대규모 네트워크 라우트 관리가 효율적으로 개선됩니다.


## 🧪 미리 보기(Preview) 기능 및 실험적 업데이트

본격적 서비스 반영 전 단계 기능이 다양하게 공개되었습니다. Azure Linux가 WSL 환경으로 확장되어 개발, 테스트, 운영 일관성이 Microsoft 기반 리눅스 환경 내에서 보장됩니다. Azure Firewall에서는 IPv6 듀얼스택 미리 보기 기능이 지원되어 현대 네트워크 환경에 맞는 보안 정책 적용이 가능합니다. Azure SQL Managed Instance Next-gen General Purpose는 가용성 영역 자동 분산 Zone Redundancy 기능이 미리 보기로 도입되어 장애 대응력과 비즈니스 연속성이 극대화됩니다.

### [Azure Linux on WSL 공개 미리 보기](https://azure.microsoft.com/updates?id=569376)
Azure Linux를 WSL에서 사용하여 개발·운영 환경의 일관성을 확보할 수 있습니다.

### [Azure Firewall, IPv6 듀얼스택 미리 보기 지원](https://azure.microsoft.com/updates?id=569520)
IPv6 네이티브 지원 및 DNS Proxy가 가능해진 Azure Firewall로 클라우드 및 하이브리드 네트워크의 보안이 미래 대응형으로 강화됩니다.

### [Azure SQL Managed Instance Next-gen General Purpose, Zone Redundancy 미리 보기](https://azure.microsoft.com/updates?id=568344)
데이터와 컴퓨트가 가용성 영역에 자동 분산되어 장애 대응력이 향상돼 미션 크리티컬 워크로드의 고가용성 운영이 용이해집니다.


## 📦 인프라 및 앱 서비스 현대화

애플리케이션 현대화와 기업 IT 의존성 해소를 위한 신규 기능이 지속적으로 제공되었습니다. Azure App Service의 Managed Instance는 VM 혹은 온프레미스에서 남아있는 복잡한 .NET Framework 워크로드를 코드 변경 없이 PaaS 환경으로 옮길 수 있어 기업의 현대화 전환이 가속화됩니다. Dragon Copilot AI 워크플로우 앱·에이전트가 Marketplace에 출시되어 의료분야 업무 자동화 및 데이터 활용이 한층 강화되었습니다. Azure SQL의 8월 중순 업데이트에서는 키보드 단축키 커스터마이징 등 생산성 중심 기능이 추가되어 데이터 업무 효율성이 높아집니다.

### [Azure App Service Managed Instance 정식 지원](https://azure.microsoft.com/updates?id=568952)
온프레미스 및 VM 기반 .NET 애플리케이션을 무코드 변경으로 PaaS 환경에 통합 가능해집니다.

### [Dragon Copilot Physician Apps, Microsoft Marketplace 공개](https://azure.microsoft.com/updates?id=557775)
AI 기반 의료 워크플로우 자동화 앱·에이전트가 Marketplace에서 원스톱 구매 가능해져 임상 데이터 활용성 및 효율화가 더욱 강화됩니다.

### [Azure SQL, 8월 중순 업데이트](https://azure.microsoft.com/updates?id=569145)
SQL 관리 대시보드 내 단축키 커스터마이즈 등 사용 편의 기능이 추가되어 데이터 업무가 더욱 효율적이고 직관적으로 지원됩니다.


## ⏳ 서비스 사용 종료 및 정책 변화

서비스 정책에서 가장 큰 변화는 VMware 솔루션의 라이선싱 환경입니다. Broadcom의 라이선스 정책 변경에 따라 Azure VMware Solution License-included 서비스가 2027년 8월 30일부로 지원 종료되며, 모든 고객은 BYOL(Bring Your Own License) 방식으로 전환해야 합니다. 기존 서비스 중단을 예방하려면 라이선스 구매 및 환경 전환 로드맵을 신속하게 수립하고 VM SKU 교환 등 후속 조치를 진행해야 하며, 2026년 10월 15일 이후 기존 PayGo SKU도 단계적으로 사용 중단됩니다. 이 정책 변화는 Azure VMware Solution 활용 고객에게 매우 중대한 영향이 있으므로, 사전 대비가 반드시 필요합니다.

### [Azure VMware Solution License 포함 서비스, 2027년 8월 30일 지원 종료](https://azure.microsoft.com/updates?id=569535)
BYOL 방식 라이선스 구매·환경 전환이 필수화되며, 미리 로드맵을 수립해야 서비스 중단 없이 전환이 가능합니다.