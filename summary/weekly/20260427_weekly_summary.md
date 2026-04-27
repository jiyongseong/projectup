# Azure 주간 업데이트 요약 - 2026년 04월 27일

## 🗄️ 데이터베이스 및 분석 플랫폼

지난주 Azure는 데이터베이스 인프라의 확장성, 고가용성, 실시간 데이터 보호와 같은 엔터프라이즈 핵심 기능을 대폭 업그레이드하였습니다. Azure Database for PostgreSQL Flexible Server에서는 프리미엄 SSD v2 적용으로 성능이 4배 이상 향상되었고, 계층적 읽기 복제(최대 30개 복제본 지원)가 가능해져 대규모 글로벌 서비스 및 분석 환경에 최적화된 확장성을 제공합니다. 네트워킹 측면에서도 프라이빗 엔드포인트 지원 네트워크로의 무중단 마이그레이션, 논리적 복제 모니터링 지표 제공 등 데이터 거버넌스와 복원력 확보가 쉬워졌습니다. Cosmos DB의 동적 데이터 마스킹 정식 지원으로 개인정보 보호와 규제 준수도 강화되었습니다. Azure 데이터 분석 플랫폼은 전반적으로 성능, 보안, 운영 투명성을 높이며, 다양한 데이터 워크로드에 대응하도록 진화하고 있습니다.

### [Cascading Read Replicas, Azure Database for PostgreSQL의 단계적 읽기 복제 정식 지원](https://azure.microsoft.com/updates?id=560939)
계층적 읽기 복제로, 하나의 소스에서 최대 5개 복제본을 만들고, 2단계에 걸쳐 최대 30개까지 확장할 수 있어 글로벌 서비스의 성능과 가용성이 개선되었습니다.

### [Azure Cosmos DB의 동적 데이터 마스킹 정식 지원](https://azure.microsoft.com/updates?id=559633)
정책 기반 실시간 마스킹으로 민감 데이터의 안전한 노출을 지원하며, 보안 및 컴플라이언스 요구 사항 준수를 단순화합니다.

### [Premium SSD v2, Azure Database for PostgreSQL Flexible Server에 적용](https://azure.microsoft.com/updates?id=560336)
최대 4배 향상된 IOPS, 저장소와 성능의 유연한 독립 확장으로 트랜잭션 및 고성능 워크로드 대응력을 강화합니다.


## 🛠️ 관리 및 모니터링, 인프라 최적화

Azure의 최신 관리·모니터링 기능은 대규모, 하이브리드, 멀티클라우드 환경에서도 효율적이고 신뢰할 수 있는 IT 운영을 지원합니다. Azure Monitor Pipeline은 개방형 텔레메트리 수집 및 통합, 손실 방지, 자동화된 인증서 관리로 기업의 로그/이벤트 유입 최적화를 제공합니다. Elastic SAN에서는 사용량 기반 용량 자동 확장 및 CRC 오류 보호 등, 인프라 관리의 번거로움과 위험 요소를 제거하는 방향으로 발전하고 있습니다. AKS(쿠버네티스)에는 WireGuard 기반 네트워크 암호화가 추가되어, 관리 오버헤드를 최소화하면서 안전한 데이터 통신이 구현됩니다. 새로운 모니터링 지표와 자동화 기능은 IT담당자의 운영 효율과 예측력을 대폭 높여주고 있습니다.

### [Azure Monitor 파이프라인 정식 지원](https://azure.microsoft.com/updates?id=559886)
텔레메트리의 대규모 처리, 스키마 자동화, 중단 시 데이터 손실 방지, 중앙집중형 정책 적용 등 엔터프라이즈 모니터링 역량을 강화합니다.

### [Elastic SAN의 Capacity Autoscaling 정식 지원](https://azure.microsoft.com/updates?id=560919)
정책 기반 용량 자동 확장으로, 급변하는 워크로드 수요에 민첩하게 대응 가능한 비용효율적 SAN 환경이 구현됩니다.

### [AKS WireGuard 네트워크 암호화 정식 지원](https://azure.microsoft.com/updates?id=560015)
노드 간 트래픽 자동 암호화로 데이터 전송의 안전성과 자동화된 키 관리, 간편 운영을 제공합니다.


## 🚀 AI, 오픈소스, DevOps 및 하이브리드 클라우드

AI/DevOps 및 오픈소스 통합 분야에서 Azure는 하이브리드 및 멀티클라우드 업무를 위한 유연성, 실시간 모니터링, 혁신적 워크로드 전환을 지원합니다. Azure Monitor는 OpenShift 및 Arc 지원을 정식화하며, 컨테이너 환경과 관찰성이 완전하게 연동됩니다. SQL Server 마이그레이션 확대 및 OTLP 네이티브 수집 미리 보기는 운영 환경 간 자유로운 전환과 오픈소스 계측 표준 기반의 데이터 활용을 추구합니다. 애플리케이션 모니터링의 통합, 자동화된 지표 분석, 클라우드 이전 경로 다변화 등 다양한 혁신이 강화되었으며, 클라우드와 온프레미스의 경계를 효과적으로 해소합니다.

### [Azure Monitor: OpenShift 및 Azure Red Hat OpenShift 통합 정식 지원](https://azure.microsoft.com/updates?id=560358)
OpenShift, Azure Arc 기반 쿠버네티스까지 원활하게 연동, 모니터링, 관찰성 확보가 가능합니다.

### [Azure Arc, SQL Server on Azure VM 마이그레이션 대상 지원 (미리 보기)](https://azure.microsoft.com/updates?id=560805)
SQL Server 온프레미스-클라우드간 자유로운 아키텍처 전환 시나리오가 제공되어 마이그레이션 융통성이 크게 증가합니다.

### [Azure Monitor Agent, OpenTelemetry Protocol(OTLP) 네이티브 수집 미리 보기](https://azure.microsoft.com/updates?id=560530)
오픈소스 계측 데이터를 Azure Monitor, Application Insights, Grafana 등 다양한 도구에서 직접 분석할 수 있습니다.


## 🧬 Microsoft Fabric

Microsoft Fabric 부문의 업데이트는 Azure Database for PostgreSQL와의 통합을 심화하면서 데이터 통합, 분석 최적화, 운영 투명성 측면에서 뚜렷한 발전을 보였습니다. JSON, JSONB 등 네이티브 데이터형이 Fabric으로 전송 가능해져 데이터 거버넌스가 대폭 간소화되었으며, 미러링 권한 관리 간소화, 오류 추적 UDF 지원, 미러링 상태 실시간 모니터링이 추가되었습니다. 또한, 고가용성 환경과 Fabric의 결합도 확대되어, 신뢰성 높은 AI·분석 서비스 인프라를 보다 유연하게 설계할 수 있습니다. 이러한 변화는 실시간 분석 데이터 파이프라인 구축, 대용량 복합 워크로드 지원에 있어 Fabric 플랫폼의 경쟁력을 높이고 있습니다.

### [Azure Database for PostgreSQL, Microsoft Fabric 미러링 기능 향상 정식 지원](https://azure.microsoft.com/updates?id=560293)
네이티브 데이터 타입 지원과 권한·미러링 설정 간소화로, 다양한 데이터 구조와 복잡한 분석 파이프라인 구현이 쉬워졌습니다.

### [운영 모니터링 효율성 개선](https://azure.microsoft.com/updates?id=560293)
오류 메시지 투명화, UDF 기반 미러링 상태 확인 등 운영 중 가시성 향상 및 신속한 문제 대응이 가능합니다.

### [고가용성 엔진 조합 지원 확대](https://azure.microsoft.com/updates?id=560293)
Fabric과 PostgreSQL HA 환경 결합으로, 고신뢰·확장형 분석 및 AI 기반 서비스 설계가 용이해졌습니다.


## 🔒 스토리지, 보안 및 지원 정책

저장소와 보안 정책 영역에서는 데이터 무결성, 장기 데이터보호, 서비스 신뢰성 확보에 중점을 둔 개선이 이뤄졌습니다. Elastic SAN의 CRC-32C 체크섬 검증은 데이터 오류 감지 정확도를 높였으며, Azure NetApp Files의 고도화된 랜섬웨어 보호 기능은 위협 탐지, 자동 스냅샷, 공격 보고서 보존 등 선제적 보안 접근을 강화합니다. 백업 옵션, 장애 조치, 데이터 복구 전략의 다변화로 랜섬웨어 시대에 맞는 비즈니스 연속성 모델이 제시됩니다. 한편, .NET 8(LTS)의 지원 종료 예고로, 향후 보안/기술 지원을 위한 조기 업그레이드 필요성도 강조되고 있습니다.

### [Elastic SAN의 CRC 보호 정식 지원](https://azure.microsoft.com/updates?id=560889)
고급 오류 검출 기능으로 서비스 전체적인 데이터 무결성과 정책 기반 거버넌스를 보장합니다.

### [Azure NetApp Files 고도화된 랜섬웨어 보호(정식 지원)](https://azure.microsoft.com/updates?id=560188)
지능적 위협 탐지, 스냅샷, 보고서 제공으로 클라우드 저장소 환경의 신뢰성과 가용성이 크게 향상되었습니다.

### [.NET 8(LTS) 지원 종료 예고 – 2026년 11월 10일까지 업그레이드 권장](https://azure.microsoft.com/updates?id=558033)
중장기적으로 애플리케이션 및 클라우드 서비스의 보안, 성능, 안정성 유지를 위해 .NET 10(LTS)로의 전환 준비가 필요합니다.