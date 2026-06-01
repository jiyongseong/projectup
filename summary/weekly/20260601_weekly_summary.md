# Azure 주간 업데이트 요약 - 2026년 06월 01일

## 🌐 네트워킹 및 보안

지난주 네트워킹 및 보안 부문에서는 엔터프라이즈 애플리케이션과 네트워크를 위한 통합·자동화 기능이 주요한 흐름을 이뤘습니다. Application Gateway for Containers와 Istio 서비스 메시의 정식 통합은 클라우드 네이티브 환경에서 인증서 관리, mTLS 자동화, 단일 인그레스 구성 등 운영 효율성과 보안성을 대폭 강화합니다. 또한 가상 네트워크 흐름 로그를 Microsoft Sentinel과 직접 연동할 수 있게 되어, 보안 이벤트 대응과 네트워크 상태 가시성이 개선되었으며, 엔드-투-엔드 위협 탐지 및 통합 보안 분석이 더욱 용이해졌습니다. Virtual Network Manager와 Virtual WAN 통합을 통한 대규모 네트워크 정책 자동화 역시, 클라우드/하이브리드 환경에서의 정책 일관성 유지와 운영 부담 경감을 도모합니다. 전반적으로 이번 주 업데이트는 단순 관리 비용 절감뿐 아니라, 비즈니스 복원력 강화와 복잡한 네트워크 아키텍처의 실효적 대응 체계 마련이라는 측면에서 의미가 큽니다.

### [애플리케이션 게이트웨이 for Containers – Istio 서비스 메시 통합 정식 지원](https://azure.microsoft.com/updates?id=564714)
Istio 기반 서비스 메시에서 mTLS 연동, 인증서 수명주기 자동화 등 보안 및 운영 효율성 극대화. AKS와 오픈소스 Istio 모두 지원.

### [가상 네트워크 흐름 로그 Microsoft Sentinel 연동 정식 지원](https://azure.microsoft.com/updates?id=564689)
네트워크 흐름 로그의 Sentinel 즉시 연동이 가능, 네트워크-보안 데이터 통합 분석 및 사고감지 역량 향상.

### [Azure Virtual Network Manager와 Virtual WAN 통합 미리 보기 출시](https://azure.microsoft.com/updates?id=564478)
수백 개 스포크 네트워크를 동적으로 Virtual WAN 허브와 연동, 대규모 환경에서 네트워크 그룹 정책 및 라우팅 자동화 지원.

---

## 🛠️ 관리 및 마이그레이션

관리 및 마이그레이션 영역에서는 장기간 운영관점에서 IT 복원력과 자동화 중심의 혁신이 강화되었습니다. Azure Site Recovery가 Performance Plus 관리 디스크에 대해 미리 보기 지원을 시작, 프리미엄 SSD 환경 포함 다양한 워크로드의 무중단 재해복구가 가능해져 핵심 비즈니스의 연속성과 신뢰도가 향상되었습니다. 대규모 네트워크 관리 이슈 해소를 위해 Virtual Network Manager와 Virtual WAN을 통합·자동화하고, 네트워크 흐름 로그-보안 운영 시스템 연계 등 운영 프로세스 일원화도 진전되었습니다. 이러한 변화는 조직의 관리 복잡성을 줄이고, 정책 실행과 규정 준수, IT 리소스 재구성의 신속함을 실질적으로 지원합니다.

### [Azure Site Recovery – Performance Plus 관리 디스크 미리 보기 지원](https://azure.microsoft.com/updates?id=564644)
Premium/Standard SSD 및 HDD의 Performance Plus 환경까지 복제, 장애조치, 테스트 실행 지원. 중요 업무 중단 없이 재해복구 대비 가능해짐.

### [Azure Virtual Network Manager와 Virtual WAN 연동 미리 보기](https://azure.microsoft.com/updates?id=564478)
스포크 네트워크 연결 자동화, 그룹 정책 기반 라우팅 적용 등 대규모 클라우드 네트워크 관리 효율화.

### [가상 네트워크 흐름 로그 연동 – Sentinel 통합](https://azure.microsoft.com/updates?id=564689)
네트워크 및 보안 로그 분석의 자동화·통합이 강화되어 실시간 위협 탐지와 운영 거버넌스 향상.

---

## 🧩 플랫폼 및 서비스 혁신

플랫폼과 서비스 혁신 방향에서는 클라우드 마켓의 확장과 자동화 서비스 통합, 차세대 워크로드 대응 역량이 부각됐습니다. Microsoft Marketplace의 다중 파트너 프라이빗 오퍼가 유럽 30개국으로 확대되어, 법인과 파트너사가 안전하게 혁신적인 AI·서드파티 클라우드 솔루션을 유통/도입할 수 있게 됐으며, 파트너 기반 고객 지원 네트워크가 강화되었습니다. 네트워크, 애플리케이션 게이트웨이, Sentinel 등 기존 핵심 서비스에 통합형 신기능이 지속적으로 반영되고 있으며, 각종 정책 자동화, 클라우드 네이티브 보안, 운영 프로세스 통합이 전방위적으로 확장되는 추세가 이어지고 있습니다.

### [Microsoft Marketplace – 다중 파트너 프라이빗 오퍼 유럽 30개국 확대](https://azure.microsoft.com/updates?id=563016)
유럽 전역 파트너 연결이 강화돼 맞춤형 AI·클라우드 솔루션 도입과 고객사-파트너 공동 시장 확장 지원.

### [애플리케이션 게이트웨이 for Containers – Istio 통합](https://azure.microsoft.com/updates?id=564714)
서비스 메시, AKS 등 다양한 클라우드 인프라에 인그레스 경로 일원화. 운영 효율성과 보안이 동시 강화.

### [Virtual Network Manager와 Virtual WAN 허브 통합](https://azure.microsoft.com/updates?id=564478)
네트워크/정책 자동화, 하이브리드 네트워크 혁신의 기반을 제공하는 핵심 기술 미리 보기 제공.

---

## 🪐 미리 보기(Preview) 주요 업데이트

이번 주 공개된 미리보기(Preview)는 고가용성·자동화가 중요한 핵심 인프라에 집중되어 있습니다. Azure Site Recovery는 Premium SSD 등 고성능 관리 디스크 환경까지 재해복구 자동화를 확대, 복제·장애조치 과정에서의 성능 일관성을 보장합니다. Azure Virtual Network Manager와 Virtual WAN 통합도 대규모 네트워크 그룹에 대한 손쉬운 연결과 정책 배포 실현에 중점을 두고, 네트워크 흐름 로그를 Sentinel과 연동해 보안 사고 대응 자동화 실효성을 높입니다. 이러한 미리 보기 기능들은 대기업·기관 고객의 실제 클라우드 운영 과제 해결에 직접 연결되어, 품질 개선 및 실전 테스트가 활발히 이루어질 전망입니다.

### [Azure Site Recovery – Performance Plus 관리 디스크 지원 미리보기](https://azure.microsoft.com/updates?id=564644)
고성능 SSD/HDD 기반 VM도 재해복구 자동화 가능, 중요한 생산 워크로드의 비상복구 지원 범위 확대.

### [Azure Virtual Network Manager와 Virtual WAN 연동 미리보기](https://azure.microsoft.com/updates?id=564478)
수백 개의 VNet을 동적 그룹 정책 기반으로 Virtual WAN에 연결, 손쉬운 확장·정책 자동화 실현.

### [가상 네트워크 흐름 로그 – Sentinel 연동 미리보기](https://azure.microsoft.com/updates?id=564689)
Sentinel과 네트워크 흐름 데이터의 통합으로 통합 분석 및 보안사고 대응 역량 강화.

---

## 🇰🇷 한국 리전 관련 주요 업데이트

이번 주 Azure 공식 업데이트 중 한국(한국 중부, 한국 남부) 리전에 특화된 신규 서비스나 기능 정식 발표는 없었습니다. 다만, 글로벌 네트워킹 서비스 통합, 관리형 재해복구, AI 및 마켓플레이스 혁신 등 주요 기능은 한국 리전에 적극적으로 도입·확장될 수 있으니 향후 국내 공식 발표 및 지원 범위 변동에 유의할 필요가 있습니다. 지역별 특화 기능이 등장할 경우, 유관 기업·기관에 별도 상세 안내를 제공할 예정입니다.