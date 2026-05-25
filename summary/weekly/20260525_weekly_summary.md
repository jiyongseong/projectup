# Azure 주간 업데이트 요약 - 2026년 05월 25일

## 🚀 주요 서비스 및 플랫폼 업데이트

지난주 Azure는 다양한 핵심 서비스의 정식 지원과 혁신적 기능을 도입하며, 플랫폼 전체의 클라우드 자동화, 개발자 생산성, 인프라 보안 및 실시간 통신 역량을 한층 강화했습니다. SaaS 구독 자동 활성화 기능을 통해 Marketplace에서 SaaS 제품의 구매 즉시 서비스 사용 및 과금이 동시에 이루어져, 별도 활성화 과정 없이 즉각적인 서비스 도입이 가능합니다. 또한, Azure Kubernetes Service의 Application Insights 자동 계측 정식 지원으로, Java와 Node.js 기반 워크로드의 모니터링 자동화가 소스코드 변경 없이 이루어져 운영 생산성과 장애 진단 효율을 크게 향상시킵니다. 이 밖에도 Azure Front Door의 WebSocket 정식 지원이 추가되어, 금융·게임·챗·대시보드 등 실시간 데이터 송수신이 필수적인 시나리오에 안정적인 저지연 통신 환경을 제공합니다. 전반적으로 이번 업데이트는 네트워크, 운영, 개발자 경험 등 모든 측면에서 기업의 클라우드 활용 가치를 크게 높입니다.

### [Microsoft Marketplace의 SaaS 구독 자동 활성화](https://azure.microsoft.com/updates?id=561771)
SaaS 제품 구매와 동시에 구독과 과금이 자동 활성화되어 즉시 서비스 이용이 가능하며, 파트너별 활성화 정책도 사전 확인할 수 있습니다.

### [AKS 앱의 Application Insights 자동 계측 정식 지원](https://azure.microsoft.com/updates?id=562049)
Azure Kubernetes Service 앱에서 코드 수정 없이 Java/Node.js 워크로드의 모니터링이 가능해, 장애 분석 및 분산 추적 등 운영 효율이 개선됩니다.

### [Azure Front Door의 WebSocket 지원 정식 제공](https://azure.microsoft.com/updates?id=562548)
WebSocket이 기본 활성화되어 실시간 데이터/통신이 필요한 다양한 시나리오에서 높은 효율과 안정성 제공이 가능해졌습니다.


## 💾 데이터 및 스토리지 혁신

Azure는 데이터 관리와 스토리지 기반의 최신화와 운용 편의성 향상을 위해 여러 혁신적 기능과 신제품을 정식 출시했습니다. Azure NetApp Files의 캐시 볼륨 정식 지원을 통해 빈번하게 사용하는 데이터를 클라우드에서 직접 캐싱함으로써 WAN 지연·비용을 절감하고, 대규모 파일 분산 협업 및 하이브리드 환경에 최적화된 인프라를 실현할 수 있습니다. 또한, NetApp Files에 S3 호환 오브젝트 REST API가 도입되어 데이터 이동 없이 Microsoft Fabric, AI, 분석 서비스와 연동이 쉬워졌고, 보안 및 거버넌스도 강화됐습니다. 대규모 병렬 데이터 이전이 가능한 Azure Storage Mover의 Blob간 마이그레이션 지원도 기업의 데이터 이전, 통합, 아카이빙에 매우 유용합니다. 이처럼 Azure는 기업의 데이터 기반 비즈니스 의사 결정과 인프라 현대화를 강력하게 지원하고 있습니다.

### [Azure NetApp Files 캐시 볼륨 정식 지원](https://azure.microsoft.com/updates?id=562259)
주로 사용하는 데이터를 클라우드에 캐시해 대규모 파일 작업과 분산 협업 환경에서 지연을 줄이고, 비용 효율성을 높입니다.

### [Azure NetApp Files Object REST API 정식 지원](https://azure.microsoft.com/updates?id=562254)
전통적 파일 스토리지에 S3 호환 REST API가 도입되어 AI·분석·Fabric 등과의 연동이 간소화되고, 보안·규정 준수도 강화됩니다.

### [Blob간 데이터 마이그레이션을 지원하는 Azure Storage Mover](https://azure.microsoft.com/updates?id=562753)
Blob 컨테이너 간 대규모 병렬 데이터 이전·진행 추적이 가능해, 기업의 데이터 이전과 통합이 효율적으로 진행됩니다.


## 🔒 네트워크 및 보안 강화

이번 주 Azure는 네트워크 인프라 확장성과 보안 정책 강화를 중심으로 업그레이드를 단행했습니다. 네트워크 보안 그룹(NSG) 규칙 및 라우트 테이블의 기본 한도가 대폭 확장되어 대규모 엔터프라이즈 환경에서도 다양한 계층·서브넷에 정교한 보안 정책을 적용할 수 있습니다. 또한, Network Watcher의 규칙 영향 분석기가 정식 지원되어, 보안 그룹이나 네트워크 규칙 변경이 실제 트래픽에 미치는 영향을 사전에 시뮬레이션하고 네트워크 장애를 사전에 예방할 수 있게 되었습니다. Azure VPN Gateway에서는 인증서 기반 사이트 간 VPN이 가능해져 보안과 신뢰성이 크게 향상되었습니다. 이로써 Azure 네트워크는 확장성과 보안 두 축 모두에서 더욱 신뢰도 높은 운영이 가능합니다.

### [네트워크 보안 그룹 및 라우트 테이블 기본 한도 상향](https://azure.microsoft.com/updates?id=562695)
NSG 규칙, 주소/포트, 라우트 한도가 모두 대폭 확장하여 대규모 네트워크 구조에서 보안 정책 적용이 용이해졌습니다.

### [Network Watcher 규칙 영향 분석기 정식 지원](https://azure.microsoft.com/updates?id=562690)
네트워크 보안 규칙 변경이 운영 트래픽에 미치는 영향을 사전에 시뮬레이션하여, 오류나 네트워크 장애를 미리 예방할 수 있습니다.

### [Azure VPN Gateway의 인증서 기반 사이트 간 VPN 지원](https://azure.microsoft.com/updates?id=562705)
인증서 기반 비대칭 신뢰 모델 도입으로 보안성이 강화되고, 키 관리 편의와 인증 위조 위험이 감소합니다.


## 🧑‍💻 개발자 및 관리 도구 업데이트

Azure는 대규모 운영 환경에서의 자동화, 관리 효율성 및 AI 활용 확대를 위해 다양한 개발·운영 도구 기능을 강화하고 있습니다. Storage Actions에 Mock runs 기능이 도입되어 실제 데이터 변경 전 작업 시뮬레이션 및 영향 리포트 검증이 가능해졌으며, 데이터 관리 자동화의 신뢰성이 높아졌습니다. 또한, LangChain과 Cosmos DB의 Python 패키지 정식 지원으로 벡터 검색, 대화 이력 관리 등 대규모 AI 기반 애플리케이션 구축이 간편해졌습니다. Storage Mover는 마이그레이션 스케줄링까지 지원하여 반복적인 데이터 이전 시나리오도 자동화해, 관리 효율성과 예측 가능성을 한껏 높여줍니다.

### [Azure Storage Actions의 Mock runs 지원](https://azure.microsoft.com/updates?id=559494)
자동화 작업을 실제 실행 전에 시뮬레이션해, 영향 리포트 검증 및 안전한 데이터 관리 자동화가 가능합니다.

### [LangChain-Cosmos DB Python 패키지 정식 제공](https://azure.microsoft.com/updates?id=562074)
AI 기반 검색, 채팅, 코파일럿 구축 등에서 Cosmos DB를 데이터베이스로 직접 활용할 수 있습니다.

### [Azure Storage Mover의 마이그레이션 스케줄링 지원](https://azure.microsoft.com/updates?id=562622)
마이그레이션 작업을 반복 스케줄로 예약하여, 업무 시간 외 데이터 이전·무중단 이전 등이 가능합니다.


## 🧩 미리 보기, 사용 중단 및 규정 변화

마지막으로, Azure는 서비스 혁신을 지속하면서도 미래 아키텍처 대응과 보안 강화를 위한 각종 정책 변화와 신기능 미리 보기를 발표했습니다. TLS 1.0/1.1 보안 표준 지원이 2027년 5월말 지원 종료됨에 따라, 모든 클라이언트·애플리케이션은 TLS 1.2 이상으로 이전해야 하며, 이는 보안 수준을 한 단계 높이는 중요한 변화입니다. App Configuration의 Scorecards 기능(미리 보기)은 롤아웃 변화 효과를 텔레메트리 기반으로 정량 평가할 수 있어, 변화 탐지와 최적화가 더욱 쉬워집니다. 또한 ExpressRoute와 VPN Gateway의 라우트 광고 요약 기능(미리 보기)으로 대규모 네트워크 환경에서 효율적인 라우팅이 가능해지며, Azure의 신뢰성, 확장성, 보안성이 더욱 강화됩니다.

### [App Service/Functions/Logic Apps에서 TLS 1.0/1.1 지원 종료](https://azure.microsoft.com/updates?id=557852)
2027년 5월 31일부로 TLS 1.0/1.1 지원이 종료돼, 애플리케이션의 TLS 1.2 이상 지원이 필수화됩니다.

### [Azure App Configuration Scorecards(미리 보기) 출시](https://azure.microsoft.com/updates?id=561049)
피처 롤아웃 효과를 텔레메트리 기반으로 정량 평가 가능해, 변화 감지 및 문제 식별이 한층 체계화됩니다.

### [ExpressRoute·VPN Gateway 라우트 광고 요약 기능 미리 보기](https://azure.microsoft.com/updates?id=562813)
대규모 네트워크 환경에서 효율적인 라우트 광고로 환경 확장성과 운용 편의성이 크게 향상됩니다.