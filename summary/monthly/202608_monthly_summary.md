# Azure 월간 업데이트 요약 - 2026년 08월

## 전반적인 트렌드 및 핵심 인사이트

2026년 8월 Azure 업데이트에서는 하이브리드 및 멀티클라우드 지원의 확장, 네트워크 및 보안 기능 강화, 대규모 AI·데이터 분석 플랫폼의 지역 확장과 높은 성능 VM의 추가 출시, 일관된 개발 경험을 위한 툴의 개선, 그리고 운영 효율 및 관리 자동화 솔루션의 강화가 두드러집니다. 특히 애플리케이션, 데이터, 인프라 전반에 걸쳐 정식 지원(General Availability)이 대거 추진되었으며, 프리뷰(미리 보기) 기능도 많이 공개되어 Azure 플랫폼이 안정성과 확장성, 보안성을 지속적으로 강화하고 있습니다.

네트워크 부문에서는 Azure Firewall 및 Azure Bastion·AKS에서의 성능 최적화와 IPv6 지원, 대규모 라우팅 및 관리 기능의 향상이 적극적으로 반영되었습니다. 컴퓨트 영역은 vCPU 크기 확장, VM 이미지 빌더의 에어갭·주권 클라우드 지원, vCore 커스터마이즈와 신속한 스토리지 확장 등이 눈에 띕니다. 데이터 및 AI 영역에서는 Azure Databricks의 기능 확대와 지역 추가, SQL Database의 불변성 강화, AI 거버넌스 및 연결 기능이 정식 출시되며, 글로벌 데이터 분석 플랫폼의 서비스 지속 강화가 이루어지고 있습니다.

운영 자동화 및 DevOps 측면에서는 SRE Agent의 네트워크 통합·새로운 무료 체험, 관찰성 도구의 확장, 규정 준수와 위험 관리 지원이 뚜렷하게 나타났습니다. 또한 Marketplace 구매 프로세스 간소화, App Service의 관리 인스턴스·마크다운 지원 등 개발·운영자 모두의 편의성이 크게 개선되었습니다.

프리뷰 및 사용 중단/지원 종료 항목도 공개되어 Azure의 서비스 생명주기가 명확히 관리되고 있습니다. 대형 서비스의 라이선스 변경, 서비스 종료 및 업그레이드 관련 안내도 지속적으로 제공되며, 고객의 지속적인 업그레이드·전환을 요구합니다. Microsoft Fabric과 Foundry 등 신기술도 적극 반영되어 통합 관리를 지원하는 기능들이 확대되고 있습니다.

## 🔒 네트워크 및 보안

이번 달에는 네트워크 성능과 보안 측면에서 주요 기능이 정식 지원되었습니다. Azure Firewall의 IDPS 성능 향상, 명시적 프록시 및 IPv6 프리뷰, Bastion과 AKS의 결합, Application Gateway WAF의 사용자 정의 응답, Virtual Network 라우팅 장치의 출시 등이 집중적으로 이루어졌습니다. 동시에 Front Door의 일괄 규칙 관리와 BYON 기능을 통한 재해 복구의 네트워크 유연성도 확대되었습니다.

### [2.2X IDPS 성능 최적화 in Azure Firewall](https://azure.microsoft.com/updates?id=569256)
Azure Firewall Premium의 TLS 검사 및 IDPS 처리 성능이 최대 22Gbps로 향상되었으며, TCP 연결당 IDPS 처리도 600Mbps까지 증가해 대규모 네트워크 환경에서 보안성과 성능을 동시에 확보할 수 있게 되었습니다.

### [Azure Bastion 공유 링크 만료 기능 정식 지원](https://azure.microsoft.com/updates?id=570020)
Azure Bastion에서 공유 링크의 만료일시 지정이 가능해져, 임시 접속과 장기적 접근을 효과적으로 제한할 수 있습니다. 이 기능은 보안 및 접근 관리 측면에서 조직의 거버넌스에 큰 도움이 됩니다.

### [Azure Virtual Network 라우팅 장치 정식 지원](https://azure.microsoft.com/updates?id=568605)
전용 하드웨어 기반 라우팅 장치가 VNet에 추가됨으로써 고대역폭, 저지연 동서 라우팅을 실현하며, IPv6, 듀얼스택 지원과 전역 프라이빗 연결이 가능해졌습니다.

### [Azure Firewall 명시적 Proxy 기능 정식 지원](https://azure.microsoft.com/updates?id=568825)
명시적 프록시 설정을 통해 HTTP/HTTPS 트래픽을 Firewall로 직접 전달 가능해지고, PAC 파일·Portal 연동 등으로 외부 접근 및 세분화된 제어가 용이해졌습니다.

### [Application Gateway WAF 차단 응답 커스터마이징 정식 지원](https://azure.microsoft.com/updates?id=569504)
웹 애플리케이션 방화벽의 차단 요청 응답 코드와 메시지를 사용자가 정의할 수 있어, 비즈니스 시나리오별로 상세 응답 제어가 가능해졌습니다.

## 💻 컴퓨트 및 인프라

할당 가능 vCPU 크기의 대폭 확대, VM 이미지 빌더의 신뢰 클라우드 지원, Managed Instance App Service의 정식 지원, 디스크/스토리지 실시간 확장, vCore 커스터마이즈 등 인프라 효율성과 확장성을 극대화하는 업데이트가 이루어졌습니다. 특히 메모리·네트워크·스토리지 성능과 커스터마이즈 기능이 강조되었습니다.

### [Azure 248/372 vCPU D/E v7 VM 크기 정식 지원](https://azure.microsoft.com/updates?id=569546)
최대 372 vCPU·2.8TiB 메모리로 확장 가능한 D/E v7 시리즈 VM이 출시되어, 대용량 DB와 AI 워크로드·저지연 어플리케이션 운영에 적합한 인프라 환경을 제공합니다.

### [Azure VM Image Builder 주권/에어갭 클라우드 정식 지원](https://azure.microsoft.com/updates?id=570105)
Azure Government, 중국, 에어갭 환경까지 VM 이미지 빌더 서비스가 정식 지원되어, 규제 산업·공공기관 환경에서 일관된 이미지 파이프라인과 보안 설정을 운용할 수 있게 되었습니다.

### [Live Resize for Shared Premium SSD v2/Ultra Data Disks 정식 지원](https://azure.microsoft.com/updates?id=569281)
실시간 디스크 확장 기능이 새롭게 지원되어, 운영 중에도 애플리케이션 중단 없이 스토리지 용량을 동적으로 확대할 수 있습니다.

### [vCore 커스터마이즈: SMT/HT 비활성화 및 코어 수 구성](https://azure.microsoft.com/updates?id=569051)
SMT/HT 비활성화 및 코어 수 조정 기능이 제공되어, 라이선스 비용 최적화와 워크로드별 맞춤 성능 구성이 가능합니다. SQL Server 등 라이선스 기반 워크로드에 적합합니다.

### [Managed Instance on Azure App Service 정식 지원](https://azure.microsoft.com/updates?id=568952)
온프레미스 또는 VM에 있는 .NET 기반 복잡한 앱도 코드 변경 없이 App Service로 마이그레이션 가능하며, Windows 서비스와 다양한 엔터프라이즈 기능을 활용할 수 있게 됩니다.

## 🗄️ 데이터 및 AI · 분석

데이터 영역에서는 Azure Databricks의 지역 확장, Lakebase 정식 지원, AI Gateway와 SharePoint Connector 출시 등 데이터 연결·거버넌스 기능이 강화되었습니다. SQL Database에서는 불변 백업, 빠른 프로비저닝, 단축키 커스터마이즈, PostgreSQL 사전 검증, Databricks Runtime 종료 예정 등 데이터 신뢰성·운영성 개선이 이뤄졌습니다.

### [Azure Databricks Lakebase 4개 지역 추가](https://azure.microsoft.com/updates?id=569684)
Lakebase의 정식 지원 지역이 북미·유럽·동아시아로 확장되어, 글로벌 대용량 데이터 워크로드의 분산 및 확장성이 한층 높아졌습니다.

### [SharePoint Connector for Azure Databricks 정식 지원](https://azure.microsoft.com/updates?id=568905)
Lakeflow Connect를 통해 SharePoint 문서를 Databricks에 직접 유입·AI/분석 워크플로우와 통합 가능하며, 기업 콘텐트와 데이터 중심의 AI 업무 혁신이 실현됩니다.

### [Azure SQL Database 프로비저닝 및 단축키 커스터마이즈 정식 지원](https://azure.microsoft.com/updates?id=569160)
에디터 내에서 Azure SQL Database를 직접 생성·연결할 수 있게 되고, 자동화 템플릿과 단축키 커스터마이즈로 개발 생산성이 크게 향상됩니다.

### [Azure SQL Database 백업 7일 불변성 정식 지원](https://azure.microsoft.com/updates?id=568339)
자동으로 최신 7일 백업이 불변성을 유지하게 되어, 랜섬웨어/데이터 손실 방지에 크게 기여합니다.

### [Azure Database for PostgreSQL Flexible Server 사전 검증 체크 정식 지원](https://azure.microsoft.com/updates?id=568419)
버전 업그레이드 전 사전 검증 기능으로, 확장성 및 신뢰성 있는 운영 환경 확보가 가능합니다. 장애 발생 가능성을 미리 파악·해결할 수 있습니다.

## 🛠️ DevOps · 운영 관리 및 Marketplace

운영 자동화 및 DevOps 부문에서는 Azure SRE Agent의 무료 체험과 VNet 연동, AKS 관찰성(Managed Prometheus), Front Door 규칙 일괄관리, SaaS 구매 간소화 등의 기능이 정식 지원되었습니다. 재해 복구 환경(BYON), Marketplace 및 Copilot 구매·운영 개선 등 다양한 형태의 운영, 관리 효율성이 확대되고 있습니다.

### [Azure SRE Agent 30일 무료 체험 및 VNet 통합 정식 지원](https://azure.microsoft.com/updates?id=569760)
SRE Agent를 30일간 자유롭게 체험 가능하며, VNet 연동으로 네트워크 보안·프라이빗 리소스 접근까지 확장되어 DevOps 현장에 효율적으로 적용할 수 있습니다.

### [AKS 컨트롤 플레인 메트릭 수집 정식 지원](https://azure.microsoft.com/updates?id=568830)
Azure Monitor Managed Prometheus를 활용한 AKS 컨트롤 플레인 모니터링으로 오케스트레이션/운영 상태를 더 깊이 분석할 수 있습니다.

### [Azure Front Door 규칙 일괄 업데이트 정식 지원](https://azure.microsoft.com/updates?id=569246)
규칙 세트 일괄 관리로 대규모 정책 변경에서 일관성·안정성이 크게 개선됩니다.

### [Azure Site Recovery BYON NIC 기능 정식 지원](https://azure.microsoft.com/updates?id=569515)
재해 복구 시 네트워크 구성과 IP를 미리 준비할 수 있어, 운영 환경 복원에 더욱 유연한 제어가 가능합니다.

### [Marketplace SaaS 단일 클릭 구매 경험 정식 지원](https://azure.microsoft.com/updates?id=568591)
Azure Portal에서 SaaS 제품 구매시 모든 필수 정보를 한 번에 확인하고, 간소화된 구매 과정을 통해 빠른 서비스 준비가 이루어집니다.

## 📦 스토리지 및 데이터 관리

스토리지 관리의 동적 확장과 컨테이너 환경 연계, Azure Files 및 AKS 연동 등 저장소·데이터 연동 기능이 크게 강화됐습니다. 프리뷰에서는 AWS 파일서버에서 Azure Files로의 에이전트리스 마이그레이션, 듀얼스택·퍼시스턴트 볼륨 등 다양한 연결 시나리오가 편리하게 지원됩니다.

### [Live Resize for Shared Premium SSD v2/Ultra Data Disks 정식 지원](https://azure.microsoft.com/updates?id=569281)
운영 중 스토리지 크기를 다운타임 없이 증대할 수 있어, 비용 최적화 및 확장성이 보장됩니다.

### [Azure Files CSI 드라이버(컨테이너 저장소) Workload ID 지원 정식](https://azure.microsoft.com/updates?id=570120)
AKS 내 Workload ID 기반 SMB 파일 공유 연동으로, Pod 단위의 최소 권한 접근 및 보안 요건 충족이 가능해집니다.

### [Azure Storage Mover AWS FSx에서 Azure Files로 마이그레이션 프리뷰](https://azure.microsoft.com/updates?id=567979)
에이전트 없이 AWS FSx에서 Azure Files로 직접 데이터 이전이 가능해져, 클라우드 간 이동이 쉽고 관리 부담이 줄어듭니다.

### [Azure Private Link IPv6 지원 프리뷰](https://azure.microsoft.com/updates?id=568842)
IPv6 기반 Private Endpoint를 통해 Azure PaaS 서비스를 프라이빗하게 연동할 수 있습니다.

### [Azure Bastion IPv4/IPv6 듀얼스택 프리뷰](https://azure.microsoft.com/updates?id=570025)
새롭게 구축되는 Bastion 환경에서 IPv4·IPv6 듀얼스택 공용 IP를 지원합니다.

## ⚙️ 관리, 거버넌스, 서비스 생명주기

관리 및 거버넌스 부문에서는 대규모 라우팅 프리픽스, Trusted Launch 기본화, 서비스 생명주기 관리(라이선스/이미지/노드 지원 종료 예정), Copilot/Marketplace 운영 개선, 서비스 종료 및 지원 정책 공지가 제공됐습니다.

### [게이트웨이 라우트 광고 프리픽스 요약 정식 지원](https://azure.microsoft.com/updates?id=569743)
ExpressRoute/VPN Gateway에서 대규모 프리픽스 요약이 가능해져, 라우팅 효율성과 확장성이 향상됨.

### [Trusted Launch 기본값으로 정식 지원](https://azure.microsoft.com/updates?id=568600)
Secure Boot/vTPM이 Gen2 VM 및 VM Scale Set 신규 배포시 자동 활성화되어 기본 보안성을 강화합니다.

### [Azure VMware Solution 라이선스 포함 서비스 2027년 8월 30일 지원 종료](https://azure.microsoft.com/updates?id=569535)
브로드컴 라이선스 정책 변화에 따라 AVS의 라이선스 포함 서비스가 종료되며, 고객은 BYOL(Bring Your Own License)로 전환 필요.

### [Azure Databricks Runtime 10.4 LTS 2026년 11월 1일 서비스 종료 안내](https://azure.microsoft.com/updates?id=569353)
2026년 말 Databricks Runtime 10.4 LTS가 공식적으로 종료되어, 관련 클러스터와 워크로드는 상위 버전으로 이전이 요구됩니다.

### [Node 22 LTS 2027년 4월 30일 지원 종료 안내](https://azure.microsoft.com/updates?id=567334)
App Service에서 Node 22 LTS 지원이 종료되며, 최신 Node 버전으로 업그레이드 필요성과 보안 리스크 감소에 대한 가이드가 공개되었습니다.

## 🧪 프리뷰 기능 및 혁신

프리뷰에서는 IPv6/듀얼스택 네트워크, Databricks의 기능 확장, SQL Database의 데이터 마스킹, Azure Linux on WSL, 퍼리미터 링크, 네트워크 라우트맵 등 다양한 실험적 신기술이 공개되어 Azure의 미래 로드맵을 제시하고 있습니다.

### [Azure DNS Traffic Manager 연동을 통한 DNS 기반 로드밸런싱 프리뷰](https://azure.microsoft.com/updates?id=565214)
CNAME hop을 제거하고 DNSSEC 호환성을 지원하며, Azure DNS-트래픽 매니저 연동 기능 개선.

### [Azure ExpressRoute 레질리언시 가드 프리뷰](https://azure.microsoft.com/updates?id=568666)
싱글/멀티홈 환경에 맞춘 네트워크 resiliency 구성을 손쉽게 안내하고, 변경 리스크를 줄여줍니다.

### [Azure Bastion IPv6 듀얼스택 프리뷰](https://azure.microsoft.com/updates?id=570025)
사용자에서 Bastion까지 IPv6를 활용한 연결이 가능해짐.

### [Azure Firewall IPv6 듀얼스택 프리뷰](https://azure.microsoft.com/updates?id=569520)
IPv6 네이티브 트래픽 필터링 및 DNS Proxy 기능이 지원되며, 하이브리드 환경의 보안성이 강화됩니다.

### [Azure Linux on WSL 프리뷰](https://azure.microsoft.com/updates?id=569376)
개발 환경부터 운영까지 Azure Linux를 일관적으로 활용 가능하며, 생산환경과 개발 환경의 차이를 줄이고 버그 및 이슈 확인이 빠르게 이루어집니다.

## 🤖 AI · 애널리틱스 · 혁신적 서비스

AI 및 분석 플랫폼에서 Databricks의 Lakebase, Genie Agent 무료 제공, AI Gateway, Marketplace 연동, Copilot 기능 등이 강조되며, Microsoft Fabric의 기본 복구 기능, Postgres Extended Support 등 고도화된 관리와 AI 거버넌스가 눈에 띕니다.

### [Azure Databricks Genie One 및 Genie Agents 무료 사용 기간 연장 안내](https://azure.microsoft.com/updates?id=568964)
Genie One 및 Genie Agents의 무료 사용이 2027년 1월 31일까지 연장되어, 사용자 중심 AI 분석의 저변 확대에 기여합니다.

### [Unity AI Gateway on Azure Databricks 정식 지원](https://azure.microsoft.com/updates?id=568910)
AI 모델, 에이전트, 도구의 중앙 거버넌스와 비용 관리, 액세스 제어, 외부 AI 서비스 통합 등 AI 업무의 관리와 보안이 체계적으로 강화됩니다.

### [Dragon Copilot Physician App/Agent Marketplace 연동 정식 지원](https://azure.microsoft.com/updates?id=557775)
Microsoft Marketplace에서 Dragon Copilot 앱 및 에이전트의 구매가 가능해져 의사 업무 보조 AI 도입이 더 빨라지고, 효율적 기획·구매가 실현됩니다.

### [Azure Copilot 에이전트 직접 접근 기능 발표](https://azure.microsoft.com/updates?id=569685)
트러블슈팅·최적화·배포·탄력성 등 Copilot 에이전트를 직접 선택·활용할 수 있어서, 운영 자동화·관리 지능화가 실제 서비스로 확장됩니다.

### [Microsoft Fabric Item Recovery 기본 설정 활성화 발표](https://azure.microsoft.com/updates?id=569140)
Fabric 테넌트의 Item 복구 기능이 기본 활성화되어, 3일간의 복구 윈도우 제공으로 데이터 손실 위험이 크게 줄어듭니다.

## 총평 및 다음 달 전망

2026년 8월 Azure 업데이트는 대규모 정식 지원 기능 출시와 프리뷰 혁신 기능 공개가 균형 있게 이루어졌으며, 하이브리드/멀티클라우드 지원, 네트워크 성능, 데이터 신뢰성, 운영 자동화, 개발 운용 편의성 등 플랫폼 전반의 품질에 큰 향상이 있었습니다. 서비스 종료 및 라이선스 전환, 지원 정책 변화 안내로 고객의 클라우드 생명주기가 더욱 명확해졌으며, AI·분석 거버넌스와 보안 체계도 고도화되고 있습니다.

다음 달에는 프리뷰에서 정식 지원으로의 전환과 더 많은 AI 거버넌스·운영 자동화 기능 공개, 글로벌 인프라 확장, 네트워크/보안 기반 기능들의 추가 발표가 기대됩니다. Azure는 기업 IT 환경에서 요구되는 신뢰성·확장성·운영 효율성을 바탕으로 디지털 혁신의 중심을 계속 이어갈 전망입니다.