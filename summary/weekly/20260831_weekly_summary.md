# Azure 주간 업데이트 요약 - 2026년 08월 31일

## 🖥️ 컴퓨트 및 VM

지난주 Azure의 컴퓨트와 VM 분야에서는 신규 VM 사이즈의 정식 지원, 자동화 에이전트의 체험판, 보안·컴플라이언스에 특화된 이미지 빌더 등 강력한 성능 확장과 표준화된 구축 관리가 주요 이슈였습니다. 인텔® Xeon® 6 기반의 D/E v7 시리즈 VM은 최대 372 vCPU, 2.8TiB 메모리, 400Gbps 네트워크 대역폭, 9.6M IOPS NVMe 성능을 제공하여 대규모 AI, 인메모리 데이터베이스, 초고성능 애플리케이션 지원을 강화합니다. VM 이미지 빌더는 주권/에어갭 환경까지 적용 범위를 넓혀 정부/공공 및 규제 산업 내 이미지 생성, 배포, 컴플라이언스 검증을 자동화합니다. SRE Agent의 30일 체험판 출시로 인프라 자동화 및 위험 탐지가 누구나 쉽게 실험 가능해졌습니다. Node 22 LTS 지원 종료 고지 또한 운영 앱의 신속한 업그레이드 필요성을 강조합니다.

### [Azure D/E v7 시리즈 VM 248/372 vCPU 사이즈 정식 지원](https://azure.microsoft.com/updates?id=569546)
인텔® Xeon® 6 기반 고성능 VM이 최대 372 vCPU까지 확장되어 대규모 AI·DB 워크로드 및 네트워크·스토리지 성능을 지원합니다.

### [Azure SRE Agent 30일 체험판 출시](https://azure.microsoft.com/updates?id=569760)
운영 자동화 에이전트(30일 무료 체험)로 알림 대응, 원인 분석, 위험 탐지·후속 조치까지 사전 실험이 가능합니다.

### [Azure VM Image Builder 주권·에어갭 클라우드 정식 지원](https://azure.microsoft.com/updates?id=570105)
정부·공공 및 규제 환경에서 표준 이미지 생성, 하드닝, 컴플라이언스 체크를 자동화하여 운영 일관성과 보안을 확보합니다.

---

## 🔒 네트워킹 및 보안

네트워킹 및 보안 카테고리에서는 Azure Bastion과 WAF(Application Gateway)의 기능 강화, AKS 연동, IPv6 듀얼스택 미리 보기 도입 등 접근 제어와 정책 유연성이 크게 향상되었습니다. Bastion 공유 링크 만료 일정을 직접 지정해 일시적 접근만 허용, 보안 정책 강화가 가능하며, WAF의 차단 응답 커스텀 코드 설정으로 사용자 경험 및 조직 맞춤 정책 대응력이 증가했습니다. 신규 배포된 Bastion의 IPv6 듀얼스택 지원은 향후 네트워크 확장 및 테스트 시 참고할 수 있습니다. 컨테이너 환경과 네트워킹의 통합이 진행되고 있으며, 보안·운영 효율이 더욱 높아지고 있습니다.

### [Azure Bastion 공유 링크 만료 정식 지원](https://azure.microsoft.com/updates?id=570020)
접근 만료 시각 지정으로 임시 링크를 통한 자원 접근 제어가 가능해져 보안·컴플라이언스 대응력이 높아졌습니다.

### [Application Gateway WAF 차단 응답 커스텀 코드·메시지 기능 정식 지원](https://azure.microsoft.com/updates?id=569504)
WAF가 차단한 요청에 대해 정책별 맞춤 응답 코드를 설정하고, 사용자 경험을 개선할 수 있습니다.

### [Azure Bastion IPv6 듀얼스택 지원 미리 보기](https://azure.microsoft.com/updates?id=570025)
IPv4/IPv6 주소 동시 배포가 가능해져 향후 네트워크 환경의 확장 및 테스트에 유연성을 제공합니다.

---

## 🐳 컨테이너 & AKS

Azure 컨테이너 및 AKS 부문에서는 네트워크 성능과 접근 제어, 스토리지 안전성에 대한 혁신 기능이 정식 지원으로 출시되었습니다. eBPF 기반 컨테이너 네트워크 라우팅으로 레이턴시 감소, 대규모 클러스터 운영에서 고성능·고확장성을 제공합니다. Bastion과 AKS API 연동을 통한 안전한 클러스터 API 접근이 가능해져 운영 효율과 보안성이 크게 향상됩니다. Azure Files CSI 드라이버의 워크로드 아이덴티티 지원으로, Pod 단위 최소 권한 접근과 컴플라이언스 대응력이 강화되었습니다. 이러한 기능들은 엔터프라이즈 및 규제 환경에서의 민감한 데이터와 워크로드를 안전하게 보호하면서 운영 효율을 극대화합니다.

### [AKS 고급 컨테이너 네트워크 eBPF 라우팅 정식 지원](https://azure.microsoft.com/updates?id=569873)
eBPF 기반 네트워크로 레이턴시 최소화, 고성능·고확장 클러스터 운영 및 운영 효율 개선이 가능합니다.

### [Azure Bastion 통한 AKS 클러스터 API 서버 연결 정식 지원](https://azure.microsoft.com/updates?id=570030)
Bastion 활용으로 AKS API 접속 시 공용 IP 노출 없이 안전한 관리가 가능해집니다.

### [AKS Azure Files CSI 운용 워크로드 아이덴티티 지원 정식 지원](https://azure.microsoft.com/updates?id=570120)
Pod 단위 인증 최적화로 민감 데이터 접근 제어 및 규제산업 환경에서 안전한 스토리지 연동이 가능합니다.

---

## ⚡ 운영 자동화 & 관리

운영 자동화 및 관리 분야에서는 인시던트 대응과 지속적 모니터링 체계를 혁신할 기능들이 본격화되었습니다. SRE Agent의 VNet 통합 정식 지원으로 민감 네트워크 환경에서도 자동화 에이전트가 안전하게 행동 가능하고, Live Reports 미리 보기 기능 출시로 동적 리포트를 일/주/월 단위 자동 갱신, 팀·운영 효율 및 신속 의사결정이 가능해졌습니다. Node 22 LTS 지원 종료(2027년 4월 30일 예정)는 App Service 내 운영앱의 사전 업그레이드 필요성을 알리고 있습니다. 이러한 관리 자동화 기술 도입은 보안·운영 리스크 최소화를 위한 선제적 대응에 필수적 변화를 제공합니다.

### [Azure SRE Agent VNet 통합 정식 지원](https://azure.microsoft.com/updates?id=569695)
민감 네트워크 환경(NSG, 프라이빗 DNS 등) 내에서도 SRE Agent 보안·컴플라이언스 요구를 충족하며 안전하게 운영할 수 있습니다.

### [Azure SRE Agent Live Reports 미리 보기](https://azure.microsoft.com/updates?id=569690)
SRE Agent 대화 내역을 기반으로 동적·자동 갱신 리포트 제공, 팀 단위 정보 공유와 빠른 의사결정 지원이 확대됩니다.

### [Node 22 LTS 지원 종료, Node 24 LTS로 업그레이드 필요](https://azure.microsoft.com/updates?id=567334)
2027년 4월 30일 Node 22 LTS 지원이 종료되므로 App Service 앱은 Node 24 LTS로 선제 업그레이드해야 합니다.

---

## 🌐 데이터베이스 & 기타 플랫폼

데이터베이스와 기타 플랫폼 영역에서는 Azure Database for PostgreSQL Flexible Server의 확장 지원으로 보안·패치·기술 지원이 보장되어 신버전 전환기에 안정적인 마이그레이션 환경을 제공합니다. Aspire 13.5는 대시보드, Interaction Service 확장 및 Kubernetes 볼륨 영속화 지원 등 앱 개발·운영 플랫폼의 혁신을 뒷받침하며, VM 이미지 빌더의 글로벌·주권 클라우드 자동화 지원 강화로 다양한 산업군이 데이터 주권, 컴플라이언스 요구에 대응할 수 있게 되었습니다. 이러한 기능들은 데이터·앱 관리의 미래 환경 구축에서 일관성, 보안, 확장성, 효율성까지 다각적 혁신을 이룹니다.

### [Azure Database for PostgreSQL Flexible Server 확장 지원 발표](https://azure.microsoft.com/updates?id=569526)
커뮤니티 지원 만료 이후에도 보안패치·버그수정 및 기술지원이 제공되어 안정성·신뢰성 있는 전환을 보장합니다.

### [Aspire 13.5 발표](https://azure.microsoft.com/updates?id=569910)
새 대시보드, Interaction Service 확대, Kubernetes 볼륨 영속화 등 개발·운영 플랫폼 혁신이 이루어졌습니다.

### [Azure VM Image Builder 글로벌·주권 클라우드 이미지 자동화 지원 강화](https://azure.microsoft.com/updates?id=570105)
주권·공공 클라우드에도 일관된 하드닝·검증·배포 프로세스 적용, 데이터 주권 및 컴플라이언스 환경에서 안전한 이미지 관리가 가능합니다.