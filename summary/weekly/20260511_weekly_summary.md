# Azure 주간 업데이트 요약 - 2026년 05월 11일

## 💻 컴퓨트 및 가상 머신

지난주 Azure는 차세대 인텔® Xeon® 6 기반의 D/E/Dl v7 가상 머신(VM) 정식 지원 등, 데이터센터 현대화 및 AI 워크로드를 위한 신규 VM 라인업을 발표했습니다. 최대 372 vCPU, 2.8TiB 메모리 등 대규모 워크로드 지원이 가능하며, 주요 VM 시리즈 예약 인스턴스의 지원 종료 예고로 인프라 재정비와 비용 최적화 필요성도 커졌습니다. 더불어, 스토리지 성능 혁신 및 VM 복구 자동화, 서버리스 환경 확장 등 대·중소기업이 모두 활용할 수 있는 컴퓨팅 개선이 대대적으로 이뤄졌습니다.

### [Azure Dl/D/E v7 가상 머신 정식 지원](https://azure.microsoft.com/updates?id=560734)
최신 인텔® Xeon® 6(Granite Rapids) 기반 가상 머신이 미국 중부 리전에 정식 출시되어 연산, 저장소, 네트워킹 모두 대폭 강화되었습니다.

### [Azure Functions Durable Task Scheduler Consumption SKU 정식 지원](https://azure.microsoft.com/updates?id=560957)
서버리스 기반 워크플로우 오케스트레이션 서비스의 구독 단위(SKU)가 정식 지원으로 전환되어, AI, 이벤트 처리 등 다양한 확장 시나리오에 비용 효율성과 자동 확장성을 제공합니다.

### [특정 VM 시리즈의 예약 인스턴스 지원 종료 안내(2026년 7월)](https://azure.microsoft.com/updates?id=560948)
기존 Av2, D, F 등 주요 VM 시리즈의 예약 인스턴스 신규 구매 및 갱신이 2026년 7월부터 순차적으로 종료되며, 최신 VM 시리즈로의 이전 및 비용 전략 수립이 필요합니다.


## ☁️ 스토리지 및 데이터 서비스

스토리지 분야에선 Azure Elastic SAN 및 NetApp Files의 기능성이 대폭 확장되었습니다. AVS(Private Cloud) 통합을 통해 VMware 환경에서의 대규모 스토리지 운용이 한층 효율적으로 진화했으며, 단일 볼륨 스냅샷, 기본 백업 설정 등 자동화와 데이터 보호도 강화됐습니다. 이외에도 프리미엄 SSD v2 디스크의 일본서부 3개 가용영역 지원, SAN을 통한 효율적 복구, 백업/복원 자동화 등의 기능이 추가되어, 미션 크리티컬 환경에서의 신속한 데이터 처리와 복구, 스토리지 확장성이 크게 높아졌습니다.

### [Azure Elastic SAN, AV64 SKU 정식 지원](https://azure.microsoft.com/updates?id=560894)
Azure VMware Solution(AVS) 환경에서 고성능·고용량 Elastic SAN 데이터스토어를 AV64 SKU로 유연하게 활용할 수 있습니다.

### [AVS Gen2 Private Cloud의 Azure Elastic SAN 지원](https://azure.microsoft.com/updates?id=560909)
ExpressRoute 없이 단일 프라이빗 엔드포인트 구성만으로 AVS Gen2 환경에서 SAN 성능 최적화 및 간편 배포가 가능합니다.

### [Azure Elastic SAN 단일 볼륨 스냅샷 정식 지원](https://azure.microsoft.com/updates?id=560899)
SAN 내 개별 볼륨을 대상으로 증분 스냅샷 백업·복원이 제공되어, 비용 효율성과 데이터 가용성이 한층 강화되었습니다.


## 🛡️ 네트워킹 및 관리

네트워크 및 관제 분야에서는 자동화·AI 기반 대량 복구 기능과 컨테이너 클러스터 관리 편의성이 대폭 개선되었습니다. Application Gateway for Containers가 AKS Automatic 환경에 미리 보기로 통합되어, 인그레스·로드밸런싱 관리를 더욱 자동화할 수 있습니다. 또한 대량의 VM 백업 복구(최대 100개) 및 Azure Communication Services 운영 정책 변경 등, 기업 운영의 연속성과 보안성, 유연성을 높이기 위한 업데이트가 이루어졌습니다.

### [Application Gateway for Containers, AKS Automatic 미리 보기 지원](https://azure.microsoft.com/updates?id=558403)
AKS Automatic 클러스터에서 관리형 Application Gateway for Containers의 손쉬운 통합 및 자동화가 가능합니다.

### [Teams Phone Multi-line 용 AlternateId 구성 변경 권고](https://azure.microsoft.com/updates?id=561432)
Azure Communication Services 내부 파라미터인 AlternateId의 고객 사용 중단이 즉시 권고되며, 미조치 시 서비스 중단 위험이 발생할 수 있습니다.

### [Azure Backup ‘벌크 복구’ 기능 미리 보기](https://azure.microsoft.com/updates?id=561373)
Azure Backup을 통한 대량 VM 복구 기능이 도입되어, 장애, 랜섬웨어 등 복구 시 신속성과 운용 효율성이 크게 개선됩니다.


## 🧠 데이터베이스 및 AI

데이터베이스 및 AI 부문에서는 Cosmos DB와 Azure SQL, Cognitive API 등 핵심 데이터·AI 서비스의 미리 보기 혁신과 주요 API의 지원 종료 관련 공지가 이어졌습니다. AI 기반 워크플로우 자동화, 대규모 벡터 데이터 처리 최적화, 메모리 자원 효율화, 백업 정책 강화 등 Big Data 및 AI 활용성을 크게 높여주는 기술 변화가 있었습니다. 또한, Azure Document Intelligence v3.0 API 지원 종료가 예고되어 최신 버전으로의 사전 이전 대응이 필요합니다.

### [Azure Cosmos DB Shell 미리 보기 출시](https://azure.microsoft.com/updates?id=561162)
AI 지원 커맨드라인 환경(MCP 기반) 제공으로 Cosmos DB 데이터 쿼리 및 워크플로우 자동화가 한층 고도화되었습니다.

### [Cosmos DB 구면 양자화 벡터서치 미리 보기](https://azure.microsoft.com/updates?id=561167)
고급 벡터 압축 기술인 구면 양자화로 고속·고정확도 벡터검색이 가능해져 AI/LLM 등 차세대 데이터 활용에 유리합니다.

### [Azure Document Intelligence v3.0 API 지원 종료(2029년 3월)](https://azure.microsoft.com/updates?id=561176)
기존 v3.0 API는 2029년 3월 30일에 지원이 종료될 예정이며, 데이터 추출 기능 지속 사용을 위해 v4.0으로 반드시 업그레이드해야 합니다.


## 🛠️ 구독 및 가격 정책, 서비스 사용 중단/종료

이번 주에는 대규모 인프라 구축 시 영향을 미칠 VM 시리즈 예약 인스턴스의 지원 종료와, 기존 AI·데이터 API 사용 중단 일정 등이 주요 이슈로 부각되었습니다. 특히, 예산 절감과 서비스 연속성을 위해 기존 VM 시리즈의 예약 인스턴스 운영을 점검하고, 문서지능 API 등 서비스의 사전 업그레이드, 장애 발생 시 대응방안 마련이 요구되고 있습니다. 국가별(일본서부 등) 서비스 가용성이 확장되어 글로벌 인프라 활용성도 증진되었습니다.

### [특정 VM 시리즈의 예약 인스턴스 지원 종료 안내(2026년 7월)](https://azure.microsoft.com/updates?id=560948)
주요 VM(Av2, D, F 등)의 1년 및 3년 예약 인스턴스 신규 구매/갱신이 2026년 7월부터 단계적으로 중단됩니다.

### [Azure Document Intelligence v3.0 API 지원 종료(2029년 3월)](https://azure.microsoft.com/updates?id=561176)
API 지원이 종료되어, 반드시 최신 버전(v4.0)으로의 신속한 업그레이드가 중요합니다.

### [Azure Premium SSD v2, 일본 서부 전체 가용 영역 출시](https://azure.microsoft.com/updates?id=561814)
최신 프리미엄 SSD v2가 일본 서부의 모든 가용 영역에서 지원되어, 글로벌 스토리지 운용 유연성과 성능이 크게 강화되었습니다.