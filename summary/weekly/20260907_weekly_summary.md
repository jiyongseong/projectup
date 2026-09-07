# Azure 주간 업데이트 요약 - 2026년 09월 07일

## ⚙️ 컴퓨팅 및 컨테이너
지난주 Azure 컴퓨팅 및 컨테이너 분야에서는 클라우드 인프라의 성능 최적화와 보안 강화가 특히 두드러졌습니다. Azure Kubernetes Service(AKS)는 Artifact Streaming을 정식 지원, 대형 컨테이너 이미지의 풀링 병목을 극복해 실시간 워크로드 확장성을 제공하므로 대규모 서비스 환경에 적합한 투명한 확장 모델을 구축할 수 있습니다. Azure Linux 기반 기밀 VM 지원으로 민감한 데이터와 컨테이너 워크로드를 무중단으로 고도 보안 환경으로 이전할 수 있으며, Windows Server 2025를 AKS에서 정식 지원해 최신 Windows 콘테이너 워크로드의 안정적 운영, FIPS 기본 보안 활성화 등이 보장됩니다. 또한, Microsoft Defender for Cloud가 Azure Container Apps까지 보안 체계를 확장하면서 컨테이너 환경 운영 전반에서 위험 평가와 공격 경로 분석 등 보안 통합 관리가 용이해졌습니다. 이러한 변화는 다양한 운영 요구와 민감 워크로드에 대응하는 클라우드 플랫폼의 진화된 역량을 보여줍니다.

### [정식 지원] AKS에서 Artifact Streaming 출시
AKS의 Azure Container Registry 연동으로 이미지 풀링 지연 없이 신속한 워크로드 확장 및 배포가 가능해집니다.

### [정식 지원] Azure Linux용 Confidential VM 지원
Azure Linux 기반 AKS에서 기밀 VM을 통한 민감 컨테이너 워크로드 보호와 무중단 마이그레이션이 가능합니다.

### [정식 지원] AKS에서 Windows Server 2025 지원
최신 Windows Server 환경에서 컨테이너 배포와 안정성, 기본 보안 기능(FIPS 등) 활성화가 지원됩니다.


## 🛠️ 관리 및 거버넌스
관리 및 거버넌스 분야에서는 로그 데이터와 AI 기반 모니터링, 비용 및 회계 관리 기능이 크게 강화되었습니다. Azure Monitor Auxiliary Logs Plan은 표준 Azure Table 및 커스텀 테이블을 자유롭게 지원하며, Analytics와 Auxiliary 플랜 간 테이블 전환 기능으로 로그 저장 비용과 관리 효율성 모두 높아졌습니다. Azure Copilot Observability Agent는 Basic/Auxiliary 테이블 플랜 지원으로 대용량 텔레메트리를 저비용으로 관리하고, Kubernetes 운영 데이터의 AI 분석 범위를 확장합니다. Microsoft Marketplace 구매 주문 매핑 기능은 구매 내역을 3개월 후까지 회계 시 재매핑할 수 있어 비용 추적 및 내부 회계 프로세스를 더욱 탄력적으로 개선할 수 있습니다. 이와 같이 운영 효율성, 분석 유연성, 비용 관리의 통합적 발전이 Azure 자원의 전략적 이용을 강화합니다.

### [정식 지원] Azure Monitor Auxiliary Logs Plan Azure Table 및 플랜 전환 지원
표준 Azure 테이블 및 DCR 커스텀 테이블 관리, 플랜 전환으로 로그 관리 유연성과 비용 절감 효과가 극대화됩니다.

### [정식 지원] Azure Copilot Observability Agent의 Basic/Auxiliary 테이블 플랜 지원
대용량 로그를 저비용으로 저장, AI 기반 분석 확대, Kubernetes 운영 데이터의 효율적 탐색 실현.

### [정식 지원] Microsoft Marketplace 구매 주문 매핑 기능
클라우드 및 AI 서비스 비용을 회계 기준에 맞춰 최대 3개월 후까지 재매핑, 비용 관리와 회계 연동의 유연성 강화.


## 🌐 네트워킹 및 보안
네트워킹 및 보안 영역에서는 자동화와 보안 정책 세분화가 주요 트렌드였습니다. Azure Firewall의 자동 SNAT 경로 학습이 도입되어 원본 IP 보존과 SNAT 관리를 자동화함으로써 네트워크 운영 복잡성을 줄였습니다. Azure Virtual Network Manager IPAM 기능은 여러 지역에서 IP 계획 중앙화 관리, 주소 충돌 방지를 제공하여 대규모 네트워크 인프라의 주소 공간을 더욱 안정적으로 관리할 수 있게 합니다. Azure Front Door의 WAF 정책 프로필/도메인/경로별 미리 보기 기능 도입으로 민감 경로에 맞춤형 보안 정책 적용이 가능해져 세밀한 보안 구성이 손쉽게 이루어집니다. 이 업데이트들은 네트워크 및 클라우드 보안 운영의 자동화와 효율성을 높이며, 글로벌 배포 환경에서도 신뢰성과 확장성을 확보하도록 지원합니다.

### [정식 지원] Azure Firewall 자동 SNAT 경로 학습
자동화된 경로 학습 및 No-SNAT 적용으로 원본 IP 보존과 SNAT 관리 효율화 달성.

### [정식 지원] Azure Virtual Network Manager IPAM, 추가 지역 지원
여러 지역에서 IP 관리 중앙화, 네트워크 충돌 방지로 글로벌 네트워크 운영에 안정성 제공.

### [미리 보기] Azure Front Door 프로필/경로별 WAF 정책 지원
WAF 정책 세분화로 민감 경로 및 도메인별 맞춤형 보안 설정 가능, 효율적인 보안 관리 실현.


## 🖥️ 스토리지 및 데이터베이스
지난주 Azure 스토리지 및 데이터베이스 분야는 데이터 처리 신뢰성과 확장성에서 큰 발전을 보였습니다. Azure VM의 Per-disk resiliency 기능(미리 보기)은 단일 디스크 장애 발생 시 해당 디스크만 분리·복구가 가능하며, VM과 다른 디스크는 지속적으로 운용되어 핵심 워크로드의 고가용성 보장에 중요한 역할을 합니다. Azure Database for MySQL의 reader endpoint 기능(미리 보기)은 다수의 읽기 리플리카에서 자동으로 읽기 트래픽을 분산 처리하여 아키텍처를 단순화하고 성능을 개선합니다. Azure Monitor Auxiliary Logs Plan이 정부 및 중국 지역까지 지원 범위를 확장해 대용량 로그 데이터 관리 효율화와 준수 요구에 특화된 저장 및 분석 환경을 제공합니다. 이러한 기능들은 클라우드 데이터 관리와 고가용성 인프라의 표준을 더욱 높이고 있습니다.

### [미리 보기] Azure VM Per-disk resiliency 기능
장기간 디스크 연결 장애 시 장애 디스크만 분리·복구, VM및 다른 디스크는 무중단 운용 가능.

### [미리 보기] Azure Database for MySQL Reader Endpoint 지원
최대 10개 리플리카에서 단일 엔드포인트로 읽기 트래픽 자동 분산, 아키텍처 단순화와 성능 향상 제공.

### [정식 지원] Azure Monitor Auxiliary Logs Plan, 정부 및 중국 지역 지원
대용량 준수·감사 로그의 비용 효율적 관리와 글로벌 표준 준수를 정부 및 중국 지역에서도 구현.


## 🚀 하이브리드 및 멀티클라우드
하이브리드 및 멀티클라우드 분야에서는 다양한 클라우드 환경 간 연결성 및 운영 편의가 대폭 강화되었습니다. Azure Multicloud Interconnect 서비스(미리 보기)는 Azure와 AWS 등 주요 클라우드 간 프라이빗 네트워크를 신속하게 구성할 수 있으며, 단일 포털에서 직접 연동, 높은 내구성과 실시간 네트워크 상태 모니터링 등이 구현되어 복수 클라우드 환경의 분산 워크로드, 데이터 이동, AI 서비스 운영이 효율적으로 진행됩니다. 공식 문서와 블로그를 통해 서비스 온보딩, 운영 가이드, 주요 사례 등 실제 전략적 멀티클라우드 접속 방법이 상세히 제공되어 기업의 멀티클라우드 도입과 운용을 지원합니다. 이러한 기능은 클라우드 운영의 복잡성을 줄이고 혁신 전략 실현의 기반을 마련합니다.

### [미리 보기] Azure Multicloud Interconnect 서비스 출시
주요 클라우드 간 프라이빗 멀티클라우드 네트워크 접속을 손쉽게 설정, 복잡한 워크로드 분산 및 운용 효율 극대화.

### [Azure Multicloud Interconnect 공식 문서](https://aka.ms/AzureMulticloudInterconnect_learn)
온보딩, 운영, 클라우드 환경별 특징 및 연동 기술 가이드 제공.

### [Azure Multicloud Interconnect 출시 블로그](https://aka.ms/MulticloudInterconnect-blog)
멀티클라우드 접속 전략과 신규 기능, 주요 적용 사례 등 구체적 운영 방법 소개.