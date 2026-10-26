# Azure 주간 업데이트 요약 - 2026년 10월 26일

## 🌀 서비스 출시 및 주요 기능 업데이트
지난주 Azure에서는 데이터 분석, 데이터베이스 보안, 백업 및 복구 등 핵심 클라우드 서비스에 대한 정식 지원 출시가 이루어졌습니다. ABFS Vectored Read 기능의 도입으로 Azure Data Lake Storage에서 인근 파일 범위 결합 및 비동기식 읽기 처리를 통해 분석 쿼리 성능이 비약적으로 향상되었습니다. Azure Cosmos DB의 안전 키 교체 기능은 각 계정 키의 마지막 사용 시점을 메타데이터로 확인하여 키 교체 이전에 활성 상태 파악이 가능해졌고, 서비스 중단 리스크를 줄여 credential 관리와 서비스 연속성을 최적화합니다. 또한 Azure Backup은 Premium SSDv2 및 Ultra 디스크를 사용하는 가상 머신에서 파일 단위 복구 기능을 제공함으로써 개별 파일/폴더의 신속 복구가 가능하게 되어 운영 효율성과 실수 복구 대응력이 대폭 향상되었습니다. 이러한 기능들은 대용량 데이터 처리 환경 및 고가용성 인프라를 운영하는 기업들에게 실질적인 보안 및 복구 유연성을 부여하며, 프로덕션 환경의 데이터 관리 신뢰도를 크게 끌어올렸습니다.

### [ABFS Vectored Read for Azure Data Lake Storage 정식 지원 출시](https://azure.microsoft.com/updates?id=577618)
분석 엔진에서 인근 파일 범위 결합 및 비동기식 읽기 실행으로 네트워크 트립 수를 줄이고 선택적 분석 성능을 극대화합니다. Spark 작업에 손쉽게 적용 가능합니다.

### [Azure Cosmos DB 안전 키 교체](https://azure.microsoft.com/updates?id=576716)
계정 키의 마지막 사용 시점을 메타데이터로 확인 가능하여 키 교체 전 활성 상태 파악 및 서비스 중단 리스크 감소, credential 관리와 연속성 최적화.

### [Azure VM Item Level Recovery for Premium SSDv2 및 Ultra 디스크](https://azure.microsoft.com/updates?id=577963)
VM 전체 복구 없이 개별 파일 또는 폴더를 선택적으로 복구 가능하며 운영 효율성 및 실수 복구 대응력이 대폭 향상됩니다.

---

## 📊 관측, 관리 및 모니터링
이번 주 Azure Monitor의 고급 플랫폼 메트릭과 메트릭 사용 인사이트가 정식 지원되며, 리소스 변경 및 트렌드 감지 정확도가 크게 향상됐습니다. 고급 플랫폼 메트릭은 세밀한 신호를 통해 운영 현황을 빠르게 파악할 수 있으며, 사용자는 Azure 포털에서 직접 활성화할 수 있습니다. 메트릭 사용 인사이트는 미활용 메트릭 탐지, 인게스트 트렌드 분석 등을 통해 비용 및 용량 계획, 효율적 리소스 배치에 도움을 주고 있습니다. Azure DNS와 Traffic Manager의 통합 로드밸런싱 기능 출시로 DNS 레코드셋과 Traffic Manager 프로필을 직접 연결할 수 있게 되어 CNAME 필요성이 해소되고 DNS 조회 지연 및 DNSSEC 호환성 개선 등 네트워크 관리 효율이 크게 높아졌습니다. 이러한 변화를 통해 기업은 관측 가능성, 관리 효율성, 네트워크 운영 속도 및 보안을 전반적으로 강화할 수 있게 되었습니다.

### [Azure Monitor 고급 플랫폼 메트릭 정식 지원](https://azure.microsoft.com/updates?id=575329)
리소스 변화 및 트렌드를 세밀하게 탐지하며, 구독별 Azure 포털에서 직접 활성화 가능합니다.

### [Azure Monitor workspace 메트릭 사용 인사이트 정식 지원](https://azure.microsoft.com/updates?id=577165)
메트릭 사용량 및 트렌드, 미사용 메트릭 시각화로 비용 절감과 용량 관리 최적화를 지원합니다.

### [Azure DNS 및 Traffic Manager 연동 로드밸런싱 기능 출시](https://azure.microsoft.com/updates?id=573917)
DNS 레코드셋과 Traffic Manager 프로필 직접 연결로 CNAME 필요성 제거 및 DNS 지연 감소, DNSSEC 호환성 향상.

---

## 🔒 네트워크 및 보안
네트워크와 보안 부문에서는 기업 인프라 보호와 트래픽 제어 강화를 위한 신규 기능이 발표되었습니다. Keyless TLS(비키 TLS)는 TLS 인증서를 보관할 때 프라이빗 키를 외부로 내보내지 않고 HSM 내부에서 TLS 핸드셰이크 시그니처를 수행해 최고 수준의 키 관리와 보안을 제공합니다. Azure Front Door Premium WAF는 서비스 태그 기반 매치 조건을 정식 지원하여 Azure 서비스별 IP 프리픽스 자동 관리, 민감 경로 트래픽 제어, 레이트 리미트 정책 적용 등 WAF 정책 유연성 및 보안 심화 효과를 얻을 수 있습니다. 또한 VNet Peering Route 미리 보기 기능은 대형 허브-스포크 네트워크에서 사용자 정의 경로로 트래픽을 집중 관리할 수 있도록 설계되어 네트워크 경로 관리의 복잡성을 줄이고 트래픽 제어 능력을 높입니다. 이로써 Azure 네트워크 전반에서 보안 수준과 운영 유연성이 실질적으로 향상됐습니다.

### [Application Gateway Keyless TLS 및 Managed HSM 연동](https://azure.microsoft.com/updates?id=577130)
TLS 프라이빗 키를 외부 장치로 내보내지 않고 HSM 내부에서만 사용해 FIPS 140-3 인증 보안 및 키 관리 신뢰도가 향상됩니다.

### [Azure Front Door Premium WAF 서비스 태그 매치 조건 정식 지원](https://azure.microsoft.com/updates?id=577156)
Azure 서비스별 IP 프리픽스를 자동 관리하여 민감 경로 트래픽 제어, 접근 제한 및 레이트 리미트 정책 구현이 용이해집니다.

### [VNet Peering Route 미리 보기](https://azure.microsoft.com/updates?id=576242)
피어링 경로 전파 제어로 대형 네트워크에서 사용자 정의 경로와 네트워크 가상 장비를 통한 트래픽 집중 관리가 가능합니다.

---

## 📬 플랫폼 및 IAM 관리
Microsoft Entra ID(구 Azure AD)의 "내가 선택하는 텔레포니" 정책이 2026년 10월 30일부터 적용되며, 조직은 SMS 및 음성 인증 방식에 대해 서드파티 제공업체를 직접 선택·관리할 수 있는 유연성이 부여됩니다. 기존 Microsoft 제공 인증 방식은 2027년 2월 1일부터 단계적으로 지원 종료가 예정되어 있으며, 이에 따라 인증 방식의 유연성과 개인정보, 규제 요구 대응력이 크게 높아집니다. 조직별로 관련 비즈니스, 규제, 기술 요건을 판단 후 구입·전환 준비가 필요하며, Azure 구독 자격 및 구매 정책, 비용 검토, 공급업체 평가 등 다각적 준비가 요구됩니다. 이는 Azure 환경에서 보안 정책, 통합 인증, 비용 관리 등에 영향을 끼칠 수 있으므로 전문 관리자의 분석과 선제적 대응이 필수적입니다.

### [Microsoft Entra: Choose Your Own Telephony 도입 안내](https://azure.microsoft.com/updates?id=577273)
SMS/음성 인증을 위한 지원사 제공업체 직접 선택 가능, 기존 MS 인증 서비스는 2027년 2월부터 단계적 지원 종료 예정. 규제, 보안, 비용 검토 및 구매 정책 준비 권장.

---

## 🌏 한국 리전 관련 업데이트
해당 주간 Azure 주요 업데이트 중 한국(Korea Central, Korea South) 리전에 특화된 콘텐츠는 공식적으로 발표되지 않았습니다. 앞으로 국내 리전 관련 최신 변경이나 서비스 출시가 확인될 경우, 해당 카테고리에 세부 정보를 즉시 추가하여 안내드리겠습니다.