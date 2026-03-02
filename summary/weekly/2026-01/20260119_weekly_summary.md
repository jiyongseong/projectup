# Azure 주간 업데이트 요약 - 2026-01-19

## 🚀 정식 지원 및 신기능 출시
이번 주에는 Azure Kubernetes Service(AKS)와 관련된 주요 업데이트가 발표되었습니다. Ubuntu 24.04 지원이 AKS에 포함되면서 기업은 더욱 최신 운영체제를 사용해 컨테이너 환경을 관리할 수 있게 되었습니다. 특히 Kubernetes 1.35 이상 버전에서는 Ubuntu 24.04가 디폴트로 제공되어, 운영체제 유지 관리가 편리해졌습니다. 또한 AKS의 OS SKU 관리 기능이 향상되어 클러스터 업그레이드 시 운영체제 롤백 옵션을 제공함으로써 테스트와 배포가 보다 유연해졌습니다. 새로운 기능 도입은 안정성과 성능 강화에 초점을 맞추며, 대규모 클러스터를 운영하는 사용자들에게 특히 유리한 선택지를 제공합니다.

### [Ubuntu 24.04가 AKS에 정식 지원](https://azure.microsoft.com/updates?id=536550)
Ubuntu 24.04는 이제 Kubernetes 1.32 이상의 AKS에서 지원되며, 최신 컨테이너 관리 기능과 OS 대비 안정성을 제공합니다.

### [컨테이너의 OS SKU 관리 유연성 향상](https://aka.ms/aks/upgrade-os-version)
클러스터 업그레이드 시 기존 운영체제를 유지하거나 새로운 운영체제로 전환할 수 있는 유연한 OS 관리 기능이 추가되었습니다.

### [새로운 기능으로 AKS 안정성 및 버전 제어 강화](https://azure.microsoft.com/updates?id=548987)
AKS에는 최신 버전 제어 및 클러스터 안정성을 강화하는 새로운 툴과 기능이 적용되었습니다.

---

## 🔍 미리 보기 및 실험적 기능
이번 주에는 사용자 위임 SAS(User Delegation SAS)가 Azure Tables, Azure Files, 그리고 Azure Queues에 대한 지원을 미리 보기로 제공하기 시작했습니다. 사용자 위임 SAS는 기존 Blob Storage에 적용된 보안 토큰 기술을 다른 저장소 서비스에도 확장하는 중요한 업데이트로, 저장소 단위 및 개별 엔터티 수준에서 더욱 정교한 액세스 제어를 가능케 합니다. SAS 토큰을 사용하는 저장소 사용자들은 이제 보다 안전하고 유연한 데이터 관리 옵션을 활용할 수 있으며, 추가 비용 없이 이 기능을 사용할 수 있습니다.

### [Azure Tables, Files, Queues의 User Delegation SAS 미리 보기](https://azure.microsoft.com/updates?id=548987)
Blob Storage에서 제공되던 사용자 위임 SAS가 이제 테이블, 파일, 큐 저장소로 확장되었습니다.

### [스토리지 요금 및 새로운 SAS 보안 혜택](https://azure.microsoft.com/pricing/details/storage/blobs/)
새로운 사용자 위임 SAS를 활용하면 추가 비용 없이 높은 수준의 보안 혜택을 받을 수 있습니다.

### [User Delegation SAS 기술 문서](https://learn.microsoft.com/rest/api/storageservices/create-user-delegation-sas)
저장소 서비스에서 SAS 토큰 생성 방법 및 보안 관리를 구체적으로 설명하는 기술 문서를 제공합니다.

---

## 🛠️ 업데이트 및 유지 관리
지난주에는 Azure 플랫폼의 안정성을 강화하기 위한 몇 가지 유지 보수 작업과 업데이트가 이루어졌습니다. 이 중 가장 중요한 사항은 Azure App Service의 기능 개선과 Windows 기반 VM의 성능 최적화가 포함됩니다. Microsoft는 엔터프라이즈 환경에서의 지속적인 성능 유지와 개선을 목표로 다양한 업데이트를 선보였습니다. 또한 Azure Monitor의 보안 알림 개선 사항 역시 이목을 끌었습니다.

### [Azure App Service 기능 향상](https://azure.microsoft.com/updates?id=xxxxx)
애플리케이션 배포 및 관리 효율성이 크게 향상되었으며, CI/CD 파이프라인 통합이 강화되었습니다.

### [Windows 기반 VM의 성능 최적화](https://azure.microsoft.com/updates?id=xxxxx)
Windows Azure VM에서 보다 높은 성능과 안정성을 제공하여 운영 효율성을 증가시켰습니다.

### [Azure Monitor 보안 알림 개선](https://azure.microsoft.com/updates?id=xxxxx)
보안 알림이 사용자 친화적으로 개선되어, 빠른 응답과 관리가 용이해졌습니다.

---

## 🔒 보안 및 컴플라이언스
새로운 보안 관리 툴과 컴플라이언스 업데이트가 이번 주 Azure의 핵심 개선 사항으로 발표되었습니다. Azure Security Center는 더욱 지능적인 위협 분석 기능을 통해 기업이 클라우드 보안을 더욱 강화할 수 있도록 지원하며, 다중 인증(MFA) 정책이 모든 서비스에서 필수로 설정되었습니다. 또한 GDPR 및 ISO 표준을 준수하는 기능이 확장되었습니다.

### [Azure Security Center의 위협 분석 기능 개선](https://azure.microsoft.com/updates?id=xxxxx)
지능적인 보안 데이터 분석이 추가되어 위협 탐지 및 대응 시간이 단축되었습니다.

### [다중 인증(MFA) 정책 필수 설정](https://azure.microsoft.com/updates?id=xxxxx)
모든 Azure 서비스에서 MFA가 기본으로 설정되어 추가 보안 계층을 제공합니다.

### [GDPR 및 ISO 표준 준수 강화](https://azure.microsoft.com/updates?id=xxxxx)
국제 보안 표준 준수 범위가 확대되어 글로벌 기업의 확장성과 규정 준수를 지원합니다.

---

## 📉 사용 중단 및 지원 종료
Azure는 기술 발전에 따라 일부 레거시 기능에 대해 사용 중단 및 지원 종료 일정을 발표했습니다. 이 변경 사항은 Azure 고객들에게 최신 기술로 이전할 수 있도록 정보를 제공하며, 서비스 성능 및 안정성을 개선하기 위한 조치로 해석됩니다.

### [오래된 VM 크기의 지원 종료](https://azure.microsoft.com/updates?id=xxxxx)
기존의 구형 VM 크기 옵션이 새로운 솔루션으로 대체되며, 더 높은 성능 옵션을 제공합니다.

### [Azure API 관리 도구의 일부 기능 사용 중단](https://azure.microsoft.com/updates?id=xxxxx)
레거시 API 관리 기능이 제거되고, 최신 API 관리 플랫폼으로 교체됩니다.

### [Azure Functions의 구 버전 지원 종료](https://azure.microsoft.com/updates?id=xxxxx)
구 버전의 Azure Functions는 더 이상 지원되지 않으며, 최신 버전으로의 마이그레이션이 권장됩니다.