# Azure 주간 업데이트 요약 - 2026년 08월 10일

## 🌐 네트워킹 및 보안

지난주 Azure는 네트워킹과 보안 분야에서 다양한 정식 지원과 미리 보기 기능을 선보였습니다. Azure Virtual Network Routing Appliance의 정식 지원으로 네트워크 간 고성능·저지연 연결이 가능해졌으며, 이는 글로벌 및 지역 간 프라이빗 엔드포인트 연동, IPv6 네트워크 강화, 운영 자동화와 가용성 보장 등 실질적 네트워크 성능 향상을 의미합니다. Azure Firewall의 Explicit Proxy 정식 지원은 HTTP/HTTPS 트래픽을 중앙화된 경로로 통제하며 보안 정책의 자동화와 하이브리드 환경 구축에 핵심 역할을 하게 됩니다. DNS 기반 트래픽 관리와 DNSSEC 보안강화, ExpressRoute 복원력 가드 도입, Private Link의 IPv6 지원 등 미리 보기 기능들은 네트워크 경계, 데이터 보호, 확장성 요구에 보다 효율적으로 대응할 수 있는 강력한 옵션을 제공합니다. 이런 변화는 다중 지역 및 하이브리드 환경에서의 연동성과 취약점 대응, 운영 편의성을 대폭 강화하며 최신 클라우드 네트워크의 신뢰성과 유연성을 한 단계 끌어올릴 것으로 전망됩니다.

### [Azure Virtual Network Routing Appliance 정식 지원](https://azure.microsoft.com/updates?id=568605)
고성능 하드웨어를 활용한 최대 200Gbps급 네트워크 라우팅, IPv6/IPv4 듀얼 스택 지원, 글로벌 및 지역 프라이빗 엔드포인트 연계 등 네트워크의 성능과 안정성을 획기적으로 향상시키는 업데이트입니다.

### [Azure Firewall Explicit Proxy 정식 지원](https://azure.microsoft.com/updates?id=568825)
HTTP/HTTPS 트래픽을 Azure Firewall로 직접 라우팅해 통제 효과를 극대화하며, Azure Arc 등 하이브리드 환경에서 보안성과 운영 편의성을 크게 개선할 수 있습니다.

### [Azure DNS Traffic Manager 연동 미리 보기 출시](https://azure.microsoft.com/updates?id=565214)
DNS 레코드와 Traffic Manager를 직접 연결하여 CNAME 루프 지연을 제거하고 DNSSEC 호환성을 강화해, DNS 기반 로드밸런싱의 속도와 보안성이 개선되었습니다.

---

## 🖥️ 컴퓨트 및 VM

컴퓨트 및 가상 머신 영역에서는 기본 보안 정책의 자동화와 VM 시리즈 변경, 고가용성 네트워크 관리 옵션이 주요 업데이트로 공개되었습니다. Trusted Launch의 기본값 적용은 Gen2 VM 및 VM 스케일셋 전체에 Secure Boot와 vTPM을 자동화하여, 추가 비용 없이 엄격한 보안 기준을 실현하게 합니다. cc_v5 컨피덴셜 VM 시리즈의 2026년 9월 지원 종료 예고는 반드시 VM 크기 조정이 필요한 고객을 미리 준비시키고, 컴플라이언스 및 플랫폼 최적화의 연계 정책을 촉진합니다. ExpressRoute 복원력 가드 미리 보기 출시는 네트워크 게이트웨이 구성의 신뢰도를 극대화하고 하이브리드 및 멀티사이트 운영 구조에 맞는 복원력 방안을 제시하여, 네트워크·컴퓨트 자산의 안정성을 보강하는 데에 중점을 두고 있습니다. 전반적으로 컴퓨트 영역에서는 운영 안정성과 보안, 비용 최적화를 실현할 수 있도록 플랫폼 기본 정책과 VM 운영 방침이 개선되고 있습니다.

### [Trusted Launch 기본값 적용 정식 지원](https://azure.microsoft.com/updates?id=568600)
Gen2 VM·VM 스케일셋에 Secure Boot, vTPM 자동 활성화로 클라우드 워크로드의 보안 기준을 실질적으로 높였습니다.

### [cc_v5 컨피덴셜 VM 시리즈 지원 종료 예고](https://azure.microsoft.com/updates?id=568661)
DCas_cc_v5, DCads_cc_v5, ECas_cc_v5, ECads_cc_v5 등 VM은 2026년 9월 1일부로 지원 종료되며, 미리 크기 조정이 반드시 필요합니다.

### [ExpressRoute 복원력 가드 미리 보기 출시](https://azure.microsoft.com/updates?id=568666)
Single-homed/멀티홈드 맞춤 복원력 설정, 포털 안내, 보안 구성으로 네트워크 안정성·복원력을 극대화할 수 있습니다.

---

## 💾 데이터 및 AI/애널리틱스

데이터 및 AI·애널리틱스 분야에서는 보안과 중앙화된 데이터 거버넌스, 엔터프라이즈 연동성이 크게 향상됐습니다. Azure SQL Database/Managed Instance의 자동 백업 불변성 적용은 데이터 무결성과 복원력 강화, Ransomware 등 위협 대응에 중요한 역할을 하며, 별도 설정 없이 점진적 복구 보장을 제공합니다. Azure Databricks의 SharePoint Connector 정식 지원은 엔터프라이즈 파일과 AI/데이터 워크플로를 원활히 통합할 수 있게 하여 데이터 기반 서비스의 확장성과 효율성을 크게 개선합니다. Unity AI Gateway 정식 지원은 다양한 AI 모델·도구·서비스의 중앙 통제와 가드레일 적용, 비용·사용 관리 기능을 한 플랫폼에서 구현하여 복잡한 AI 운영 환경의 거버넌스를 획기적으로 개선합니다. Genie One/Agents 무료 사용 기간 연장 등 Databricks 내 프로모션 정책은 AI·분석 서비스의 진입장벽을 낮추고, 서비스 활용 활성화에 기여하고 있습니다.

### [Azure SQL Database 및 Managed Instance 백업 불변성 적용](https://azure.microsoft.com/updates?id=568339)
지난 7일간 모든 DB 백업에 자동적으로 불변성 적용, 데이터 무결성과 복구 보장, Ransomware 위협 대응에 적합합니다.

### [Azure Databricks SharePoint Connector 정식 지원](https://azure.microsoft.com/updates?id=568905)
Lakeflow Connect를 통해 SharePoint 파일을 Databricks로 인제스트, 엔터프라이즈 데이터와 AI 워크플로의 통합을 실현합니다.

### [Unity AI Gateway on Azure Databricks 정식 지원](https://azure.microsoft.com/updates?id=568910)
AI 모델·도구·서비스의 중앙 거버넌스, 비용·접근 관리, 가드레일 적용으로 복잡한 AI 운영 환경을 효율적으로 통제할 수 있습니다.

---

## 🚀 하이브리드 및 멀티클라우드

하이브리드 및 멀티클라우드 카테고리에서는 자산의 연동·이동성 개선, 데이터 복구 정책 강화, 보안 연동 기능이 확대되었습니다. AWS FSx에서 Azure Files로의 데이터 마이그레이션 기능이 미리 보기로 출시되어 별도의 에이전트 없이 안전하고 간편하게 파일 데이터를 이동할 수 있습니다. Azure SQL Database의 자동 백업 불변성 기능은 하이브리드 환경 맞춤 데이터 복구·보호 정책을 지원하고 보안 정책 강화에 적합하며, Private Link의 IPv6 지원 및 Azure Arc 온보딩 시 Azure Firewall Explicit Proxy 활용 등 다양한 멀티클라우드 환경에서 네트워크 확장성과 보안 관리성이 향상됩니다. 이러한 기능들은 여러 클라우드에서 일관된 데이터 보호, 네트워크 확장, 중앙화된 보안 정책을 적용할 수 있게 하여 대규모 분산 환경 운영에 있어 최적의 가용성·보안성을 제공합니다.

### [AWS FSx to Azure Files 마이그레이션 미리 보기 출시](https://azure.microsoft.com/updates?id=567979)
네이티브 에이전트 불필요, 클라우드-클라우드 간 파일 데이터의 안전·신속 이전 지원으로 업무 연속성 강화.

### [Azure SQL Database 백업 불변성 (하이브리드 환경 적용)](https://azure.microsoft.com/updates?id=568339)
자동적으로 모든 DB에 불변성 적용, 하이브리드·멀티클라우드 환경에서 데이터 복구·보호 정책 강화에 적합한 업데이트.

### [Azure Firewall Explicit Proxy 활용한 Azure Arc 온보딩](https://azure.microsoft.com/updates?id=568825)
Azure Arc 서버와 Azure Firewall 통합으로 하이브리드 환경의 보안 통제와 중앙화된 접속제어 기능 확장.

---

## 🛡️ 애플리케이션 및 서비스 연동

애플리케이션 및 서비스 연동 분야에서는 프라이빗 네트워크 연동의 범위 확장과 보안 경계 간 신뢰 통신 강화, 엔터프라이즈 콘텐츠 통합 등이 이뤄졌습니다. Azure Private Link에서 IPv6 지원이 미리 보기로 제공되어 주요 Azure PaaS와의 프라이빗 연결 옵션이 확대되고, 네트워크 확장성과 신뢰성 세분화가 가능해집니다. Perimeter Link 기능 미리 보기 출시는 Managed Identity 기반으로 네트워크 보안 경계 간의 신뢰 통신을 제공하여 Zero Trust 모델 실현을 강화하고, 서비스 간 중앙 통제와 인증의 효율성을 높입니다. SharePoint Connector 출시로 기업 콘텐츠와 AI/데이터 워크플로우의 대규모 연동·배포가 가능해졌으며, 다양한 인증 방식과 점진적 인제스트 기능 등 효율적 데이터 연계 방안이 제시됩니다. 이로써 서비스-네트워크 간 수직·수평 확장성과 보안 경계의 신뢰 모델이 한층 진보되었습니다.

### [Azure Private Link IPv6 지원 미리 보기 출시](https://azure.microsoft.com/updates?id=568842)
Azure Storage, Azure SQL Database 등 주요 PaaS와의 IPv6 기반 프라이빗 연결 지원으로 네트워크 연동성과 확장성 증대.

### [네트워크 보안 경계 Perimeter Link 기능 미리 보기 출시](https://azure.microsoft.com/updates?id=568837)
Managed Identity 기반으로 별도 구성 없이 네트워크 경계 간 보안 통신 지원, Zero Trust 환경 실질 강화.

### [SharePoint Connector for Azure Databricks 정식 지원](https://azure.microsoft.com/updates?id=568905)
기업 콘텐츠·AI/데이터 워크플로우 통합, 다양한 인증방식, 단계적 인제스트 등 대규모 연동 배포를 지원합니다.